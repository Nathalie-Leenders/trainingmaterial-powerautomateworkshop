# Exercise 3.1: Calling a Power Automate Flow from a Bot with Copilot Studio

To be tested and added onto

## Objective

Learn how to call a Power Automate flow from a bot using actions and plugins in Copilot Studio.

## Prerequisites

- Access to Copilot Studio
- A Power Automate account
- Basic knowledge of creating flows in Power Automate

## Steps

### Step 1: Create a Power Automate Flow

1. Log in to Power Automate.
2. Click on **Create** and select **Automated flow**.
3. Name your flow and choose a trigger (e.g., **When an HTTP request is received**).
4. Add the necessary actions to your flow.
5. Save and test your flow.

### Step 2: Set Up Copilot Studio

1. Open Copilot Studio.
2. Create a new bot or open an existing one.
3. Navigate to the **Actions** tab.

### Step 3: Add a New Action

1. Click on **New Action**.
2. Name your action (e.g., `CallPowerAutomateFlow`).
3. In the **Action Type** dropdown, select **HTTP Request**.
4. Enter the URL of your Power Automate flow's HTTP trigger.
5. Configure the request method and headers as needed.
6. Save the action.

### Step 4: Integrate the Action into Your Bot

1. Go to the **Plugins** tab.
2. Create a new plugin or edit an existing one.
3. Add the `CallPowerAutomateFlow` action to the plugin.
4. Configure the plugin to call the action when a specific event occurs (e.g., when a user sends a message).

### Step 5: Test Your Bot

1. Deploy your bot.
2. Interact with your bot to trigger the action.
3. Verify that the Power Automate flow is called and performs the expected actions.

## Conclusion

You have successfully integrated a Power Automate flow with a bot using Copilot Studio. This allows you to automate tasks and enhance your bot's capabilities.

## Additional Resources

- [Power Automate Documentation](https://docs.microsoft.com/en-us/power-automate/)
- [Copilot Studio Documentation](https://docs.microsoft.com/en-us/copilot-studio/)
