---
title: Coda
description: Documentation for the Coda node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
contentType: integration
---

# Coda

The Coda node allows you to automate work in Coda, and integrate Coda with other applications. n8n has built-in support for a wide range of Coda features, including creating, getting, and deleting controls, formulas, tables, and views.

On this page, you'll find a list of operations the Coda node supports and links to more resources.

!!! note "Credentials"
    Refer to [Coda credentials](/integrations/builtin/credentials/coda/) for guidance on setting up authentication. 

!!! note "Examples and templates"
    For usage examples and templates to help you get started, take a look at n8n's [Coda integrations](https://n8n.io/integrations/coda/){:target="_blank" .external-link} list.


## Basic Operations

* Control
    * Get a control
    * Get all controls
* Formula
    * Get a formula
    * Get all formulas
* Table
    * Create/Insert a row
    * Delete one or multiple rows
    * Get all columns
    * Get all the rows
    * Get a column
    * Get a row
    * Pushes a button
* View
    * Delete view row
    * Get a view
    * Get all views
    * Get all views columns
    * Get all views rows
    * Update row
    * Push view button

## Example Usage

This workflow allows you to insert data into a new row for a table in Coda. You can also find the [workflow](https://n8n.io/workflows/482) on the website. This example usage workflow would use the following three nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Set](/integrations/builtin/core-nodes/n8n-nodes-base.set/)
- [Coda]()

The final workflow should look like the following image.

![A workflow with the Coda node](/_images/integrations/builtin/app-nodes/coda/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Set node

1. Click on the *Add Value* button and select 'String' from the dropdown list.
2. Enter `Column 1`in the *Name* field.
3. Enter the value for the first column in the *Value* field.
4. Repeat the first three steps of all the columns that you have in your Coda table.

**Note:** Here, we've used the default table in Coda, which has three columns namely Column 1, Column 2, and Column 3. Please make sure that the column names in the *Name* field matches the names of the table columns in Coda.

### 3. Coda node

1. First of all, you'll have to enter credentials for the Coda node. You can find out how to do that [here](/integrations/builtin/credentials/coda/).
2. Select the name of your document from the *Doc* dropdown list.
3. Select the name of your table from the *Table* dropdown list.
4. Click on *Execute Node* to run the workflow.





