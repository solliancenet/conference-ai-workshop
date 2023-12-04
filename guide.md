# Participant guide

## Access the user portal

FoundationaLLM provides a chat-based user interface (user portal) to interact with LLM agents and ask questions about your data. Complete the following steps to access the web app:

1. Navigate to <https://fllmad01chatuica.orangeisland-5b7e94c0.southcentralus.azurecontainerapps.io>
2. Select **Sign in**.

    ![FoundationaLLM sign in page.](media/sign-in-page.png)

3. When prompted, enter the `xxx_nnn@solliancetraining.onmicrosoft.com` email address we provided at the beginning of the session.

    ![Microsoft Entra ID signin form with provided username.](media/entra-id-username.png)

4. Select **Next**, enter your provided password at the prompt, then select **Sign in**.

5. **VERY IMPORTANT!** If you are prompted to download and set up the Microsoft Authenticator app within an Action Required dialog, select **Ask later**. Please **do not** set up multi-factor authentication with this account.

    ![Action Required dialog is displayed with the Ask later button highlighted.](media/ask-later.png)

6. The user portal appears with an empty chat history (1), input box for asking questions to the agent (2), and an agent select list (3) that lets you select either the default agent or the private anomaly agent that you will configure (more on this in a bit).

    ![The user portal is displayed as described above.](media/user-portal.png)

## Access the Azure storage account

FoundationaLLM (FLLM) follows a configuration-based approach to defining FLLM agents. This enables organizations to manage agents and their behaviors without requiring code modifications or new deployments. During this workshop, you will be modifying an anomaly agent to answer questions about rum product data stored in a SQL database. Each attendee has a private instance of the anomaly agent associated with their assigned account. You can only edit the metadata for your agent so you don't mess with anyone else's progress :)

Follow the steps below to sign in to Azure and access your files:

1. In a new browser tab, navigate to <https://portal.azure.com>.

2. If prompted, sign in with your `xxx_nnn@solliancetraining.onmicrosoft.com` account. When the portal comes up, you will see a notification that you do not have any Azure subscriptions.

    ![The Azure portal displays a notification that there are no subscriptions.](media/no-subscriptions.png)

3. Select the **Settings** button (1) in the top toolbar to switch directories. Select **Switch** next to the "Solliance, Inc." directory name. Please note, you might have to go through this step a number of times before the portal switches directories.

    ![The portal settings page is displayed with the settings icon and the Switch button highlighted.](media/azure-switch-directories.png)

4. Scroll down on the portal home page and select **Resource groups**, then select the `foundationallm-after-dark` resource group.

    ![Resource groups is highlighted on the Azure portal home page.](media/select-resource-groups.png)

5. Scroll down the list of resources and select the **fllmad01sa** storage account.

    ![The storage account is highlighted.](media/resource-group-storage-account.png)

6. Select **Storage browser** in the left-hand menu (1), expand **Blob containers** (2), then select the **user-profiles** container (3).

    ![The user-profiles storage container is selected.](media/storage-account-user-profiles.png)
