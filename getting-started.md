# Getting started with Challenge Environment

### Overall Estimated Duration : 4 Hours

Welcome to Copilot Hackathon, We've prepared a seamless environment for you to explore and learn. Let's begin by making the most of this experience.

### Accessing Your Challenge Environment

Once you're ready to dive in, your virtual machine and Challenge guide will be right at your fingertips within your web browser.

![](./media/gs-2.png)

### Exploring Your Challenge Resources

To get a better understanding of your Challenge resources and credentials, navigate to the Environment tab.

![](./media/gs-1.png)

### Utilizing the Split Window Feature

For convenience, you can open the Challenge guide in a separate window by selecting the Split Window button from the Top right corner

![](./media/gs-7.png)

### Managing Your Virtual Machine

Feel free to start, stop, or restart your virtual machine as needed from the Resources tab. Your experience is in your hands!

![](./media/gs-6.png)

## Let's Get Started with Azure Portal

1. In the JumpVM, click on **Azure portal** shortcut of Microsoft Edge browser which is created on desktop.

   ![](./media/gs-8.png)

2. On **Sign into Microsoft Azure** tab you will see login screen, in that enter following email/username and then click on **Next**.

   - Email/Username: <inject key="AzureAdUserEmail"></inject>
     
     ![](./media/gs-3.png)

3. Now enter the following password and click on **Sign in**.

   - Password: <inject key="AzureAdUserPassword"></inject>

     ![](./media/gs-4.png)

     >**Note:** If you see the Action Required dialog box, then select Ask Later option.

     ![](./media/gs-5.png)

4. If you see the pop-up **Stay Signed in?**, click No.

5. If you see the pop-up **You have free Azure Advisor recommendations!**, close the window to continue the Challenge.

6. If a **Welcome to Microsoft Azure** popup window appears, click **Cancel** to skip the tour.

## Creating Environment in Power Platform

1. From your browser, navigate to **Power Platform Admin Center** using this link [Power Platform](https://admin.powerplatform.microsoft.com/)

1. If the **Sign in** page is prompted, use the provided credentials to sign in to Power Platform and click **Next**.

   - Email/Username: <inject key="AzureAdUserEmail"></inject>

     ![](./media/pp-1.png)

1. Now, enter the following password and click on **Sign in**.

   - Password: <inject key="AzureAdUserPassword"></inject>

     ![](./media/pp-2.png)
   
1. On the **Stay signed in** pane, click on **No**.

   ![](./media/pp-3.png)

1. Once signed in, toggle **Try the new admin center** button to use new experience.

   ![](./media/pp-14.png)

1. Once you are in the **Power Platform Admin center** page, select **Manage (1)** from left menu and click on **+ New (2)**, to create a new environment.

   ![](./media/pp-4-updated.png)

1. In the **New environment** page, provide the following details and click on **Next (5)** :

   - **Name**: provide as **odl_user_<inject key="DeploymentID" enableCopy="false" />_env** **(1)**.

   - **Get new features early**: Toggle this option to **Yes (2)**.

   - **Type**: Select **Production (3)** from dropdown.

   - **Add a Dataverse data store**: Toggle this option to **Yes (4)**.

     ![](./media/pp-5.png)

1. In the next pane, click on **+ Select** under **Security group**.

   ![](./media/pp-6.png)

1. In the **Edit security group** pane, choose **None** option and click on **Done**.

   ![](./media/pp-7.png)

1. Once configurations are done, click on **Save**.

   ![](./media/pp-8.png)

1. Now the environment creation will start, please wait till the **State** changes from **Preparing** to **Ready**.

   ![](./media/pp-9.png)

## Accessing Copilot Studio

1. As you have now created a new environment, navigate to **Copilot Studio**  in a new tab using this link: [copilot studio](https://go.microsoft.com/fwlink/p/?linkid=2252408&clcid=0x409&culture=en-us&country=us)

1. On Welcome to Microsoft Copilot Studio page, Click on **Get Started**.

   ![](./media/pp-13.png)

1. If the **Welcome to Copilot Studio** prompt appears, click **Skip**.
 
1. Once you are inside **Copilot Studio** you will be in the home page. 

   ![](./media/ex1img3.png)

1. In the home page, select the environment option as shown.

   ![](./media/pp-10.png)

1. Change the environment to the new environment that you have created earlier. Keep the tab open as you will be using this in further exercises.

   ![](./media/pp-11.png)

1. Keep this browser tab open, you will be using this further.

1. Now, click on the **Next** from lower right corner to move on next page.

