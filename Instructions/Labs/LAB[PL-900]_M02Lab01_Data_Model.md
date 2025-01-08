---
lab:
    title: 'Lab 1: Data Modeling'
    module: 'Module 2: Identify foundational components of Microsoft Power Platform'
---

# Lab 1: Data Modeling

**WWL Tenants - Terms of Use**
If you are being provided with a tenant as a part of an instructor-led training delivery, please note that the tenant is made available for the purpose of supporting the hands-on labs in the instructor-led training. 
Tenants should not be shared or used for purposes outside of hands-on labs. The tenant used in this course is a trial tenant and cannot be used or accessed after the class is over and is not eligible for extension. 
Tenants must not be converted to a paid subscription. Tenants obtained as a part of this course remain the property of Microsoft Corporation and we reserve the right to obtain access and repossess at any time. 

## Scenario

Bellows College is an educational organization with multiple campuses and programs. Many of Bellow Colleges instructors and administrators need to attend events, and purchase items. Historically tracking these expenses has been a challenge. 

Campus administration would like to modernize their expense reporting system by providing employees with a digital way to report expenses. 

Throughout this course, you will build applications and perform automation to enable the Bellows College employees to manage expenses.

Finally, you will import sample data into Microsoft Dataverse.

## High-level lab steps

To prepare your learning environments you will:

- Refer to the [data model document]([https://github.com/MicrosoftLearning/PL-900-Microsoft-Power-Platform-Fundamentals/blob/master/Allfiles/Campus Management.png](https://github.com/MicrosoftLearning/PL-900-Microsoft-Power-Platform-Fundamentals/blob/master/Allfiles/Campus%20Management.png)) for the metadata description (tables and relationships). You can hold ctrl + left-click or right-click the link to open the data model document in a new window.

- Create Expense table

- Add some sample data. 

### Prerequisites

- Completion of **Module 1 Lab 0 - Validate lab environment**

Things to consider before you begin

- Naming conventions - enter names carefully.

## Exercise 1: Create New Table

**Objective:** In this exercise, you will create a new custom table for Expenses.

### Task #1: Create Expenses Table and Columns

The **Expenses** table will contain information about individual expenses that an employee can submit including reason, type, date, and amount.

1. If you are not already signed in, sign into https://make.powerapps.com

1. From the **Environment** menu in the top right, ensure the **Dev One** environment is selected.

1. Using the navigation on the left, select **Tables**.

1. Select **+ New table** and select **Table (advanced properties)** from the drop down menu.

1. For **Display name**, enter `Expense`

1. Select **Save**.

1. Under the **Schema** section, select **Columns**.

### Create Expense Date column

1. Select **+ New column**.

1. Enter `Expense Date` for **Display name**.

1. Select **Date only** for **Data type**.

1. Change **Required**, to **Business required**.

1. Expand **Advanced options**.

1. In **Time zone adjustment**, select **Date only**.

	>**Note:** We use **Date only** behavior to record date information, because date of the expenses should not change when viewed from a different time zone.

1. Select **Save**.

### Create Expense Type Column

1. Select **+ New column**.

1. Enter `Expense Type` for **Display name**.

1. Select **Choice** for **Data type**.

1. In **Required**, select **Optional**.

1. Set **Sync with global choice** to **Yes (recommended)**

1. In **Sync this choice with** field, select **Expense Type**.

1. Set the **Default choice** field to **None**.

1. Select **Save**.

### Create Expense Purpose Column

1. Select **+ New column**.

1. Enter `Expense Purpose` for **Display name**.

1. Select **Choice** for **Data type**.

1. In **Required**, select **Optional**.

1. Set **Sync with global choice** to **Yes (recommended)**

1. In **Sync this choice with** field, select **Expense Purpose**.

1. Set the **Default choice** field to **None**.

1. Select **Save**.

### Create Item Description column

1. Select **+ New column**.

1. Enter `Item Description` for **Display name**.

1. Select **Multiple Lines of text &gt; Plain Text** for **Data type**.

1. Select **Save**.

### Create Expense Amount column

1. Select **+ New column**.

1. Enter `Expense Amount` for **Display name**.

1. Select **Currency** for **Data type**.

1. Select **Save**.

 
## Exercise 2: Enter data

**Objective:** In this exercise, you manually enter some sample data into your new table. 

### Task #1: Modify the columns displayed

1. If not already signed in, sign in to https://make.powerapps.com

1. Select the **Dev One** environment at the top right if it is not already selected.

1. Using the navigation on the left, select **Tables**.

1. Open the **Expense** table created in the previous exercise.

1. Next to the **Name** column, select **+26 more**.

1. From the menu that appears, select the following columns.

	1. Expense Date

	2. Expense Purpose 

	3. Expense Type

	4. Expense Amount

	5. Item Description

1. Select the **Save** button.

## Task #2: Add a sample record.

1. Select the **Arrow** next to **Edit**. From the menu that appears, select **Edit in new tab**.

1. In the **Name** column, enter `John Doe`.

1. In the **Expense Date** column, enter **xxx**.

1. In the **Expense Purpose**, select **Conference**.

1. In the **Expense Type** column, select **Travel**.

1. In the **Expense Amount** column, enter `750.00`.

1. In the **Item Description**, enter a short description.

1. Hit the Tab button to advance to the next row and **save** the record.

Congratulations, you have successfully created a new table and added data.


