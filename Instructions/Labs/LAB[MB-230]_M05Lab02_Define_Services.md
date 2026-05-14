# Lab 09 – Define Services

## Lab scenario

You are the scheduling manager at City Power & Light who has been tasked with testing the Service Scheduling functionality to perform services for customers at your locations.

## Lab objectives

In this lab, you will perform:

+ Exercise 1: Define Services
+ Exercise 2: Create and schedule Service activities 

## Estimated time: 30 minutes

## Exercise 1: Define Services

In this exercise, you will define oil change and tire rotation services.

### Task 1: Create Oil Change Service

In this task, you will create an oil change service.

1. Open the **Dynamics 365 - Customer Service Hub (1)** app.

2. Click on **Home** at the top of the left-hand side navigation.

3. Click on **Service** at the bottom of the **Site Map** in the left-hand navigation and select **Scheduling (2)**.

4. Click on **Services (3)** in the **Scheduling** section.

5. Click **+ New (4)**.

   ![](../images/Change-Service-1.png)

6. Enter **Oil Change** for **Name** and click **Save**.

   ![](../images/oil-1.png)

7. Select the **Resource Requirements** tab, change the **Name** to **Oil Change (1)**, select **All** for **Select**, and select **Organizational Unit (2)** for **Part of Same**.

   ![](../images/oil-2.png)

8. Click **+ Requirement** from the command bar.

9. Enter **30 minutes** for **Duration (1)**.

10. Enter **Service Technician** for **Name** and select **Technician (3)** for **Resource Category**.

11. Select the **Oil Change** row.

    ![](../images/oil-3.png)

13. Select oil change and click **+ Requirement** from command bar.

14. Enter **Service Bay (1)** for **Name**, select **Service Bay Facility (2)** for **Resource Category**.

    ![](../images/oil-4.png)

15. Click **Save**.

### Task 2: Create Tire Service

1. Click + **New** in the command bar.

2. Enter **Tire Rotation (1)** for **Name** and click **Save (2)**.

   ![](../images/oil-5.png)

3. Select the **Resource Requirements (1)** tab, change the **Name** to **Tire Rotation (2)**, select **All (3)** for **Select**, and select **Organizational Unit (4)** for **Part of Same**.

    ![](../images/Lab9-task2-1.png)

4. Click **+ Requirement**.

5. Enter **1 hour** for **Duration**.

6. Enter **Senior Technician** for **Name** and select **Senior Technician** for **Resource Category**.

7. Select the **Tire Rotation** row and click **+ Requirement**.

8. Enter **Service Bay** for **Name** and select **Service Bay Facility** for **Resource Category**.

9. Select the **Tire Rotation** row and click **+ Requirement**.

10. Enter **Service Technician** for **Name** and select **Technician** for **Resource Category**.

11. Select the **Tire Rotation** row and click **+ Requirement**.

12. Enter **Tire Jack** for **Name** and select **Tire Jack Equipment** for **Resource Category**.

13. The **Tire Rotation** service should now have **4** requirements.

    ![](../images/oil-6.png)

1. Click **Save**.

## Exercise 2: Create and schedule Service activities 

In this exercise, you create and schedule service activities for an oil change and a tire rotation.

### Task 1: Schedule Oil Change Service

In this task you will create and schedule an oil change service activity.

1. Open the **Dynamics 365 - Customer Service Hub** app.

2. Click on **Home** at the top of the left-hand side navigation.

3. Click on **Service (1)** at the bottom of the **Site Map** in the left-hand navigation and select **Scheduling (2)**.

    ![](../images/Lab8-task1-2.png)

4. Click on **Service Activities (1)** in the **Scheduling** section and click on **Service Activity (2)** from the command bar.

   ![](../images/Lab9-ex2-task1-1.png)

6. Enter **Oil Change Service (1)** for **Subject**, select **Oil Change (2)** for **Service**, select **Main Ave Location (3)** for **Organizational Unit**, and click **Save**.
    
   ![](../images/oil-8.png)

7. Click on **Book** from the command bar.

8. Go to the **Filter View (1)**, select **Main Ave Location** for **Organizational Unit (2)**, and click **Search (3)**.

   ![](../images/oil-9.png)

9. Expand one of the available slots and see what resources are included in it.

   ![](../images/oil-10.png)

10. In our case Service Bay 1 and **Jennifer Leary (1)** will be included.

11. Click on the Team date from the list.

12. Select a **date one week from today(Do not select weekend date) (2)**. The rest of the dates will change to reflect the change you made.

13. Click **Book & Exit (3)**.

    ![](../images/oil-11.png)

14. Refresh the service activity record.

15. The status should now change form **Requested** to **Scheduled**.

16. Select the **Bookings** tab. You should see the booked resources for this service activity.

    ![](../images/oil-12.png)

17. Click **Scheduling** in the **Tools** section.

18. Select **Main Ave Location** for **Organizational Units (1)** and click **Apply (2)**.

    ![](../images/oil-13.png)

19. Select **Horizontal View** and click on the date picker.

20. Select the date you booked the **Oil Change** service activity.

21. **Jennifer Leary** and **Service Bay 1** should show as booked for **30** minutes. Click on the **Jennifer Leary’s** booking to get the details of booking.

    ![](../images/oil-14.png)

22. Go to the Details pane. You should see more information about the booking.

**Result:** You have successfully created Customer Service Scheduling Services in this lab.

### Review

In this lab, you have completed:

- Create Oil Change Service
- Create Tire Service
- Define Business Closure
- Create and schedule service activities for an oil change and a tire rotation
  
### Proceed with the next Lab.
