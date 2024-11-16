# Power Automate Exercise: Actions, Triggers, Variables, and Data Operations

## Objective
Learn how to create a Power Automate flow that uses actions, triggers, variables, and data operations in Dataverse, all with a fun Muppets theme!

## Scenario
Fozzie Bear keeps losing his comedy props. Create a flow that automatically tracks and logs the location of each prop whenever it is moved.

## Prerequisites
- Access to Power Automate
- Basic understanding of Power Automate concepts
- Access to Dataverse
- A love for the Muppets!

## Exercise Duration
**45 minutes**

## Steps

## Step 0: Create your solution
1. Open Power Apps.
2. Select **Solutions** from the left-hand menu.
3. Create a new solution named **Muppet Power Automate workshop**.

### Step 1: Create a New Flow
1. Go to Power Automate.
2. Click on **Create** and select **Automated flow**.
3. Name your flow "Fozzie's Prop Tracker".
4. Choose the trigger **When a row is added, modified or deleted (Dataverse)**.

### Step 2: Configure the Trigger
1. Select your Dataverse environment.
2. Choose the table where you track props (e.g., Props).
3. Set the trigger to fire on **Added or Modified**.
4. Click **New step**.

### Step 3: Add Actions
1. Add an action **Initialize variable**.
    - **Name**: `propName`
    - **Type**: `String`
    - **Value**: `Name` from the Dataverse row.
2. Add an action **Initialize variable**.
    - **Name**: `propLocation`
    - **Type**: `String`
    - **Value**: `Location` from the Dataverse row.

### Step 4: Add Data Operations
1. Add an action **Compose**.
    - **Inputs**: `body` from the trigger output.
2. Add an action **Filter array**.
    - **From**: `body` from the Dataverse table/trigger output.
    - **Condition**: `Name` is equal to `propName`.
2. Add an action **Select**.
    - **From**: `Filter array` output.
    - **Map**: `Name` to `Name`, `Location` to `Location`.

### Step 5: Test the Flow
1. Save the flow.
2. Go to your Dataverse table and create or update a row.
3. Check the flow run history to ensure it executed successfully.
4. Verify the outputs of each action.

### Step 6: Review and Cleanup
1. Review the flow and understand each step.
2. Delete the test row from the Dataverse table.
3. Optionally, delete the flow if no longer needed.

## Conclusion
By the end of this exercise, you should have a better understanding of how to use actions, triggers, variables, and data operations in Power Automate with Dataverse, all while helping Fozzie Bear keep track of his comedy props!