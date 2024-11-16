## Exercise 4.1: Refreshing a Power BI Dataset with Power Automate

### Objective
Learn how to add a button in Power BI that triggers a Power Automate flow to refresh a dataset.

### Step 1: Add a Button in Power BI
1. Open your Power BI report.
2. Go to the **Insert** tab.
3. Select **Buttons** and choose the type of button you want to add (e.g., **Blank**).
4. Place the button on your report canvas and customize its appearance.

### Step 2: Create a Power Automate Flow to Refresh the Dataset
1. Go to [Power Automate](https://flow.microsoft.com).
2. Click on **Create** and select **Instant cloud flow**.
3. Name your flow and choose **Manually trigger a flow**.
4. Click **+ New step** and search for **Power BI**.
5. Select **Refresh a dataset**.
6. Choose the **Workspace** and **Dataset** you want to refresh.
7. Save your flow.

### Step 3: Implement the Flow with the Button in Power BI
1. Go back to your Power BI report.
2. Select the button you added.
3. In the **Visualizations** pane, go to the **Action** section.
4. Toggle the **Action** switch to **On**.
5. Set the **Type** to **Web URL**.
6. Paste the URL of the Power Automate flow you created.
7. Apply and save your report.


Now, when you click the button in your Power BI report, it will trigger the Power Automate flow to refresh the dataset.
