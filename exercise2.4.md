# Exercise 2.4: Adding a Button to Call a Flow in a Dataverse Form

In this exercise, you will learn how to add a button to a Dataverse form in a model-driven app that calls a Power Automate flow.

## Steps

### Step 1: Open your model-driven app

1. Navigate to [Power Apps](https://make.Power Apps.com/).
2. Select your model-driven app.

### Step 2: Edit the form

1. Go to the **Tables** section and select the table you want to modify.
2. Click on **Forms** and choose the form you want to edit.

### Step 3: Add a button

1. In the form designer, click on **+ Add** and select **Button**.
2. Configure the button properties (e.g., label, icon).

### Step 4: Configure the button to call a flow

1. Click on the button you added.
2. In the properties pane, find the **Action** section.
3. Select **Run Flow**.
4. Choose the flow you want to call from the list of available flows.
5. If needed, create a new flow to order snacks and notify Rizzo to fit with our scenario.
6. Add a new step to **Create an order** in your ordering system. (you could configure a Microsoft List 'list' for this, or create a new Dataverse table)
7. Add an action to create a row in either the list or Dataverse table.

### Step 5: Save and publish

1. Save your changes.
2. Click on **Publish** to make the changes live.

## Verification

1. Open a record in your model-driven app.
2. Verify that the button appears on the form.
3. Click the button and ensure it triggers the flow as expected.

## Optional

1. Explore how to make messages appear in the Model Driven app if the flow run was successful or not.

Congratulations! You have successfully added a button to a Dataverse form that calls a Power Automate flow.
