# MID Server Setup

## Overview
The MID Server acts as a secure communication bridge between ServiceNow and on-premise systems. This guide outlines the steps for installation and configuration.

## Steps
1. Download the MID Server installer from ServiceNow.
2. Run the installer and follow the prompts:
   - Provide the instance URL and credentials.
   - Select the target installation folder.
3. Verify the MID Server status in ServiceNow:
   - Navigate to **MID Server > Servers** and ensure it is online.
4. Assign credentials for Discovery in **MID Server > Credentials**.
5. Run a connectivity test to validate the setup.

## Best Practices
- Use separate MID Servers for different environments (e.g., Dev, Prod).
- Regularly monitor MID Server health and logs.
