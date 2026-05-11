# Lab 0 - Setup Dynamics 365 for Customer Service

## Scenario

Dynamics 365 for Customer Service is the backbone of their customer support operations. With hundreds of inquiries pouring in daily, the system effortlessly manages the entire customer service lifecycle. When a customer contacts the company with a product issue, a support agent swiftly creates a case in Dynamics 365, capturing all relevant details. The system intelligently assigns the case to the most suitable agent based on their expertise, workload, and availability. Armed with a comprehensive view of the customer's history, the agent promptly reaches out to the customer, providing personalized assistance and resolving the issue. Collaborating with colleagues within the system, they share knowledge articles and seek assistance when needed. The system ensures adherence to service level agreements, automatically escalating cases that require immediate attention. Managers leverage the system's analytics capabilities to monitor team performance, identify bottlenecks, and make data-driven decisions. After successful resolution, customer feedback surveys are automatically triggered, enabling the company to gauge customer satisfaction and continuously improve their support services. With Dynamics 365 for Customer Service at the helm, the company delivers exceptional customer experiences, solidifying their position as a leader in the industry.

In this practice lab, you will validate and set up your tenant.

## Exercise 1 - Access the Dynamics 365 application

### Task 1 – Log into the Power Platform admin center

1. Navigate to access <https://admin.powerplatform.microsoft.com> 

1. If not Sign-in, then on the **Sign into Microsoft Azure** tab you will see the login screen, in that enter following **Email/Username** and then click on **Next**. 
   * Email/Username: <inject key="AzureAdUserEmail"></inject>
   
    ![](https://github.com/CloudLabsAI-Azure/AIW-SAP-on-Azure/raw/main/media/M2-Ex1-portalsignin-1.png?raw=true)
    
1. Now enter the following **Password** and click on **Sign in**.
   * Password: <inject key="AzureAdUserPassword"></inject>

    ![](https://github.com/CloudLabsAI-Azure/AIW-SAP-on-Azure/blob/main/media/M2-Ex1-portalsignin-2.png?raw=true)

1. If you see the pop-up **Stay Signed in?**, click No.

    ![](../images/staysignedinNO.png)

1. If you see the pop-up **Welcome to the Power Platform admin center!**, click on **X** at top right corner.

1. Feel free to explore the Power Platform admin center but **do not make any changes.**

### Task 2 – Create Environment into the Power Platform admin center

1. On the Power Platform admin center, from the navigation pane, select **Manage (1)** and select **Environments (2)** and observe the **default environment present (3)**. Do not **use**, **modify**, or **delete** the **default** environment.

    ![](../images/Lab0-task2-1.png)

1. Next, select **Manage (1)** and on the **Environments (2)** pane, select **+ New (3)** to create a new environment.

    ![](../images/Lab0-task2-2.png)

1. On the **New environment** page, specify the following settings:

   - Type: Choose **Production (1)**
   - Name: Enter **Prod-Env (2)**
   - Click on **Change default settings (3)** 
   
    ![](../images/Lab0-task2-3.png)
    
1. Now scroll-down and enable **Add a Dataverse data store (1)** under default settings and click on **Next (2)**.
   
    ![](../images/Lab0-task2-4.png)

1. Next, click on **+ Select** under Security group.

    ![](../images/Lab0-task2-5.png)

   - On the **Edit security group page** select **None(1)** option from the list and click on **Done(2)**

    ![](../images/Lab0-task2-6.png) 

1. Next, enable the toggle button under **Enable Dynamics 365 apps (1)** and click on **Save (2)**.

    ![](../images/Lab0-task2-7.png)
   
   >**Note**: Wait for the Environment to get **ready** before you continue with this lab.   
   
> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - Hit the Validate button for the corresponding task. If you receive a success message, you can proceed to the next task.
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide. 
> - In case if you need any assistance, please contact us at cloudlabs-support@spektrasystems.com. We are available 24/7 to help you out.
   
### Task 3 - Installing Dynamic 365 Service Scheduling.

1. On the Power Platform admin center, select the **Prod-Env** environment.

   ![](../images/Lab0-task3-1.png)
    
1. Click on the drop-down next to **Resources (1)** and select **Dynamic 365 apps (2)**.

    ![](../images/Lab0-task3-2.png)
    
1. Click on **Install app** located on the command bar.

    ![](../images/Lab0-task3-3.png)
    
1. Search and select **Dynamic 365 Service Scheduling(1)** then click on **Next(2)**.

    ![](../images/scheduleselect.png)
    
1. On the **Install Dynamic 365 Service Scheduling** page, check the **I agree to terms of service (1)** box then click on **Install (2)**.

    ![](../images/Lab0-task3-4.png)
  
     >**Note:** It will take 25-30 minutes to get install. Once it got installed you can see that the status got changed from **Installing** to **Installed**. You can move on to the next task.
 
      ![](../images/install.png)

### Task 4 – Access the Dynamics 365 application

1. On the Power Platform admin center, select the **Prod-Env** environment.

   ![](../images/Lab0-task3-1.png)
   
1. Select the **Open** located on the command bar.

   ![](../images/Lab0-task4-1.png)

1. From the list of available Dynamics 365 apps, select the **Customer Service Hub** app.

   ![](../images/service-hub-app.png)

1. Spend a few minutes exploring the application.

1. You should now be showing the **Dashboard** view.

> **Note:** If the **Customer Service Hub** app doesn't appear in the list, follow below steps:

1. Copy and paste this link to navigate to Power apps page.

    ```
    https://make.powerapps.com/
    ```

1. Click on **Environment tab (1)** at top right corner, make sure that you are in **Prod-Env (2)** environment.

    ![](../images/Lab0-task4-2.png)

1. Select **Apps** from left panel.

    ![](../images/Lab0-task4-3.png)

1. Select **All (1)**, search for **Customer Service Hub (2)** and click on **Play &#x25B6; (3)** to open **Customer Service Hub** app.

    ![](../images/Lab0-task4-4.png)

> **Result:** You have successfully created your Dynamics 365 environment.

### Proceed with the next Lab.
