# Exercise 2.5: Adding a Button to Call a Flow from the Main Grid Command Bar

In this exercise, you will learn how to add a button to the main grid command bar in a Model-driven app that calls a Power Automate flow.

## Steps

### Step 0: Create a flow capable of receiving this

1. Create a flow, with the trigger When an HTTP request is received
2. Configure your actions to notify the Swedish Chef in advance about his required appearances.
3. Add an action to send an email to the Chef with the details of the show idea.
4. Optionally, add an action to update a shared calendar with the Chef's schedule.

### Step 1: Open Model-driven App Designer

1. Open your Model-driven app.
2. Navigate to the App Designer.

### Step 2: Select the Entity

1. Select the entity you want to customize.
2. Open the entity's main grid.

### Step 3: Add a New Button

1. Click on the "..." (more commands) in the main grid command bar.
2. Select "Edit Command Bar".

### Step 4: Configure the Button

1. Click on "Add" to add a new button.
2. Set the `Label` to a meaningful name.
3. Set the `Command` to a new command.

### Step 5: Create a Command

1. Click on "Commands" in the command bar editor.
2. Select "Add Command".
3. Set the `Action` to "JavaScript Action".
4. Write a JavaScript function to call the Power Automate flow.

### Step 6: Add JavaScript Web Resource

1. Create a new JavaScript web resource in your Model-driven app.
2. Add the following code to call the flow:

    ```javascript
    function callFlow() {
        var flowUrl = "YOUR_FLOW_URL";
        var req = new XMLHttpRequest();
        req.open("POST", flowUrl, true);
        req.setRequestHeader("Content-Type", "application/json");
        req.send();
    }
    ```

### Step 7: Publish Customizations

1. Save and publish your customizations.
2. Test the button in the main grid command bar to ensure it calls the Power Automate flow.
