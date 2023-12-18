## Lab 11 - Integrate Logic App with Threat Protection and XDR

## Lab scenario

The integration of a Logic App with Threat Protection involves configuring triggers and actions to receive alerts, while interaction with XDR solutions requires adding actions to exchange data, perform analyses, and trigger responses. Implementing conditional checks and logic within the Logic App allows for tailored handling of received threat information, ensuring effective responses and workflow execution before thorough testing and deployment to production environments. 

## Lab objectives
 In this lab, you will perform the following:
 - Task 1: Create a hunting query
 - Task 2: Create a NRT query rule
 - Task 3: Create a Search
 - Task 4: Explore Notebooks
 
## Estimated timing: 60 minutes

## Architecture Diagram

## Exersise 1: Integrate Logic App with Threat Protection and XDR

### Task 1: Create an Azure logic app

1. In the Azure portal, search for and select **Logic App** and, on the **Logic Apps** blade, select **+ Add** the select **Consumption**.

1. On the **Basics** tab of the **Logic App** blade, specify the following settings (leave others with their default values):

    | Setting | Value | 
    | --- | --- |
    | Subscription | the name of the Azure subscription you are using in this lab |
    | Resource group | select the existing resource group from drop down |
    | Logic App name | **logicapp1** | 
    | Select the location | select the location where resource group is deployed. |
    | Public | **workflow** |
    | Plan type | **Standard** |

1. Select **Review + create** and then select **Create**. 

### Task 2: Design Your Logic App Workflow

1. You'll enter the Logic App Designer interface. Here, you'll see a blank canvas to design your workflow.

1. Click on the "+ New step" button to add triggers and actions.

1. Configure triggers (e.g., HTTP request, Recurrence, etc.) that will start the Logic App workflow.

1. Add actions by selecting connectors and actions from the available services. Connectors can include services like Azure Security Center, Microsoft Defender for Endpoint, or any other relevant services related to your integration with Threat Protection and XDR.

1. Configure these actions to receive alerts or events from the Threat Protection service and interact with your XDR solution based on your integration requirements.

1. Set up logic, conditions, and response actions based on the received data and requirements.

1. After designing the Logic App workflow, click on the "Save" button in the Logic App Designer.

## Exersice 2: Trigger Configuration

### Task 1: Access Logic App Designer

1. Sign in to the Azure Portal at portal.azure.com.

1. Navigate to the Logic App you created or wish to configure the trigger for.

1. Click on the Logic App name to open the Logic App Designer.

### Task 2: Add a Trigger

1. Inside the Logic App Designer, you'll see a blank canvas. Click on the "+ Add" button to add a trigger.

1. In the search bar, type the name of the trigger you want to use. For example, "HTTP request" or "Recurrence" for a scheduled trigger.

1. Select the appropriate trigger from the available options. For instance, if you choose "When an HTTP request is received," select it to add this trigger to your Logic App workflow.

### Task 3: Configure the Trigger
1. After adding the trigger, you'll be prompted to configure it.
1. **For HTTP Request Trigger:** - If you selected the "When an HTTP request is received" trigger: - You'll get a URL (HTTP POST URL) that you can use to trigger this Logic App by sending an HTTP POST request to that URL. - You can set optional parameters and define the schema for the request that the trigger expects.
1. **For Recurrence Trigger:** - If you selected a scheduled trigger like Recurrence: - Set the frequency, interval, start time, and time zone for the trigger. - Configure recurrence settings such as daily, weekly, monthly, etc., based on your requirements.

1. Once you've configured the trigger settings according to your needs, click on the "Save" button in the Logic App Designer to save the changes.

## Exericise 3 :Add Actions for Threat Protection
### Task 1: Access Logic App Designer

1. Sign in to the Azure Portal at portal.azure.com.
1. Navigate to the Logic App you previously created or want to add actions for.
1. Click on the Logic App name to access the Logic App Designer.

### Task 2: Add Actions for Threat Protection
1. Inside the Logic App Designer, within your existing or newly created workflow, click on the step where you want to add actions related to Threat Protection.
1. Click on the "+ Add" button below the selected step to add a new action.
1. In the search bar, type the name of the service or connector related to Threat Protection that you want to integrate with. For instance, you might use services like "Azure Security Center" or "Microsoft Defender for Endpoint" for Threat Protection.
1. Select the relevant service from the available connectors.

### Task 3: Configure the Action
1. Once you've selected the connector/service for Threat Protection, you'll be prompted to configure the action.

  - Provide necessary credentials or permissions to connect to the Threat Protection service.
  - Choose the specific action you want to perform (e.g., retrieving alerts, getting details of a specific threat, triggering a response, etc.).
  - Configure settings such as filters, parameters, or any other required information to retrieve or interact with the Threat Protection data.

1. After configuring the action, click on the "Save" button within the Logic App Designer to save your changes.
1. Optionally, if feasible, trigger the Logic App or wait for the trigger event to occur to test the action you added for Threat Protection.
1. Monitor the Logic App runs to ensure that the action related to Threat Protection executes as expected, retrieves alerts, or performs the intended task.

### Task 5: Continue Building Workflow
1. If your Logic App workflow involves additional actions or logic based on the Threat Protection data received, continue adding necessary steps within the Logic App Designer to process, analyze, or respond to the retrieved Threat Protection information.

## Exercise 4: Integrate with XDR:
### Task 1: Access Logic App Designer
1. Sign in to the Azure Portal at portal.azure.com.
1. Navigate to the Logic App where you want to integrate with the XDR solution.
1. Click on the Logic App name to access the Logic App Designer.

### Task 2: Add Actions for XDR Integration
1. Inside the Logic App Designer, within your workflow, click on the step where you want to integrate with the XDR solution.
1. Click on the "+ Add" button below the selected step to add a new action.
1. In the search bar, type the name of the connector or service related to your XDR solution. If there's a specific connector available for your XDR solution, select it. Otherwise, you might use generic connectors like HTTP requests to interact with an API provided by your XDR solution.

### Task 3: Configure the Action for XDR Integration
1. Once you've selected the connector or service for the XDR solution, you'll be prompted to configure the action.
1. Provide the necessary credentials or API key to authenticate and connect to your XDR solution.
1. Choose the specific action you want to perform, such as pushing threat alerts, querying for information, triggering responses, etc.
1. Configure settings, parameters, or payloads required by the XDR solution's API to send or receive data effectively.
1. After configuring the action for XDR integration, click on the "Save" button within the Logic App Designer to save your changes.
1. If feasible, trigger the Logic App or wait for the trigger event to occur to test the action related to your XDR solution.
1. Monitor the Logic App runs to ensure that the action for XDR integration executes as expected, sends/receives data, or triggers the intended responses based on specific conditions.

### Task 5: Implement Logic and Response
1. Continue building your Logic App workflow to include further actions or conditions based on the data received from the XDR solution.

   - Implement necessary logic within the Logic App to handle and process the data retrieved from the XDR solution. This could involve 
   - conditional checks, data transformations, or other processes based on the received information.

## Review
In this lab, you have completed the following:


