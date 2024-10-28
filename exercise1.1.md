# Power Automate Exercise: Actions, Triggers, Variables, and Data Operations

## Objective
Learn how to create a Power Automate flow that uses actions, triggers, variables, and data operations, all with a fun Muppets theme!

## Prerequisites
- Access to Power Automate
- Basic understanding of Power Automate concepts
- A love for the Muppets!

## Exercise Duration
45 minutes

## Steps

### Step 1: Create a New Flow (5 minutes)
1. Go to [Power Automate](https://flow.microsoft.com).
2. Click on **Create** and select **Automated flow**.
3. Name your flow "Muppets Flow".
4. Choose the trigger **When an item is created** (SharePoint).

### Step 2: Configure the Trigger (5 minutes)
1. Select your SharePoint site and list.
2. Click **New step**.

### Step 3: Add Actions (10 minutes)
1. Add an action **Get item** from SharePoint.
2. Configure it to get the item from the list where the trigger was fired.
3. Add an action **Initialize variable**.
    - Name: `muppetName`
    - Type: `String`
    - Value: `Title` from the SharePoint item.
4. Add an action **Compose**.
    - Inputs: `muppetName`

### Step 4: Add Data Operations (10 minutes)
1. Add an action **Filter array**.
    - From: `value` from the SharePoint list.
    - Condition: `Title` is equal to `muppetName`.
2. Add an action **Select**.
    - From: `Filter array` output.
    - Map: `Title` to `Title`, `ID` to `ID`.

### Step 5: Test the Flow (10 minutes)
1. Save the flow.
2. Go to your SharePoint list and create a new item.
3. Check the flow run history to ensure it executed successfully.
4. Verify the outputs of each action.

### Step 6: Review and Cleanup (5 minutes)
1. Review the flow and understand each step.
2. Delete the test item from the SharePoint list.
3. Optionally, delete the flow if no longer needed.

## Conclusion
By the end of this exercise, you should have a better understanding of how to use actions, triggers, variables, and data operations in Power Automate, all while having some Muppet-themed fun!

