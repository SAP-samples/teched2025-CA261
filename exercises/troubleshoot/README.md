## Troubleshooting Guide


Sl no | Troubleshooting Guide
---------|----------
 1 | [How to restore files and tasks to a previous step](#1-how-to-restore-files-and-tasks-to-a-previous-step)
 2 | [MCP server connection failure](#2-mcp-server-connection-failure)
 3 | [CDS Compile error](#3-cds-compilation-error) 
 4 | [How to reset and start from scratch](#4-how-to-reset-and-start-from-scratch)
 5 | [Model Claude-4.5 is Not Responding](#5-model-anthropic-claude-45-sonnet-is-not-responding)
 6 | [VS Code Terminal Timeout Issues](#6-vscode-terminal-timeout-issues)
 7 | [Cline Panel is Not Visible](#7-cline-panel-is-not-visible)


---

### 1. How to restore files and tasks to a previous step.

   ![restore task](./images/restore-task.png)

---

### 2. MCP server connection failure:
   In the Cline panel, if you notice that no response is received after Cline uses a tool from the MCP server, expand the API Request section to check for any errors related to the MCP tool.

   ![mcp server connection](./images/mcp-tool-failure.png)

   - Click on `Manage MCP Servers`
   - Click on `Retry Connection`.
   - Verify mcp servers are connected again.

   ![mcp server refresh](./images/mcp-server-refresh.png)

---

### 3. CDS Compilation error.
   - If you notice cds compilation error on console. copy and paste error message in to the task input.

   ```
   [ERROR] srv/travel-service.cds:5:10: Composition in draft-enabled entity can't lead to another entity with “@odata.draft.enabled” (in entity:“TravelService.Travel”/element:“to_Booking”)
   ```

   - Press `Enter`
   - Cline removes `@odata.draft.enabled` annotation applied on booking entity from cds service.

---

### 4. How to reset and start from scratch.
   - Close the current task.

   ![close task](./images/close-task.png)

   - In the Explorer, right-click the project folder and select delete.

   ![delete project](./images/delete-project.png)

   - Open the Cline panel. Click on `view all history`

   ![view history](./images/view-history.png)

   - Click on `Delete All History` 

   ![delete history](./images/delete-history.png)

   - In the dialog, click `Delete Everything`.

   ![delete everything](./images/delete-everything.png)

   - Then, in the Cline settings panel (top right corner), click `Done`.

---

### 5. Model `anthropic-claude-4.5-sonnet` is Not Responding

   ![model error](./images/model-error.png)

   - If the Claude 4.5 model is unresponsive or not generating results and throws above error. Switch model to the `anthropic-claude-4.0-sonnet` model in the Cline panel.
   - To do this, open the Cline panel, select **Model**, and choose `anthropic-claude-4.0-sonnet`.
   - Retry your task.

   - If the issue still exists, then you can close the current Cline task.

   ![close task](./images/close-task.png)

   - Start a new task and re-enter the prompt from excercise to continue.

---

### 6. Vscode Terminal Timeout Issues

- If the status in Cline remains pending and commands (such as `npm install`) are not executed in the VS Code terminal, toggle between **Act** and **Plan** mode, then click `Resume Task`.

  ![terminal](./images/terminal-pending.png)

   Solution:

  ![resume task](./images/task-resume.png)

   - If the issue still exists, then you can close the current Cline task.
   - Reopen the same task again.
   - Resume from where it left off.

   ![close task](./images/close-task.png)

---

### 7. Cline Panel is Not Visible

- If the Cline panel is not visible in VS Code:
  - Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac) to open the Command Palette.
  - Type `View: Show Cline` and press Enter.
  - The Cline panel will appear in the sidebar.

  ![command palette](./images/command-palette-cline.png)

---

   
