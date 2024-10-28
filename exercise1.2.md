# Exercise 1.2: Using a PowerApps Trigger

## Objective
In this exercise, you will learn how to use a PowerApps trigger to get input and output from a button in a Canvas app. This exercise should take approximately 45 minutes to complete.

## Prerequisites
- Basic understanding of PowerApps and Power Automate
- Completed Exercise 1

## Steps

### Step 1: Create a Canvas App
1. Open PowerApps.
2. Create a new Canvas app from blank.
3. Name your app `PowerAppsTriggerDemo`.

### Step 2: Add a Button
1. In the Canvas app, insert a button.
2. Set the button's `Text` property to "Submit".

### Step 3: Create a Power Automate Flow
1. Open Power Automate.
2. Create a new flow.
3. Select the `PowerApps` trigger.

### Step 4: Configure the Flow
1. Add an action `Ask in PowerApps` to get input from the button.
2. Add any additional actions you need (e.g., send an email, update a record).
3. Add an action `Respond to PowerApps` to send output back to the Canvas app.

### Step 5: Connect the Flow to the Canvas App
1. In PowerApps, select the button.
2. Go to the `Action` tab and select `Power Automate`.
3. Choose the flow you created.
4. Set the `OnSelect` property of the button to run the flow and handle the input/output.

### Step 6: Test the App
1. Save and publish your Canvas app.
2. Run the app and click the button.
3. Verify that the flow is triggered and the input/output works as expected.

## Summary
You have successfully created a Canvas app with a button that triggers a Power Automate flow, gets input, and returns output. This exercise demonstrates how to integrate PowerApps and Power Automate to create interactive applications.

## Next Steps
- Experiment with different actions in Power Automate.
- Try adding more complex logic to your flow.
- Explore other triggers and connectors available in Power Automate.
