# Exercise 7: Combining RPA and Cloud Flows

## Objective
Learn how to call a Power Automate cloud flow from a desktop flow and vice versa.

## Prerequisites
- Power Automate Desktop installed
- Access to Power Automate (cloud)
- Basic understanding of creating flows

## Steps

### Step 1: Create a Cloud Flow

1. Go to Power Automate.
2. Create a new cloud flow.
3. Add a trigger (e.g., "When an HTTP request is received").
4. Add actions as needed.
5. Save the flow and copy the HTTP POST URL.

### Step 2: Create a Desktop Flow

1. Open Power Automate Desktop.
2. Create a new desktop flow.
3. Add an action to call the cloud flow using the HTTP POST URL.
   - Use the "Invoke Web Service" action.
   - Set the method to POST.
   - Paste the copied URL.
4. Save and run the desktop flow.

### Part 2: Call a Desktop Flow from a Cloud Flow

### Step 1: Create a Desktop Flow

1. Open Power Automate Desktop.
2. Create a new desktop flow.
3. Save the flow.
### Step 2: Create a Cloud Flow

1. Go to Power Automate.
2. Create a new cloud flow.
3. Add a trigger (e.g., "Manually trigger a flow").
4. Add an action to call the desktop flow.
    - Use the "Run a flow built with Power Automate Desktop" action.
    - Select the desktop flow you created.
5. Save and run the cloud flow.

## Conclusion
By completing this exercise, you have learned how to integrate Power Automate cloud flows with desktop flows, enabling seamless automation across different environments.
