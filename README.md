# Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## 📌 Project Overview

This project demonstrates how **ServiceNow Flow Designer** can automate
a routine IT procurement process for standard laptop requests.

When a user requests a **Standard Laptop** through the Service Catalog
and the request reaches the required approval state, the configured flow
automatically creates a **Catalog Task** for the **Hardware** team with
standardized task details.

**Project Domain:** ServiceNow / IT Service Management\
**Platform:** ServiceNow\
**Module:** Flow Designer\
**Project Type:** Naan Mudhalvan Academic / Training Project

------------------------------------------------------------------------

## 🎯 Problem Statement

The standard laptop procurement process can involve manual task creation
and assignment, which may cause delays, manual overhead, or missed
configuration activities.

This project addresses that process by introducing Flow Designer
automation for the creation and assignment of the laptop configuration
task.

------------------------------------------------------------------------

## 🎯 Project Objective

The main objective is to automate the procurement and configuration
workflow for standard laptop requests.

The project aims to:

-   Reduce manual intervention in the procurement process.
-   Automatically create a Catalog Task after the required approval.
-   Assign the task to the **Hardware** group.
-   Maintain consistent task descriptions and field values.
-   Improve the efficiency and structure of IT procurement operations.

------------------------------------------------------------------------

## ⚙️ Workflow Design

The automation follows a trigger-and-action pattern:

``` text
Service Catalog Request
        ↓
Requested Item Record
        ↓
Required Approval
        ↓
Create Catalog Task
        ↓
Populate Task Details
        ↓
Assign to Hardware
        ↓
Laptop Configuration Task
```

### Flow Configuration

  Configuration       Value
  ------------------- ------------------------------
  Trigger             Service Catalog
  Request Item        Requested Item Record
  Action              Create Catalog Task
  Table               Catalog Task
  Short Description   Laptop need to be Configured
  Description         Laptop need to be Configured
  Assignment Group    Hardware
  Approval            Approved

------------------------------------------------------------------------

## 🛠️ Implementation

### Milestone 1 -- Flow Creation

A Flow Designer flow named **Standard laptop tasks** was created.

The flow uses:

-   **Service Catalog** as the trigger.
-   **Create Catalog Task** as the main action.
-   **Requested Item Record** as the request item.
-   **Hardware** as the assignment group.
-   **Approved** as the approval value.
-   **Laptop need to be Configured** as the short description and
    description.

After configuration, the flow was saved and activated.

### Milestone 2 -- Flow Assignment

The **Standard Laptop** service catalog item was configured to use the
newly created **Standard Laptop Task** flow under the **Process Engine**
section.

This connects the Standard Laptop catalog item with the automation flow.

### Milestone 3 -- Request, Approval and Catalog Task

The Standard Laptop request was placed through:

**Service Catalog → Hardware → Standard Laptop → Order Now**

The request record was then opened, the approval step was completed, and
the Requested Item was accessed.

Finally, the **Catalog Tasks** section was opened to view the generated
task record.

------------------------------------------------------------------------

## 📸 Project Evidence

The project folder contains the supporting screenshots and PDF documents
for the implementation milestones.

The main implementation evidence demonstrates:

1.  Standard Laptop catalog item configuration.
2.  Flow Designer / Workflow Studio configuration.
3.  Generated Catalog Task record.

The Catalog Task evidence shows the resulting task with details such as
request information, approval status, state, and the laptop
configuration description.

------------------------------------------------------------------------

## ✅ Expected Result

After the flow is activated and the Standard Laptop request reaches the
configured approval state, a **Catalog Task** is automatically created.

The resulting task contains:

-   **Short Description:** Laptop need to be Configured
-   **Description:** Laptop need to be Configured
-   **Assignment Group:** Hardware
-   **Approval:** Approved

This provides a consistent and automated hand-off to the Hardware team.

------------------------------------------------------------------------

## 🌟 Advantages

-   Automation of repetitive Catalog Task creation.
-   Faster hand-off to the Hardware team.
-   Consistent task descriptions and field values.
-   Reduced risk of manual omission or incorrect assignment.
-   Better visibility of configuration work through ServiceNow task
    records.
-   Improved utilization of IT support resources.
-   More standardized laptop provisioning workflow.

------------------------------------------------------------------------

## 💡 Applications

This automation approach can be applied to:

-   Standard laptop and desktop procurement.
-   Employee onboarding and device provisioning.
-   IT asset preparation and configuration.
-   Hardware replacement and refresh processes.
-   Service Catalog requests requiring specialized team tasks.

------------------------------------------------------------------------

## 🚀 Future Enhancements

Possible improvements include:

-   Automated notifications to the requester and Hardware team.
-   Different conditions for standard, high-performance, and
    special-purpose laptop requests.
-   Automatic population of model, asset type, location, and delivery
    details.
-   Additional approval checks and exception handling.
-   Inventory availability checks before creating configuration tasks.
-   Reports and dashboards for task completion time and procurement
    efficiency.

------------------------------------------------------------------------

## 📂 Project Structure

A suggested GitHub repository structure is:

``` text
Streamlining-IT-Procurement/
│
├── README.md
│
├── PDFs/
│   ├── Project_Report.pdf
│   ├── Milestone_2.pdf
│   └── Milestone_3.pdf
│
└── Screenshots/
    ├── Flow_Designer.png
    ├── Standard_Laptop_Process_Engine.png
    └── Catalog_Task.png
```

> Rename the PDF and screenshot files according to the actual filenames
> in your project folder.

------------------------------------------------------------------------

## 🏁 Conclusion

The **Streamlining IT Procurement: Automating Standard Laptop Orders
with Flow Designer** project demonstrates a practical use of ServiceNow
Flow Designer for automating an IT procurement activity.

By using a **Service Catalog trigger** and **Create Catalog Task**
action, the workflow can consistently create and assign a Hardware task
with the required information. This reduces repetitive manual work,
improves task hand-off, and supports a more structured laptop
configuration process.

The project also provides a foundation for further automation such as
notifications, inventory validation, approvals, exception handling, and
performance reporting.

------------------------------------------------------------------------

## 📚 Project Documentation

The repository includes the project documentation, milestone PDFs, and
implementation screenshots used as supporting evidence for the
ServiceNow automation project.
