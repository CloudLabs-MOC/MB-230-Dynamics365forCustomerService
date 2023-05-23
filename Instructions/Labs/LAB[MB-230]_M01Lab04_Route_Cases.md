# Practice Lab 4 – Routing cases

## Scenario

You are a customer service manager at City Power & Light who has been tasked with trying the new case routing functionality before rolling it out to your users. In this lab, you will create record creation rules, and case routing rules and test how they work.

## Exercise 1 – Configure record creation rules

### Task 1 – Enable a case to be created from an email in a queue

1. Click on the **Customer Service Hub (1)** app from the top and select **Customer service admin (2)**.

   ![](../images/Customer-service-admin-1.png)
    
1. Using the navigation on the left, select **Case settings (1)**.

1. Select **Manage (2)** next to **Automatic record creation and update rules**.

   ![](../images/creation-rules-10.png)

1. Click **+ New** located on the command bar.

1. Enter **Support email (1)** for **Rule name**.

1. Select the **Support (2)** queue you created for Queue to monitor and select **Email (2)** for Activity type to monitor.

   ![](../images/creation-rules-20.png)
    
1. Click **Save**.

1. In **Step two: conditions to evaluate and actions to take**, click **+ New**.

1. Enter **High priority emails (1)** for **Condition name**.

1. Click on **Add** and then select **Add row** from the drop-down.

1. In the left-hand side of the condition, select **Priority (Email) (2)** from the drop-down.

1. Select **Equals** from the drop-down for the operator.

1. In the right-hand side of the condition, select **High** from the drop-down.

1. Click **Save and open Power Automate (3)**.

   ![](../images/creation-rules-3.png)

1. If prompted to connect to Dataverse, click **Continue**.

1. If not Sign-in, then enter following **Email/Username** and then click on **Next**. 
   * Email/Username: <inject key="AzureAdUserEmail"></inject>
   
1. Now, enter the following **Password** and click on **Sign in**.
   * Password: <inject key="AzureAdUserPassword"></inject>

1. Expand the **Create a record (don't rename this step)** step.

   ![](../images/creation-rules-4.png)

1. Set the **Case Type** to **Request (1)**.

1. Set the **Priority field** to **High (2)**.

1. Click **Save (3)** and close the Power Automate browser tab.

   ![](../images/creation-rules-50.png)

1. Click **Close** in the *Record Creation and Update Rule Item* dialog.

2. In **Step three: additional actions to take after matching with a condition**, set *Automatically reply to email*  to **Yes (1)**.

1. In *Select email template*, search for and select **Case Auto Response (2)**.

1. Click **Save (3)**.

   ![](../images/creation-rules-61.png)

1. Click **Activate (1)** and then **Activate (1)** from popup.

   ![](../images/creation-rules-60.png)

1. Due to the lack of administrative access to email mailboxes, you will not be able to test this rule.

> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - Select the **Lab Validation** tab located at the upper right corner of the lab guide section.
> - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task. 
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

## Exercise 2 – Basic routing

### Task 1 – Configure basic routing rule set

1. Click on the **Customer Service Hub (1)** app from the top and select **Customer service admin (2)**.

    ![](../images/Customer-service-admin-1.png)
    
1. Click on **Routing (1)** in the **Customer support** section and then click on **Manage (2)** for **Basic routing rile sets**.

    ![](../images/Basic-routing-10.png)

1. Click **+ New** located on the command bar.

1. Enter **Basic case routing rules (1)** for **Name** and then click on **Save (2)**.

    ![](../images/Basic-routing-20.png)

1. Click **+ New Rule Item**.

    ![](../images/Basic-routing-21.png)

1. Click on **Add** and **Add row**.

    ![](../images/Basic-routing-22.png)
    
1. Enter **Problem (1)** for **Name**. 
    * In the left-hand side of the condition, select **Case Type (Case) (2)**. 
    * Select **Equals (3)** for the operator. for the condition, select **Problem (4)**.
    * Select **Queue (5)** for **Route To**.
    * Search for and select the **Gold (6)** queue you created in the earlier lab.
    * Click **Save & Close (7)**.

      ![](../images/Basic-routing-50.png)

1. Click **+ New Rule Item**.
    * Enter **Maintenance (1)** for **Name**.
    * Click on **Add** and **Add row**.
    * In the left-hand side of the condition, select **Subject (Case) (2)**.
    * Select **Equals (3)** for the operator.
    * In the right-hand side of the condition, select **Service (4)**.
    * Select **Queue (5)** for **Route To**.
    * Search for and select the **Silver (6)** queue you created in the earlier lab.
    * Click **Save & Close (7)**.

      ![](../images/Basic-routing-90.png)

1. Click **+ New Rule Item**.
    * Enter **Questions and Requests (1)** for **Name**.
    * Click on **Add** and **Add row**.
    * In the left-hand side of the condition, select **Case Type (Case) (2)**.
    * Select **Equals (3)** for the operator.
    * For condition, select **Question (4)** and select **Request**.
    * Select **Queue (5)** for **Route To**.
    * Search for and select the **Bronze (6)** queue you created in the earlier lab.
    * Click **Save & Close (7)**.

      ![](../images/Basic-routing-70.png)

1. Click **Save**.

36. Click **Activate (1)** and click **Yes (2)**.

    ![](../images/Basic-routing-71.png)

> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - Select the **Lab Validation** tab located at the upper right corner of the lab guide section.
> - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task. 
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

## Exercise 3 – Route cases

### Task 1 – Route cases

1.  Open the **Customer Service Hub** app.

2.  Click on **Home** at the top of the left-hand side navigation.

3.  Click on **Cases (1)** in the **Service** section of the sitemap.

4.  In the **Search this view** field, click on the lookup icon.

5.  Open the **Defective Screen Not Received (2)** case you created.

6.  Click **Queue Item Details (3)** located on the command bar.

    ![](../images/Basic-routing-72.png)

7.  The following message should be displayed *This record is not added to any queue.*

8.  Click **OK**.

    ![](../images/Basic-routing-73.png)

9.  Click **Save & Route (1)** and click **Route (2)**.

    ![](../images/Basic-routing-74.png)

10. Open the **Defective Screen** case again.

11. Click **Queue Item Details** located on the command bar.

12. The case will have been routed to the *Gold* queue.

    ![](../images/Basic-routing-76.png)

13. In the case view, click to the left of the **Service Required** case to select it.

14. Click **Apply Routing Rule** and click **Route**.

15. Open the **Service Required** case.

16. The case will have been routed to the *Silver* queue.
    
**Result:** You have successfully Configured the basic routing rule set and created the route cases in this lab. 
