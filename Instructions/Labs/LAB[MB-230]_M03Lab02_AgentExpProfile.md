# Lab 0 – Agent experience profiles

## Scenario

You are a customer service manager at City Power & Light who has been tasked with configuring the agent experience profiles for Customer Service workspace. In this lab, you will configure a new profile.

## Lab objectives

In this lab, you will perform:

+ Exercise 1: Create an agent experience profile
+ Exercise 2: Test the agent experience profile

## Estimated time: 30 minutes

## Exercise 1 – Create an agent experience profile

In this exercise you will learn how to create an agent experience profile in the Customer Service admin center.

### Task 1 – Manage agent experience profiles

1. Open the **Customer Service admin center** app. If you are in the Customer Service Workspace or Customer Service hub applications, click on the name of the app in the top left of the application next to Dynamics 365 and from the list of published apps, select the **Customer Service admin center** app.

    ![](../images/Lab13-task1-1.png)

2. In the Agent Experience section, click on **Workspaces (1)**.

3. On the **Workspaces** page, navigate to the **Experience profiles** area.

4.  Click **Manage (2)** in the Experience profiles area.

    ![](../images/Lab13-task1-2.png)

5.  Click on **+ New**.

    ![](../images/Lab13-task1-3.png)

6.  Enter **CS_Temp (1)** for **Name**, **mollyc_CS (2)** (without the space) for **Unique Name**. Click on **Create (3)**.

    > **NOTE:** Please be aware that your unique name must follow the specifications outlined under the text box. If your Unique Name is longer than 8 characters or contains anything other than alphanumeric characters, change it to comply with the requirements. Otherwise, you will receive an error.

    ![](../images/Lab13-task1-4.png)

8. Click **+ Add entity session template (1)** and click **+ Create entity session template (2)**.

    ![](../images/Lab13-task1-5.png)

1. Provide the following details:
    - For **Name**, enter **Entity Temp (1)**.
    - For **Unique Name**, enter **mollyc_ET (2)** (without the space).
    - For **Type**, Select **Entity (3)**.
    - For **Entity**, Select **Case (4)**.
    - For **Communication panel mode**, Select **Docked (5)**.
    - For **Title**, Enter **{casetitle} (6)**.
    - Click **Save (7)**.

    ![](../images/Lab13-task1-6.png)

8. In **Additional Tabs**, click on 3 dots and select **Add Existing Application Tab Template**.

    ![](../images/Lab13-task1-7.png)

9. Select the **Search** button to expand the dropdown list and select **Customer Summary (1)** and Click **Add (2)**.

    ![](../images/Lab13-task1-8.png)

10. Select the **Scripts** tab, click on **3 dots (2)** and select **Add Existing Script (3)**.

    ![](../images/Lab13-task1-9.png)

11. Click **+ New Record**, select **Agent scripts** and click **OK**.

12. Enter **Script1 (1)** for **Name** and **mollyc_script1 (2)** (without the spaces) for **Unique Name**. Click on **Save (3)**.

    ![](../images/Lab13-task1-10.png)

14. In **Script steps**, click **+ New Script step**.

    ![](../images/Lab13-task1-11.png)

1. If you receive *Leave this page?* Dialog box, click on **OK**.

    ![](../images/Lab13-task1-12.png)

1. Provide the following details:

    - **Name**: enter **Step 1 (1)**
    - **Unique Name**: enter **mollyc_step1 (2)**
    - **Order**: enter **1 (3)**
    - **Action type**: type **Text (4)**
    - **Text instructions**: type **Hi, how can I help you today? (5)**
    - Click **Save & Close (6)**.

    ![](../images/Lab13-task1-13.png)

17. You should return to the session template titled **Entity Temp.**

18. Select the **Scripts** tab (if it is not already open), click on **3 dots** and click **Add Existing Script**.

    ![](../images/Lab13-task1-14.png)

19. Select the **script1 (1)** you just created and click **Add (2)**.

    ![](../images/Lab13-task1-15.png)

20. Select **Save and close.**

    ![](../images/Lab13-task1-16.png)

21. You should return to the **Entity session templates** screen on your **Agent experience profile**. Select **+ Add**.

    ![](../images/Lab13-task1-17.png)

22. Select **Case (1)** for **Entity** and select your **Entity Temp (2)** template for Session template. Click **Add (3)**.

    ![](../images/Lab13-task1-18.png)

23. Select **Save and close**.

    ![](../images/Lab13-task1-19.png)

### Task 2 – Configure the productivity pane 

1. On your agent experience profile, select **Turn on** in the Productivity pane section.

    ![](../images/Lab13-task2-1.png)

2. Toggle **Productivity pane** to **On (1)**.

3. Toggle **Default mode** to **Expanded (2)**.

4. Toggle **Smart assist** to **On (3)**.

5. Toggle **Agent scripts** to **On (4)**.

6. Select **Save and close (5)**.

    ![](../images/Lab13-task1-2.png)

### Task 3 – Assign users to the agent experience profile

1. On your agent experience profile, select **+ Add users** in the Users section.

    ![](../images/Lab13-task3-1.png)

2. Search for **ODL_User**, select the **user (2)** from the list and click on **Add (3)**.

    ![](../images/Lab13-task3-2.png)

## Exercise 2 – Test the agent experience profile

In this exercise you will test the agent experience profile you created.

### Task 1 – Open the Customer Service workspace

1. Open the **Customer Service workspace** app. If you are in the Customer Service admin center, click on the name of the app in the top left of the application next to Dynamics 365 and from the list of published apps, select the **Customer Service workspace**.

    ![](../images/Lab13-task4-1.png)

2. In the Customer Service Agent Dashboard, find the **Defective Screen Not Received** case, and click on the case to open it.

    ![](../images/Lab13-task4-2.png)

3. A new session starts in the left-hand pane for the case and **Smart assist** opens in the **Productivity pane** and a **Customer Summary (1)** tab is available. Explore the Smart assist.

4. Click on the **Scripts (2)** icon. You should see the script created earlier in this lab.

    ![](../images/Lab13-task4-3.png)

### Review

In this lab, you have completed:

- Create an agent experience profile with a case session template
- Add a Customer Summary tab and an agent script to the session template
- Enable and configure the productivity pane with smart assist and agent scripts
- Assign users to the profile and verify it in the Customer Service workspace

### Proceed with the next Lab.