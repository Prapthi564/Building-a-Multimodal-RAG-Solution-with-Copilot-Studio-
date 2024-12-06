# Challenge: Develop a Health Symptom and Disease Identification Copilot agent using Azure OpenAI and Copilot Studio

### Estimated Time: 3 Hours
  
## Problem Statement

Develop an intelligent health symptom identification bot that helps individuals to assess potential diseases based on the symptoms they experience. The system will allow users to input their symptoms, which will then be matched against a database of diseases. The system will return a list of possible diseases associated with the provided symptoms, including their severity level, a brief yet informative description of each disease, and tailored precautionary steps or recommendations to manage or prevent further complications.

## Goals

- Match the input symptoms to a list of diseases.

- Display a brief description of each disease.

- Indicate the severity level of each disease (e.g., low, medium, high).

- Provide simple precautionary steps or recommendations for each disease.

## Datasets 

- Download and extract the datasets for this challenge using the [symptoms_datasets]() link.

## Accessing the Azure portal

1. To access the Azure portal, open a private/incognito window in your browser and navigate to the Azure Portal.

1. On the Sign in to Microsoft Azure tab, you will see a login screen. Enter the following email/username, and then click on Next.

   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>

1. Now enter the following password and click on Sign in.

   - **Password:** <inject key="AzureAdUserPassword"></inject>

1. If you see the pop-up Stay Signed in?, click No.

1. If you see the pop-up You have free Azure Advisor recommendations!, close the window to continue with the challenge.

1. If a Welcome to Microsoft Azure pop-up window appears, click Maybe Later to skip the tour.

## Challenge Objectives  

1. **Azure Blob Storage Deployment:**

   - Set up an Azure Blob Storage account with SKU size **Standard_LRS**.

   - Deploy it in the existing resource group named **copilot-<inject key="Deployment ID" enableCopy="false"/>**.

   - Ensure to provide the Azure Blob Storage account name as **blobstorage-<inject key="Deployment ID" enableCopy="false"/>**.

   - Create a container named **datasets**, upload the datasets that you have downloaded.

2. **Azure AI Search Resource Deployment:**

   - Set up an Azure AI Search resource with **Standard** tier.

   - Deploy it in the existing resource group named **copilot-<inject key="Deployment ID" enableCopy="false"/>**.

   -  Ensure to provide the Azure AI Search resource name as: **aisearch-<inject key="Deployment ID" enableCopy="false"/>**.

   - Copy the **URL** and **API Key** from the portal.

3. **Azure OpenAI Service Deployment :**

   - Set up an Azure OpenAI Service instance with SKU size **Standard S0**.

   - Deploy it in the existing resource group named **copilot-<inject key="Deployment ID" enableCopy="false"/>**.

   -  Ensure to provide the Azure OpenAI Service name as: **OpenAI-<inject key="Deployment ID" enableCopy="false"/>**.

   - Deploy the **GPT-4 model** and the **Text-Embedding** model within the Azure OpenAI Service from OpenAI Studio.

   - From the Chat Playground in OpenAI Studio, use the **Add Data Source** option to select Blob Storage as the source. Then, connect it with Azure AI Search to create **vectorized indexes**.

4. **Copilot Studio Setup and Agent Creation:**

   - Log in to [Copilot Studio](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjP2MGwj5GKAxV2hK8BHX7POdIQFnoECA4QAQ&url=https%3A%2F%2Fwww.microsoft.com%2Fen-us%2Fmicrosoft-copilot%2Fmicrosoft-copilot-studio&usg=AOvVaw1WLkkpGQ2nGBKuMr-VIVIC&opi=89978449)  using your credentials.

   - Create New Agent and provide the necessary details such as **Name**.

5. **Topic Creation and Knowledge Base Integration:**

   -  Create new topic and name the topic as **DiseaseIdentification**.

   - In the newly created topic, add a Generative Answers node and configure it to pull answers from the Knowledge Base.

   - Add previously created AI Search resource as Knowledge base.

   - Test the agent with some prompts.

6. **Publishing the Agent as Web App from Copilot Studio:**

   - Disable **authentication** from settings in Copilot Studio.

   - Configure **Demo Web App** as the channel to publish the agent.

   - Publish the agent, use the URL to navigate to the App.

## Success Criteria  

- Verify the agent by testing it with all the provided prompts to ensure it responds correctly and functions as expected:

  - `I have a rash and fever, could this be a viral infection?`

  - `Can you provide a summary of the symptoms and precautions for common respiratory diseases like the common cold, flu, and pneumonia?`

  - `I have a sore throat and fever, what diseases could this be?`

  - `I've been coughing and feeling short of breath, what conditions should I check?`

  - `Please list the diseases that require vaccination and give me a brief explanation of why they are important to prevent`

  - `I'm feeling chest pain and difficulty breathing, should I be worried about any particular disease?`

  - `Can you recommend simple precautions for managing chronic conditions like diabetes, hypertension, and asthma?`

  - `How does the severity of conditions like depression and anxiety compare with physical diseases such as pneumonia and tuberculosis?`

  - `I'm having digestive problems with bloating and irregular bowel movements, what conditions could this be?`

  - `I have a headache, nausea, and sensitivity to light, what could be causing this?`

- The agent should be deployed as a web app and made accessible online.

## Additional Resources:

- Refer to the [Copilot Studio Documentation](https://learn.microsoft.com/en-us/microsoft-copilot-studio/) for any clarifications or guidance during the challenge.

- Refer to the [Add your Own Data](https://learn.microsoft.com/en-us/azure/ai-services/openai/use-your-data-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython-new&pivots=ai-foundry-portal) for any clarifications or guidance during the challenge.

## Conclusion  

In this challenge, you have successfully developed a Disease Identification System using AI-powered technologies, with significant assistance from Azure OpenAI and Azure AI Search. Throughout the process, you utilized OpenAI's GPT-4 model for generating intelligent responses based on user inputs, integrated Azure Blob Storage for dataset management, and leveraged Azure AI Search to create vectorized indexes for efficient querying.

Your engagement with Copilot Studio enabled you to seamlessly create and configure the bot, design interactive workflows, and integrate the knowledge base for accurate disease identification. Testing the bot with various user queries confirmed the accuracy and relevance of its responses, ensuring a reliable user experience.
  

