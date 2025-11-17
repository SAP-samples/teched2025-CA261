# CA261 | Create great UX with AI, SAP Design System, SAP Fiori elements, and SAPUI5

## Description

This repository contains the material for the SAP TechEd 2025 session [CA261 | Create great UX with AI, SAP Design System, SAP Fiori elements, and SAPUI5](https://www.sap.com/events/teched/berlin/flow/sap/te25/catalog-inperson/page/catalog/session/1749126322451001Fcbi).  

***

## Overview

In this hands-on tutorial you will work through a set of exercises that highlight the benefits and capabilities of the **SAP Design System**, the **Figma** design tool, and the **MCP servers developed by SAP and Figma** to create and modify SAP Fiori applications with the help of AI coding assistants. 

You will gain comprehensive knowledge of AI assisted full-stack development, and learn how to use Figma and the SAP Design System to kickstart your SAP Fiori elements application development.

## Using AI during App Development

We are using Cline as AI client within VSCode and Anthropic claude-4.5-sonnet LLM (Large Language Model) throughout the exercises. When developing SAP Fiori applications with LLMs, you may encounter situations where a prompt is not executed as intended, or technical errors occur when calling MCP server tools. Knowing how to approach these issues systematically can save time and prevent disruption. Cline and the choosen LLM are powerful assistants for problem resolution.

### General steps in case of issues:

[Detailed steps and examples of resolving common issues](./exercises/troubleshoot/)

1. Verify connectivity:
    - Check if your machine has network access.
    - Confirm that the MCP server is up and running.

2. Approach errors systematically
    - Pause before panicking
        - Use natural pauses when the client asks for approval to inspect the current results and chat history.    
        - Stop execution with the "Cancel" button. You can always proceed from there with a new prompt
    - Identify the source: Check if the issue is:
        - CDS compiler error
        - SQLite/database error
        - Console/browser runtime error

3. Using the LLM to solve an issue
    - The LLM occasionally makes mistakes, or forgets required steps leading to error situations
    - But the LLM can read the terminal output and react to API reponses, and correct error visible there
    - Other issues, like from browser console output, can be resolved by copy-pasting the full error message into the chat and ask for a fix in a prompt
    - LLM works best when exact messages are provided rather than manual descriptions.

4. Use Restore Points if Needed
    - If a solution strategy does not work, you can always restore the files and chat to a previous checkpoint using Cline’s restore functionality.

5. Don’t be afraid to retry an exercise or step after restoring to a checkpoint.

## Exercises

Begin your exercises here. At the end of each section, there is a link to continue to the next section.

- [Exercise 1 - Open the Figma Design file in your Figma client](./exercises/ex1.0/)
  - [Exercise 1.1 - Adjust the buttons in the object page header](./exercises/ex1.1/)
  - [Exercise 1.2 - Add a form item in the object page](./exercises/ex1.2/)
  - [Exercise 1.3 - Edit the new form item in the object page](./exercises/ex1.3/)
  - [Exercise 1.4 - Export your designs](./exercises/ex1.4/)
  - [Exercise 1.5 - Enable your MCP Server in Figma](./exercises/ex1.5/)

- [Setup Visual Studio Code Development Environment](./exercises/ex1.6/)

- [Exercise 2 - Create fiori app based on figma design](./exercises/ex2.0/)
  - [Exercise 2.1 Enable automatic data loading in List Report](./exercises/ex2.1/)
  - [Exercise 2.2 Add table actions from design to list report table](./exercises/ex2.2/)
  - [Exercise 2.3 Apply business logic for action accept travel](./exercises/ex2.3/)
  - [Exercise 2.4 Configure filter travel status as valuehelp and display it as dropdown](./exercises/ex2.4/)
  - [Exercise 2.5 Apply criticality to travel status column](./exercises/ex2.5/)

- [Exercise 3 - Modify travel object page based on figma design](./exercises/ex3.0/)
  - [Exercise 3.1 Adjust Object Page Title and Description](./exercises/ex3.1/)
  - [Exercise 3.2 Set Label for Object page sub sections](./exercises/ex3.2/)
  - [Exercise 3.3 Rearrange fields in General information section as per design](./exercises/ex3.3/)
  - [Exercise 3.4 Set Criticality for status field](./exercises/ex3.4/)
  - [Exercise 3.5 Add Custom Section with RichTextEditor Building Block](./exercises/ex3.5/)

- [Exercise 4 - Create booking object page based on figma design](./exercises/ex4/)

- [Exercise 5 - Add Analytical chart to list report page](./exercises/ex5/)
