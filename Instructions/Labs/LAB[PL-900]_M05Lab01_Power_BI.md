---
lab:
    title: 'Lab 5: How to build a simple dashboard'
    module: 'Module 5: Get Started with Power BI'
---

## Lab 5: How to build a simple dashboard

## Scenario

Bellows College is an educational organization with multiple buildings on
campus. Campus visitors are currently recorded in paper journals. The
information is not captured consistently, and there are no means to collect and analyze data about the visits across the entire campus.

Campus administration would like to modernize their visitor registration system where access to the buildings is controlled by security personnel and all visits are required to be pre-registered and recorded by their hosts.

Throughout this course, you will build applications and perform automation to enable the Bellows College administration and security personnel to manage and control access to the buildings on campus.

In this lab, you will build a Power BI report and dashboard that visualizes data about campus visits.

## High-level lab steps

We will follow the below steps to design and create a Power BI dashboard:

-   Create a report with various visualizations of the campus visits information

-   Utilize a user natural language query to build additional visualizations

## Prerequisites

- Completion of **Module 0 Lab 0 - Validate lab environment**
- Completion of **Module 2 Lab 1 - Data Modeling**

## Things to consider before you begin

-   Who is the target audience of the report?
-   How will the audience consume the report? Typical device? Location?
-   Do you have sufficient data to visualize?
-   What are the possible characteristics you can use to analyze data about the visits?

## Exercise 1: Create Power BI Report

**Objective:** In this exercise, you will create a Power BI report based on data the Excel spreadsheet we leveraged in a previous exercise.

### Task \#1: Prepare Power BI service

1.  You should have a visits.pbix file stored on your virtual machine in C:/LabFiles. Download [visits.pbix](https://github.com/MicrosoftLearning/PL-900-Microsoft-Power-Platform-Fundamentals/raw/master/Allfiles/visits.pbix) and save on your computer, if it's not already there.

2.  Open a new tab and navigate to <https://app.powerbi.com/> and sign in if needed.

3.  Select **My workspace** from the left side navigation.

5.  Select **Upload** then **Browse**.

6.  Locate and select the **visits.pbix** file you have downloaded earlier. 

7.  Once the data load is complete, select the **visits** report.

    Note that the Type is set to **Report**, do not select the Dataset.

8.  Select **Edit**. 

    If the **Edit** menu item is not visible, select the ellipsis **...** and then select **Edit**.

You have now setup Power BI service to use for your labs.


### Task \#2: Create Chart and Time Visualizations

1.  Press the **Pie chart** icon in the **Visualizations** panel to insert a chart.

2.  Press the drop-down arrow beside **bc_Visit** in the Fields pane. Drag the **Building** field and drop it into **Legend** box.

3.  Drag the **Visit** field and drop it into **Values** box.

4.  Resize the pie chart using corner handles so that all chart components are visible.

5.  Click on the report outside of the pie chart to deselect it and select stacked column chart in **Visualizations** pane.

6.  Press the drop-down arrow beside **bc_Visit** in the Fields pane. Drag the **Visit** field and drop it into **Y-axis** target box.

7.  Drag **Start** field and drop it into **X-axis** target box.

8.  In the Visualizations pane, click **x** next to **Year** and **Quarter** to leave only **Month** and **Day** totals for the Axis.

9.  Resize the chart as desired using the corner handles.

10. Test the report interactivity:

    1.  Click various building slices on the pie chart and observe changes on the time report.

    2.  Click on the column chart. Press the down arrow to turn on **Drill
        down** mode (or right click on the chart and select **Drill down**), then click a column to drill down to the next level (days).

    3.  Drill up and down and select various bars on the time column chart to observe changes on the pie report.

11. Save work in progress by pressing **Save**.

## Exercise 2: Create Power BI Dashboard

### Task \#1: Create Power BI Dashboard

1.  You should have the report open from the previous task.

2.  Select **Pin to a dashboard** on the menu. Depending on the layout you may need to press **...** to show additional menu items.

3.  Select **New dashboard** on **Pin to dashboard** prompt.

4.  Enter **Campus Management** as a **Dashboard name**, press
    **Pin live**.

5.  A pop-up will prompt you that the dashboard has been created. Select **Go to dashboard**.

6.  Test interactivity of the pie and bar charts displayed.

### Task \#2: Add Visualizations Using Natural Language

1.  Within your **Campus Management** dashboard, select **Ask a question about your data** bar at the top.

2.  Enter **buildings by number of visits** in Q&A area. A bar chart will be displayed.

3.  Select **Pin visual**.

4.  Select **Existing dashboard**, select your **Campus Management** dashboard, press **Pin**.

5.  Click **Exit Q&A**.

Your **Campus Management** dashboard should be displayed with three visuals on it. You may have to scroll down to see the new Q&A visual.

Your dashboard should look similar to the following:

![](media/5-powerbi-result.png)
