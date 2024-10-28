# Bonus Exercise: Creating a Canvas App for Power BI Integration

In this exercise, you will create a Muppet-themed Canvas App that can be embedded into Power BI, uses the Power BI integration data connection, and is able to call a flow.

## Prerequisites

- Google Chrome or Microsoft Edge browser
- A Power BI subscription, with the Muppet Opportunity Analysis Sample installed
- An understanding of how to create apps in Power Apps and how to edit Power BI reports

## Create a New App

When you add the Power Apps visual to your report, it launches Power Apps Studio with a live data connection between Power Apps and Power BI.

1. **Open the Muppet Opportunity Analysis Sample Report:**
    - Open the Muppet Opportunity Analysis sample report and select the Upcoming Opportunities page.
    - Open the report in Editing mode by selecting Edit from the Options bar.

2. **Prepare the Report Canvas:**
    - Move and resize some of the report tiles to make space for the new visual.
    - From the Visualizations pane, select the Power Apps icon, then resize the visual to fit the space you made.

3. **Select Fields for the Power Apps Visual:**
    - In the Fields pane, select Opportunity > Name, Product > Product Code, and SalesStage > Sales Stage.

4. **Create the App in Power Apps Studio:**
    - On the Power Apps visual, select the Power Apps environment where you want to create the app, then select Create new.
    - In Power Apps Studio, you see that a basic app is created, with a gallery that shows one of the fields you selected in Power BI.

5. **Customize the App:**
    - In the left pane, select Screen1, then set the screen's Fill property to "LightBlue" (so it shows up better in the report).
    - Select Gallery1 and make some room for a label control by changing Properties > Size > Height to 964.
    - Expand the left navigation menu, choose + Insert, and select Classic > Text label from the list of controls.
    - Drag the label to the bottom of your visual. Set the Text property to "Opportunity Count: " & CountRows(Gallery1.AllItems). The visual on the canvas now shows a total of 487 opportunities in the dataset.

6. **Save the App:**
    - Select the Save icon from the upper right corner. Save the app with the name "Muppet Opportunities App".
