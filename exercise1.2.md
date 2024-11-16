# Exercise 1.2: Using a PowerApps Trigger

## Objective
In this exercise, you will learn how to use a PowerApps trigger to get input and output from a button in a Canvas app. This exercise should take approximately 45 minutes to complete.

## Prerequisites
- Basic understanding of PowerApps and Power Automate
- Completed Exercise 1

## Steps

### Step 1: Create a Power Automate Flow
1. Open Power Automate.
2. Create a new flow.
3. Select the `PowerApps` trigger.

### Step 4: Configure the Flow
1. Add an action `Ask in PowerApps` to get input from the button.
2. `Initialize a variable` for your text
3. `Set the variable` to the text from your trigger.
4. Add any additional actions you need, in this case `send an email`, and `post a message in teams`.
4. Add an action `Respond to PowerApps` to send output back to the Canvas app.

### Step 5 - Optional - Create message to be shown in the app
1. Upon succesful running, display a message in the app.

## Summary
You have successfully created a Canvas app with a button that triggers a Power Automate flow, gets input, and returns output. This exercise demonstrates how to integrate PowerApps and Power Automate to create interactive applications.

## Next Steps
- Experiment with different actions in Power Automate.
- Try adding more complex logic to your flow.
- Explore other triggers and connectors available in Power Automate.
