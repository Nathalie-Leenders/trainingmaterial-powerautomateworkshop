# Bonus Exercise: Integrate Cloud Flow with Power Pages (Muppets Theme)

## Prerequisites
- Power Pages license
- Power Apps Premium
- JavaScript knowledge

## Overview
In this bonus exercise, you will integrate a cloud flow with your Power Pages site. Ensure you have completed the Power Automate steps, have a Power Page ready, and for the next bonus exercise, you will connect a Dataverse table with a form.

## Steps to Integrate Cloud Flow

### Create a Cloud Flow
1. **Sign into Power Pages.**
2. **Select your site and click `Edit`.**
3. **Navigate to the `Set up` workspace, then select `Cloud flows` under `App integrations`.**
4. **Click `+ Create new flow`.**
5. **Search for `Power Pages` and select `When Power Pages calls a flow` trigger.**
6. **Define your flow steps and return values, then click `Save`.**

> **Note:** Only solution-aware flows can be attached to the Power Pages site.

### Step 3: Add the Flow to Your Site

1. Sign into Power Pages.
2. Select your site and click `Edit`.
3. Navigate to the `Set up` workspace, then select `Cloud flows (preview)` under `App integrations`.
4. Click `+ Add cloud flow`.
5. Search for the recently created flow.
6. Click `+ Add roles` under `Roles`.
7. Select roles that should have access to the flow.
8. Click `Save`.

> **Note:** When you add a flow to your site, a unique URL is generated that allows you to invoke the cloud flow from your site.

### Step 4: Invoke a Flow from Your Website

1. Use Power Pages cloud flow API to interact with Power Automate for external service integration.
2. Cloud flow API operations consist of HTTP requests and responses.

#### Operation Details
| Operation       | Method | URI                                      |
|-----------------|--------|------------------------------------------|
| Invoke cloud flow | POST   | `[Site URI]_/api/cloudflow/v1.0/trigger/<guid>` |

**Example:**

**Request:**
```http
POST https://contoso.powerappsportals.com/_api/cloudflow/v1.0/trigger/4d22a1a2-8a67-e681-9985-3f36acfb8ed4
{
    "Location": "Seattle"
}
```

**Response:**

*Cloud flow without response action:*
```http
HTTP/1.1 Accepted
Content-Type: application/json
```

*Cloud flow with response action:*
```http
HTTP/1.1 200 OK
Content-Type: application/json
{
    "conditions": "Rain",
    "humidity": "93",
    "latitude": "47.60620880126953",
    "longitude": "-122.33206939697266"
}
```

### Authenticating Cloud Flow API Requests
You don't need to include an authentication code, as the application session manages authentication and authorization. All API calls must include a Cross-Site Request Forgery (CSRF) token.

### Passing Parameters to Cloud Flow
In a cloud flow, you can define input parameters of type Text, Boolean, File, and Number. The parameter name in the request body should match the parameter name defined in the cloud flow trigger.

> **Important:**
> - You must pass the request parameters name as defined in the cloud flow.
> - Support for passing a parameter to a flow configured with secure inputs is not available.

### Sample JavaScript to Call a Flow
This sample demonstrates how to call a flow using Asynchronous JavaScript and XML (AJAX).

```javascript
shell.ajaxSafePost({
    type: "POST",
    url: "/_api/cloudflow/v1.0/trigger/44a4b2f2-0d1a-4820-bf93-9376278d49c4",
    data: JSON.stringify({
        "eventData": JSON.stringify({
            "Email": "abc@contoso.com",
            "File": {
                "name": "Report.pdf",
                "contentBytes": "base 64 encoded string"
            }
        })
    })
})
.done(function (response) {
    // Handle success
})
.fail(function(){
    // Handle failure
});
```

## Next Bonus Exercise
Connect a Dataverse table with a form.
