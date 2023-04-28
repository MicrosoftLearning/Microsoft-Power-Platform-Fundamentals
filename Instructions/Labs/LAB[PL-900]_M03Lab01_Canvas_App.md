---
lab:
    title: 'Lab 2: How to build a canvas app'
    module: 'Module 3: Get started with Power Apps'
---

# Lab 2: How to build a canvas app

## Scenario

Bellows College is an educational organization with multiple buildings on campus. Campus visits are currently recorded in paper journals. The information is not captured consistently, and there are no means to collect and analyze data about the visits across the entire campus.

Currently, campus administration is leveraging an Excel spreadsheet to track visitor registration. They would like to modernize their visitor registration system where access to the buildings is controlled by security personnel and all visits are required to be pre-registered and recorded by their hosts.

Throughout this course, you will build applications and perform automation to enable the Bellows College administration and security personnel to manage and control access to the buildings on campus.

## High-level lab steps

We will follow the below outline to design the canvas app:

- Create a canvas app from data in the Visit table

- Configure how the visits are shown on the browse screen

- Make some basic changes to the app

- Test the app functionality

## Prerequisites

- Completion of **Module 0 Lab 0 - Validate lab environment**
- Completion of **Module 2 Lab 1 - Data Modeling**

## Exercise 1: Create Visits Canvas app

**Objective:** In this exercise, you will create a canvas app by connecting your Visits table you created earlier.

### Task \#1: Create the Visits app

1.  Navigate to <https://make.powerapps.com>. You may need to reauthenticate - click **Sign in** and follow instructions if needed.

2.  Select your **[my initials] Practice** environment at the top right if it is not already selected.

3.  If necessary, click the **Home** icon on the left side of the screen. Under the **Start from** section, select **Dataverse**.

4.  Select your Dataverse connection.

    > **NOTE:** *If a Dataverse connection does not exist:*
    > - Select **New Connection**
    > - Locate **Microsoft Dataverse**
    > - Click **Create**

5.  Locate and select the **Visits** table you created in the previous lab.

6.  Select the **Connect** button in the bottom right corner.

7.  After your app is created, On the Welcome to Power Apps Studio screen, check the **Don’t show me this again** box, and then select **Skip**.

8.  After creation has completed, is should look like the image below.

![Canvas app created from Visit data.](media/2-canvas-app-from-data.png)

9. In the app designer, select the **preview the app** button (Play icon) on the command bar. *(You can also preview the app by pressing F5 on your keyboard.)* Take a look around and see how your app looks out-of-the-box.

10. Close the app preview by selecting the **X** in the upper right of the screen.

Congratulations, you have successfully created a Power App from a Dataverse table. The next step in the process is to tailor the app to match your college's branding. The next series of steps will walk you through providing some extra customization to the app.

### Task \#2: Modify and theme the newly created app

In this task, you will customize the header text on each of the three screens for your app (Browse, Detail, and Edit) and change the app theme.

1.  You are on the Browse screen. Select the **Visits** label on the screen.

1.  On the right side of the screen, under the Properties tab, update the **Text** control property to **“Bellows College Visits”**.

1. In the properties, change the **Font size** to **24**.

1.  Click in the blank background of the screen to see the updated text on your Browse screen.

1.  Using the Tree view in the left-hand navigation, select **DetailScreen1**.

1.  Select the **Visits** label on the screen.

1.  On the right side of the screen, under the properties tab, update the **Text** control property to **“Visit Details”**.

1.  Click in the blank background of the screen to see the updated text on your Details screen.

1.  Using the Tree view in the left-hand navigation, select **EditScreen1** (you may need to scroll down to see this on the Tree view).

1.  Select the **Visits** label on the screen.

1.  On the right side of the screen, under the properties tab, replace the text Table1 in the **Text** control property with **“Edit Details”**.

1.  Click in the blank background of the screen to see the updated text on your Edit screen.

1. Using the Tree view in the left-hand navigation, select the **BrowseScreen1**.

1. On the command toolbar, select the **Theme** button and from the list that appears select the **Red** theme color.

### Task \#3: Test your Visits app

In this task, you will test out your new app.

1.  With your application open in the App Designer, select **Settings**, in the **General** section update the name of your app to **Visits App**, click the **X** to close the settings screen and then select **Save**.

2.  Select the **back** arrow to return to your app.

3.  Using the navigation on the left, select **BrowseScreen1**.

4.  In the app designer, select the **preview the app** button (Play icon) on the command bar. *(You can also preview the app by pressing F5 on your keyboard.)*

4.  Once the app opens, in the **Search Items** field, enter the text **Maria**
    *(Notice how the items in the gallery filter based on what is typed in the
    search field).*

5.  Once the **Contoso Suites** record for **Maria Campbell** is displayed,
    click on the row to navigate to open the details for that visit. (**Note**: *If more than one Contoso Suites Maria Campbell record is
    displayed, select any of them*)

6.  To edit the record, select the **Pencil Icon** in the upper right corner of
    the app.

7.  You can edit the Visit Name here and click the Checkmark icon in the top right to save the change.

8.  On the top right of the screen, click the **X** Icon to return to the canvas app editor.

Congratulations! You have created and configured your first canvas app.


