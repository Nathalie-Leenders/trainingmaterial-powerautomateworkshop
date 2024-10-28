# Exercise 2.5: Adding a Button to Call a Flow from the Ribbon Workbench

In this exercise, you will learn how to add a button to the ribbon in a Model-driven app that calls a Power Automate flow.

## Prerequisites

- Completion of Exercise 7
- Access to a Model-driven app
- Power Automate flow created

## Steps

### Step 1: Open Ribbon Workbench

1. Open your Model-driven app.
2. Navigate to the Ribbon Workbench.

### Step 2: Select the Entity

1. Select the solution that contains the entity you want to customize.
2. Drag the entity to the Ribbon Workbench design area.

### Step 3: Add a New Button

1. Right-click on the ribbon where you want to add the button.
2. Select "Add Button".

### Step 4: Configure the Button

1. Set the `Label` to a meaningful name.
2. Set the `Command` to a new command.

### Step 5: Create a Command

1. Right-click on the Commands section.
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