# Setup Generative AI Hub in SAP AI Launchpad


SAP AI Launchpad provides generative AI capabilities via the Generative AI Hub.

On order to use it, you have to set up Generative AI Hub.




### Create a Configuration for Generative AI Hub


**Procedure**

1. Enter your Subaccount for AI Launchpad and open "Services" --> "Instances and Subscriptions" in the Navigation pane. Open your AI Launchpad.


2. Navigate to "ML Operations" --> "Scenarios". Make sure you see the "foundation-models" for Generative AI Hub.

   ![](images/29_ail_foundationmodels.png)

3. Open "ML Operations" --> "Configuration" and click "Create"

   ![](images/31_genai_create.png)

4. Provide a name of your choice. Select Scenario, Version and the "Executable".   

    For more information on Executables, see [SAP Help Portal](https://help.sap.com/docs/sap-ai-core/sap-ai-core-service-guide/models-and-scenarios-in-generative-ai-hub?locale=en-US&q=generative)
    
    ![](images/32_genai_conf_step1.png)

5. Provide the model name (see list of [available models on SAP Help Portal](https://help.sap.com/docs/sap-ai-core/sap-ai-core-service-guide/models-and-scenarios-in-generative-ai-hub?locale=en-US&q=generative)). 

    Keep preset "latest" for model version.

    ![](images/33_genai_conf_step2.png)

6. You cannot provide input artifacts for this executable. Click "Next" --> "Review" and "Create".


### Create a Deployment

You can make LLM available for use by creating a virtual LLM deployment. You can do so once for each model and model version.

1. After having the configuration created , click on "Create Deployment" in your just created Configuration.

    ![](images/34_genai_createdeploy.png)

2. Scenario, Executable and Configuration is already pre-filled if you create your deployment from your configuration.

    Keep the "Standard" Duration. 
    
    Click "Review" and "Create"

    ![](images/35_genai_duration.png)

3. Wait until the "Current Status" switches from "UNKNOWN" over "PENDING" to "RUNNING". This will take a minute.

    ![](images/36_genai_status.png)

    After deployment you can switch to your Prompt Editor and try your LLM.

### Make a sample Prompt

1. Switch to "Generative AI Hub" --> "Prompt Editor".

2. Make a sample prompt. For example:

    ![](images/37_genai_sampleprompt.png)

    

For more samples, see next tutorial or access it directly [Prompt LLMs in the generative AI hub in SAP AI Core & Launchpad](https://developers.sap.com/tutorials/ai-core-generative-ai.html).