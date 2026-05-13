# Lab 05 – Service Level Agreements

## Lab scenario

As a customer service manager at City Power & Light, you need to create a Service Level Agreement and make it the default agreement. In this lab, you will create an SLA and test it.

## Lab objectives

In this lab, you will perform:

+ Exercise 1 – Service Level Agreements

## Estimated time: 20 minutes

## Exercise 1 – Service Level Agreements

In this exercise, you will create a Service Level Agreement and make it the default agreement.

### Task 1 – Holiday Schedule

In this task, you will create A holiday schedule to be used with Customer Service calendars.

1.  Click on the **Customer Service Hub** app from the top and select **Customer service admin**.

    ![](../images/Customer-service-admin-1.png)
    
1.  In the site map, select **Calendar (1)** in Operations. The Calendar page appears.

1.  In the **Holiday calendar** section, select **Manage (2)**.

    ![](../images/Lab5-task1-1.png)

1.  Click **+ New**.

    ![](../images/Lab5-task1-2.png)

1.  Enter **Holidays (1)** for **Name** and click on **Create (2)**.

    ![](../images/Lab5-task1-3.png)

    > **Note :** If a pop-up appears stating "service-level agreements (SLAs) are deprecated in the web client" Click **I acknowledge**.

1.  In the Holidays section, click **+ New**.

    ![](../images/Lab5-task1-4.png)

1.  Enter **Local festival (1)** for **Name**, set the **Start Date (2)** and **End Date (3)** to be of two days duration, click **OK (4)**.

    ![](../images/Lab5-task1-5.png)
    
1. Click **Save & Close**.

    ![](../images/Lab5-task1-6.png)

### Task 2 – Customer Service Schedule

In this task, you will create a Customer Service Schedule to use with SLAs.

1. Click on the **Customer Service Hub** app from the top and select **Customer service admin**.

    ![](../images/Customer-service-admin-1.png)
    
1. In the site map, select **Calendar (1)** in Operations. The Calendar page appears.

1. In the **Customer service calendar** section, select **Manage (2)**.

    ![](../images/Lab5-task2-1.png)

1. Click **+ New**.

    ![](../images/Lab5-task2-2.png)

1. Enter **Customer Service Schedule (1)** for **Name** and click on **Create (2)**.

     ![](../images/customerservice.png)
     
1. Uncheck **Saturday (1)** and **Sunday (2)**. 

1. Click **Set Work Hours**.

1. Set Start to **9:00AM** and End to **5:00PM**. **(3)**

1. Click **OK**.

1. Set **Holiday Schedule** to **Observe (4)** and select the **Holiday Schedule (5)** you created.

1. Select your desired local **Time Zone (6)**

1. Click **Save & Close (7)**.

    ![](../images/Lab5-task2-3.png)

### Task 3 – Create Service Level Agreement

In this task, you will create a SLA that sets a 1 hour response time on a problem case.

1.  Click on the **Customer Service Hub** app from the top and select **Customer service admin**.

    ![](../images/Customer-service-admin-1.png)
    
1.  In the site map, select **Service Terms** in Operations.

1.  In the **SLA KPIs** section, select **Manage**.

    ![](../images/Entitlement-11.png)

1.  Click **+ New**.

    ![](../images/Lab5-task3-1.png)

1. On **New SLA KPI** page, follow the below instructions:

    - Enter **Case Response By** for **Name**.

    - Select **Case** for **Entity Name**.

    - Select **First Response By KPI** for **KPI Field**

    - Select **Created On** for **Applicable From**

    - Click **Save**. DO NOT navigate away from this form.

      ![](../images/caseresponseby.png)

1. Click **Activate** in the command bar.

    ![](../images/Lab5-task3-2.png)

1. Click **Activate** when the Confirm Activation dialog box appears.

    ![](../images/Lab5-task3-3.png)

1.  In the site map, select **Service Terms** in Operations.

1.  In the **Service Level Agreements** section, select **Manage**.

    ![](../images/Entitlement-13.png)

1. Click **+ New**.

    ![](../images/Lab5-task3-4.png)

1. On **New SLA** page, follow the below instructions:

    - Enter **SLA** for **Name**.

    - Select **Case** for **Primary Entity**.

    - Click **Save**.

      ![](../images/sla01.png)
      
1. Click **+ New SLA Item**.

    ![](../images/Lab5-task3-5.png)

1. A new window opens, enter **Problems (1)** for **Name**.

1. Search for and select the **SLA KPI (2)** you created for **KPI**.

1. Search for and select the **Customer Service Schedule (3)** you created for **Business Hours**.

    ![](../images/Lab5-task3-6.png)

1. Under **Applicable When**, click on **+ Add (1)** and **Add row (2)**.

    ![](../images/Lab5-task3-7.png)

1. In the left-hand side of the condition, select **Case Type (Case) (1)**.

1. Select **Equals (2)** for the operator.

1. In the right-hand side of the condition, select **Problem (3)**.

    ![](../images/Lab5-task3-8.png)

1. Under **Success Conditions**, click on **+ Add (1)** and **Add row (2)**.

    ![](../images/Lab5-task3-9.png)

1. In the left-hand side of the condition, select **First Response Sent (Case) (1)**.

1. Select **Equals (2)** for the operator.

1. In the right-hand side of the condition, select **Yes (3)**.

    ![](../images/Lab5-task3-10.png)

1. Set **Warn After** to **45 minutes (1)**.

1. Set **Failure After** to **1 hour (2)**.

1. Click **Save (3)**.

    ![](../images/Lab5-task3-11.png)

1. Click **Configure Actions**.

    >**Note:** The Configure Actions button only appears when the problem is saved.

    ![](../images/Lab5-task3-12.png)

1. If prompted to connect to Dataverse, click **Continue**.

    ![](../images/Lab5-task3-13.png)

1. Expand the **Switch** step.

    ![](../images/Lab5-task3-14.png)

1. Expand the **Is Non-compliant (1)** path, click on **Add an action (2)**.

    ![](../images/Lab5-task3-15.png)

1. Search for and select **Microsoft Dataverse**.

1. Select the **Update a row** action.

1. Select **Cases** for **Table name**.

1. Select **Regarding ID** for **Row ID**.

1. Click **Show Advanced options**.

1. Set **Is Escalated** to **Yes**.

1. Click **Save** and close the Power Automate browser tab.

    ![](../images/Lab5-task3-16.png)

1. Navigate back to **Customer service admin** and Click **Close** in the *SLA Item* dialog.

1. Click **Save**.

1. Click on **Activate (1)**. A dialog box appears to confirm SLA Activation, click on **Activate (2)**.

    ![](../images/Lab5-task3-17.png)

1. Select the **check-box (1)** on the left side of SLA, click **Set As Default (2)** option. Click **OK (3)** in the **Confirm Set as Default** pop-up.

    ![](../images/Lab5-task3-18.png)

### Task 4 – Service Level Agreement settings

In this task, you will configure the settings for service level agreements.

1. In the **Customer Service admin center** app, click on **Service Terms (1)** under Operations section.

1. Click **Manage (2)** on other settings area.

    ![](../images/Lab5-task4-1.png)

1. Verify that the **Disable SLAs** option is set to **No (1)**.

1. Set the **Apply SLA after manual override** to **Yes (2)**.

    ![](../images/Lab5-task4-2.png)

1. In **Select SLA Pause Status**, move **On Hold and Waiting for Details (3)** from Available to Selected.

    ![](../images/Lab5-task4-3.png)

1. Click on **Save**.

### Task 5 – Test Service Level Agreements

In this task, you will test that the SLA is applied to cases.

1. Switch back to the **Customer service Hub** tab.

1. Click on **Home** at the top of the left-hand side navigation.

1. Click on **Cases (1)** in the **Service** section of the sitemap and click **+ New Case (2)**.

    ![](../images/Lab5-task5-1.png)

1. Enter **SLA_Test #1 (1)** for **Case Title** and select the **Relecloud (2)** account for **Customer**.

1. Select **Web (3)** for **Origin** and click **Save (4)**.

    ![](../images/Lab5-task5-2.png)

1. Select **Details tab (1)** and in **Type section**, select **Problem (2)** from the drop-down click **Save (3)**.

    ![](../images/Lab5-task5-3.png)

1. Click on the **SLA (1)** tab. You should see the **Case Response By (2)** SLA KPI status as **In progress** with failure time set to 1 hour's time.

    ![](../images/Lab5-task5-4.png)

1.  Select the **Details (1)** tab and set **First Response Sent** to **Yes (2)** and click **Save (3)**.

    ![](../images/Lab5-task5-5.png)

1.  Select the **SLA (1)** tab. You should see the Case Response by SLA KPI with status on **Succeeded (2)**.

    ![](../images/Lab5-task5-6.png)
     
1.  Click **Go back**, click **+ New Case**.

    ![](../images/Lab5-task5-7.png)

1. Enter **SLA_Test #2 (1)** for **Case Title** and select the **Relecloud (2)** account for **Customer**.

1. Select **Email (3)** for **Origin** and click **Save (4)**.

    ![](../images/Lab5-task5-8.png)
    
1. Select the **SLA** tab. There should be no SLA KPI items.

    ![](../images/Lab5-task5-9.png)

**Result:** You have successfully created the Entitlements, Entitlement Templates, and Service Level Agreements in this lab. 

### Review

In this lab, you have completed:

- Create an entitlement for your user
- Add Channels to the entitlement and Tested the Entitlement
- Create Entitlement Templates and Tested the Entitlement
- Holiday Schedule and Customer Service Schedule
- Create and testing Service Level Agreement and settings

### Proceed with the next Lab.
