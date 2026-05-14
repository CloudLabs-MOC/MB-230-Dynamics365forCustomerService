# Lab 12 – Customer Voice

## Lab scenario

You are a customer service manager at City Power & Light who has been tasked with trying the new Customer Voice functionality to capture feedback on cases before rolling it out to your customers.

## Lab objectives

In this lab, you will perform:

+ Exercise 1: Create survey
+ Exercise 2: Send survey

## Estimated time: 20 minutes

## Exercise 1: Create survey

In this exercise, you will create a project and use a template to create a survey.

### Task 1: Create project

1.  Navigate to <https://customervoice.microsoft.com>

1. If not Sign-in, then on the **Sign into Microsoft Azure** tab you will see the login screen, in that enter following **Email/Username** and then click on **Next**. 

   - Email/Username: <inject key="AzureAdUserEmail"></inject>
   
    ![](../images/azure-login.png)
    
1. Now enter the following **Password** and click on **Sign in**.

   - Password: <inject key="AzureAdUserPassword"></inject>

1. If you see the pop-up **Action Required** page, select **Ask Later**.

1. Select **All projects (1)** and click on **New project (2)**.

    ![](../images/Lab7-task1-1.png)

1. Select the **Support (1)** template from the list. Click **Next (2)** to get Survey location page.

    ![](../images/Lab7-task1-2.png)

1. Select **See all environments** from the recent locations.

    ![](../images/resolution-31.png)

1.  Select the **Prod-Env (1)** Dynamics 365 environment and click on **select and close (2)**.

    ![](../images/resolution-30.png)

1.  Make sure **Prod-Env (1)** is selected and click **Create (2)**.

    ![](../images/Lab7-task1-3.png)

1.  Click on **All Projects (1)**

1.  Click on the **ellipsis (2)** next your project and select **Rename (3)**.

    ![](../images/resolution-29.png)

1.  Enter **Case Feedback (1)** and click on **Rename (2)**.

    ![](../images/Lab7-task1-4.png)

### Task 2: Customize survey

1.  Select your project.

2.  Click in the **Header** and change **Customer Service feedback** to **How did we do?**

3.  Hover the mouse over the header and click on the **Theme color** icon and change name inside HEX# box to **ffdd66**.

    ![](../images/resolution-28.png)

4.  Hover the mouse over the header and click on the **Image** icon and choose one of the images from the gallery.

    ![](../images/resolution-27.png)

5.  Select question 1 and set as **Required**.

    ![](../images/resolution-26.png)

6.  Select question 2 and set as **Required**.

7.  Select the last question in the survey and click on **+ Add new (1)** and click on the **chevron(V)(2)** and select the **Net Promoter Score (3)** question type. Set the question as **Required (4)**.

    ![](../images/resolution-24.png)

8.  Click on **Post-survey message** and change the Heading from *Thanks!* to **Thank you for your feedback (1)** and change the Message to **We look at all feedback to improve our service (2)**. 

    ![](../images/resolution-23.png)

9.  Click in the Footer and enter **The feedback you submit will not be shared outside of the company.**

    ![](../images/resolution-22.png)

10. Expand **Customization** and select **Personalization**.

    ![](../images/Lab7-task1-5.png)

11. Click + **Add variable (1)** and enter **casereference (2)** with default value **Your support case (3)**.

12. Click **Save (4)**.

    ![](../images/resolution-21.png)

13. Click **Close**.

14. Select **Formatting** from **Customization**.

15. Toggle **Progress bar** to **Off** and close the formatting pane.

    ![](../images/formatting.png)

16. Click into the **section header (1)** and clear the text *Input your title here*, click on the **variables (2)** drop down and select **casereference (3)**.

    ![](../images/resolution-20.png)

17. Add the text **has been resolved (1)** into the brackets.

    ![](../images/resolution-25.png)

18. Click **Preview (2)**.

    ![](../images/resolution-19.png)

19. Click **Back**.

### Task 3: Satisfaction metrics

1. Select your **project (1)** from the left panel.

1. Expand **Customization** and select **Satisfaction metrics (2)**.

   ![](../images/resolution-18.png)

1. Click **+ Add metric (1)**

1. Select **CSAT (2)** from the list.

   ![](../images/resolution-17.png)

1. Select the **first question (1)**.

1. Click **Save (2)**.

   ![](../images/resolution-16.png)

1. Click **+ Add metric**.

1. Select **Net Promoter Score** and select the **last question (1)**.

1. Click **Save (2)**.

   ![](../images/resolution-15.png)

1. Click **+ Add metric**

1. Select **Sentiment** and select the **text question (1)**.

1. Click **Save (2)**.

   ![](../images/resolution-14.png)

## Exercise 2: Send survey

In this exercise, you will create an email template and send the survey by email.

### Task 1: Configure email template

1. Navigate to <https://customervoice.microsoft.com>

2. Select your **project (1)** from the left panel.

3. Click on the **Send (2)** tab.

4. Click on the **Email (3)** tile.

   ![](../images/resolution-13.png)

5. Click on the **Template (1)** drop-down and select **Create new (2)**.

   ![](../images/resolution-12.png)

6. Enter **Case Resolution (1)** and click **Add (2)**.

   ![](../images/resolution-10.png)

7. Click on the **Insert (1)** drop-down and select **First question in survey (2)**.

   ![](../images/resolution-11.png)

8. Replace the subject line with **Please provide feedback on (1)**, click on the **Insert (2)** drop-down and select **Personalized variables (3)** and then select **casereference (4)**.

   ![](../images/resolution-8.png)

9. Click **Save**.

10. Click **Cancel**.

    ![](../images/resolution-9.png)

### Task 2: Send the survey

1. Click on the **Send** tab.

2. Click on the **Email** tile.

3. Click on the **Template** drop-down and select the **Case Resolution** template you created.

4. Click in the **Recipients field (1)** and enter **customer@contosot.com**.

5. Click **Send (2)**

     ![](../images/sendmail.png)

**Result:** You have successfully created the survey and Sent survey when a case is resolved. 

### Review

In this lab, you have completed:

- Create a project and use a template to create a survey
- Create an email template and send the survey by email.
- Use Power Automate to send a survey when a case is resolved.

### You have successfully completed the lab