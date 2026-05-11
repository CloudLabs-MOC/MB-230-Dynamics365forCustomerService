# Lab 02 – Queues

## Lab scenario

You are a customer service manager at City Power & Light. You need to create queues for the customer service representatives to use for processing cases. In this lab, you will create a create multiple queues and add cases to activities to queues.

## Lab objective
In this lab, you will perform:

+ Exercise 1 – Create Queues

## Estimated time: 30 minutes

## Exercise 1 – Create Queues

In this exercise, you will create four queues.

### Task 1 – Create Queues

1.  Click on the **Customer Service Hub (1)** app from the top and select **Customer service admin (2)**.

    ![](../images/Customer-service-admin-1.png)

1. Click on **Queues (1)** in the **Customer support** section and then click on **Manage (2)** from right side.

    ![](../images/Customer-service-admin-2.png)

1.  Now click on **+ New** located on the command bar.

    ![](../images/Lab2-task1-1.png)

1.  Enter **Support (1)** for **Name** and select **Public (2)** for **Type**, and <inject key="AzureAdUserEmail"></inject> for **Incoming Email (3)**, then click on **Save (4)**.

    ![](../images/Customer-service-admin-3.1.png)

1.  Again, click **+ New** located on the command bar.

    ![](../images/Lab2-task1-2.png)

1.  Enter **Bronze (1)** for **Name** and select **Private (2)** for **Type**.

1.  Click **Save (3)**.

     ![](../images/Customer-service-admin-4.1.png)

1. Click **+ New** located on the command bar.

1. Enter **Silver (1)** for **Name** and select **Private (2)** for **Type**. Click on **Save (3)**.

    ![](../images/Lab2-task1-3.png)

1. Click **+ New**.

1. Enter **Gold (1)** for **Name** and select **Private (2)** for **Type**. Click on **Save (3)**.

    ![](../images/Lab2-task1-4.png)

1. Click on **Queues (1)** in the **Customer support** section and then click on **Manage (2)**.

    ![](../images/Customer-service-admin-2.png)

1. Select the **My Active Queues (1)** view.

1. You should now see a private queue that was created for your user automatically, the public queue, and private queues that you created in this lab.

    ![](../images/Customer-service-admin-7.1.png)

1. Navigate back to the previous **services** tab of **Customer Services Hub**.

1. On the Services page, refresh the page and Click **Queues** under the **Service** section.

    ![](../images/Lab2-task1-5.png)

1. Change the view from **Items I am working on** to **All items**.

    ![](../images/Lab2-task1-6.png)

1. Review the options in the list for **Queues I'm a member of (1)**. You should be able to see the **four queues (1)** you created.

    ![](../images/Lab2-task1-7.png)
    
### Task 2 – Add cases to queues

1.  Open the **Customer Service Hub** app.

1.  Click on **Cases** in the **Service** section of the sitemap.

    ![](../images/Lab2-task2-1.png)

1.  Select the **My Active cases** from the drop-down, and you will be able to see **Service Required**.

    ![](../images/adds-1.png)

1.  Select the **Service required** case you created in the earlier lab.

    ![](../images/Lab2-task2-2.png)

1. Then click on **3 dots** at the top and select **Add to Queue** located on the command bar.

    ![](../images/Lab2-task2-3.png)

1.  In the **Queue** field, click on the lookup icon and select the **Bronze (1)** queue you created in the task and then **Add (2)**

    ![](../images/add-2.1.png)

1.  Click on **Cases (1)** in the **Service** section of the sitemap. Select the **Defective Screen (2)** case you created in the earlier lab

    ![](../images/Lab2-task2-4.png)

1. Then click on **3 dots** at the top and select **Add to Queue** located on the command bar.

    ![](../images/Lab2-task2-5.png)

1. In the **Queue** field, click on the lookup icon and select the **Support (1)** queue you created in the task

1. Click **Add (2)**

    ![](../images/support-add-1.2.png)

1. Click **Queues (1)** under the **Service** section. Change the view from **Items I am working on** to **All items (2)**. You should see the **Service Required** case listed for the Bronze queue.

    ![](../images/bronze.png)

1. Change the queue selector from **Queues I'm a member of (1)** to **All Public Queues (2)**.

    ![](../images/Customer-service-admin-8.1.png)

1. You should see the Defective Screen case listed for the Support queue. Change the queue selector to **All Public Queues**.

    ![](../images/public.1.png)

### Task 3 – Perform actions on queue items

1.  Click **Queues** under the **Service** section. 

    ![](../images/Lab2-task1-5.png)

1.  Change the view from **Items I am working on** to **Items available to work on (1)**. Change the queue selector to **Queues I'm a member of (2)**. You should see the Service Required case listed for the Bronze queue.

    ![](../images/details-1.1.png)

1.  Click on the check-box to the left of the case in the queue to **select it (1)**, then click on **3 dots (2)** and select **Queue Item Details (3)** located on the command bar.

    ![](../images/Lab2-task2-6.png)

1.  Note that **Worked By** is blank.

    ![](../images/details-1.3.png)

1.  Click **three dots (1)** and select **Close (2)** from drop-down.

    ![](../images/Lab2-task2-7.png)

1.  Click to the left of the case in the queue to **select it (1)** then click on **Pick (2)** located on the command bar.

    ![](../images/pick-1.1.png)

1. Leave the *Also remove the item(s) from the Queue* option set to **No (1)**, and click **Pick (2)**.

    ![](../images/details-1.5.png)

1. Change the view from **Items available to work on** to **Items I am working on**.

1. Click on the check-box to the left of the case in the queue to **select it (1)**, then click on **3 dots (2)** and select **Queue Item Details (3)** located on the command bar.

    ![](../images/Lab2-task2-6.png)

1. Note that **Worked By** is set to **<inject key="AzureAdUserEmail"></inject>** user.

    ![](../images/worked-by-1.1.png)

1.  Click **three dots (1)** and select **Close (2)** from drop-down.

    ![](../images/Lab2-task2-7.png)

1. Click to the left of the case in the queue to **select it (1)**.

1. Click **Release (2)** located on the command bar and click **Release (3)**.

    ![](../images/release-1.1.png)
    
    **Result:** You have accomplished the creation of queues, inclusion of cases in the queues, and execution of actions on queue items.

### Review
In this lab, you have completed:
- Create queues and adding cases to queues
- Perform action on queue items

### Proceed with the next Lab.
