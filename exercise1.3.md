# Exercise 1.3: Preparing a Canvas App (Muppets Themed)

In this exercise, you will create a Muppets-themed Canvas App with a button to start a flow.

## Objectives
- Create a Canvas App
- Add a button to the app
- Configure the button to start a flow

## Steps

### Step 1: Create a Canvas App
1. Open Power Apps.
2. Select **Create** from the left-hand menu.
3. Choose **Canvas app from blank**.
4. Name your app "MuppetsApp" and select **Create**.

### Step 2: Design the App
1. In the app designer, add a background image of the Muppets.
2. Add a label to the screen with the text "Welcome to the Muppets App!".

### Step 3: Add a Button
1. From the **Insert** menu, select **Button**.
2. Drag the button onto the canvas and place it below the label.
3. Change the button text to "Start Flow".

### Step 4: Create a Flow
1. Open Power Automate.
2. Select **Create** from the left-hand menu.
3. Choose **Instant cloud flow**.
4. Name your flow "MuppetsFlow" and select **Manually trigger a flow**.
5. Add any desired actions to the flow.
6. Save the flow.

### Step 5: Connect the Button to the Flow
1. Go back to Power Apps.
2. Select the button you added.
3. In the **OnSelect** property, enter the following formula:
    ```plaintext
    'MuppetsFlow'.Run()
    ```
4. Save and publish your app.

### Step 6: Test the App
1. Open the app in preview mode.
2. Click the "Start Flow" button to ensure the flow is triggered.

## Summary
You have successfully created a Muppets-themed Canvas App with a button that starts a flow.

## Prerequisites
- Completion of previous exercises in this workshop.
- Basic understanding of Power Apps and Power Automate.
