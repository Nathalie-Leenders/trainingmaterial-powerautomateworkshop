# Exercise 7: Combining RPA and Cloud Flows

## Objective
Learn how to call a Power Automate cloud flow from a desktop flow and vice versa.

## Prerequisites
- Power Automate Desktop installed
- Access to Power Automate (cloud)
- Basic understanding of creating flows

## Steps

### Part 1: Call a Cloud Flow from a Desktop Flow

1. **Create a Cloud Flow:**
    - Go to Power Automate.
    - Create a new cloud flow.
    - Add a trigger (e.g., "When an HTTP request is received").
    - Add actions as needed.
    - Save the flow and copy the HTTP POST URL.

2. **Create a Desktop Flow:**
    - Open Power Automate Desktop.
    - Create a new desktop flow.
    - Add an action to call the cloud flow using the HTTP POST URL.
      - Use the "Invoke Web Service" action.
      - Set the method to POST.
      - Paste the copied URL.
    - Save and run the desktop flow.

### Part 2: Call a Desktop Flow from a Cloud Flow

1. **Create a Desktop Flow:**
    - Open Power Automate Desktop.
    - Create a new desktop flow.
    - Save the flow.

2. **Create a Cloud Flow:**
    - Go to Power Automate.
    - Create a new cloud flow.
    - Add a trigger (e.g., "Manually trigger a flow").
    - Add an action to call the desktop flow.
      - Use the "Run a flow built with Power Automate Desktop" action.
      - Select the desktop flow you created.
    - Save and run the cloud flow.

## Conclusion
By completing this exercise, you have learned how to integrate Power Automate cloud flows with desktop flows, enabling seamless automation across different environments.
