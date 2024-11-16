# Exercise 1.3: Preparing a Canvas App (Muppets Themed)

In this exercise, you will create a Muppets-themed Canvas App called "Miss Piggy's Communication Assistant" with a button to start a flow.

## Objectives
- Create a Canvas App
- Add a button to the app
- Configure the button to start a flow

## Prerequisites
- Completion of previous exercises in this workshop.
- Basic understanding of Power Apps and Power Automate.
- Existing flow created in Exercise 1.2.

## Steps

### Step 1: Create a Canvas App
1. Open Power Apps.
2. Select **Solutions** from the left-hand menu.
3. Open the solution named **Muppet Power Automate workshop**.
4. Select **New** and choose **App** > **Canvas app**.
5. Name your app "Miss Piggy's Communication Assistant" and select **Create**.

### Step 2: Design the App
1. In the app designer, add a background image of the Muppets.
2. Add a label to the screen with the text "Welcome to Miss Piggy's Communication Assistant!".

### Step 3: Add a Button
1. From the **Insert** menu, select **Button**.
2. Drag the button onto the canvas and place it below the label.
3. Change the button text to "Start Flow".

### Step 4: Connect the Button to the Flow
1. Go back to Power Apps.
2. Select the button you added.
3. In the **OnSelect** property, enter the following formula:
    ```plaintext
    'MissPiggyText'.Run(textinput1.text)
    ```
4. Save and publish your app.

### Step 4.5: Optional - Display a success or error message
1. Change your onselect code on the button to:
```powerfx
Set(varFlowoutput,MissPiggyText.Run(TextInput1.Text)); 
If(varFlowoutput.workflowrun="Failed", 
Notify(varFlowoutput.message,NotificationType.Error),
Notify(varFlowoutput.message,NotificationType.Success))
```

### Step 5: Test the App
1. Open the app in preview mode.
2. Click the "Start Flow" button to ensure the flow is triggered.

## Summary
You have successfully created a Muppets-themed Canvas App called "Miss Piggy's Communication Assistant" with a button that starts a flow.


