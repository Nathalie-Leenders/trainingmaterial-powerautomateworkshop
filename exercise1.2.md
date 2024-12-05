# Exercise 1.2: Using a Power Apps Trigger

## Objective

In this exercise, you will learn how to use a Power Apps trigger to get input and output from a button in a Canvas app. This exercise should take approximately 45 minutes to complete.

## Prerequisites

- Basic understanding of Power Apps and Power Automate
- Completed Exercise 1

## Steps

### Step 1: Create a Power Automate Flow

1. Open Power Automate.
2. Create a new flow called MissPiggyText.
3. Select the `Power Apps V2` trigger.

### Step 4: Configure the Flow

1. Modify the action `Ask in Power Apps` to get input from the button.
2. Add a new action and choose `Initialize a variable` for your text (string type)
3. `Set the variable` to the text from your trigger. (optional)
4. Add any additional actions you need, in this case `send an email`, and `post a message in teams`.
5. Configure those items
6. Add an action `Respond to Power Apps` to send output back to the Canvas app.

### Step 5: Optional - Create message to be shown in the app

1. Upon succesful or failed running, display a custom message in the app.
2. Configure a run after, one for succesful, and paralele one for failed.
3. To do this, create a paralel branche. Add another Respond to Power Apps step.
4. Configure the run after, by clicking on the Elipsis (...) and going to the Configure run after settings.
5. For the Successful branch, check only the succesful box.
6. For the other side, select Failed, Is skipped or Timed Out.
7. In the success side `Respond to Power Apps` action, add a message text field, and add the following message: "Message succesfully sent to entire crew"
8. For the failed side, add "Message not sent to entire crew, check with IT"
9. For the logic in the canvas app to work, you'll need to create an if statement based on the flow run. Add another Text in the action `Respond to Power Apps`, with the name Workflowrun. 
10. Add in Success or Failed depending on the run after you're in. You'll need this later.


# Summary

You have successfully created a Canvas app with a button that triggers a Power Automate flow, gets input, and returns output. This exercise demonstrates how to integrate Power Apps and Power Automate to create interactive applications.

## Next Steps

- Experiment with different actions in Power Automate.
- Try adding more complex logic to your flow.
- Explore other triggers and connectors available in Power Automate.
