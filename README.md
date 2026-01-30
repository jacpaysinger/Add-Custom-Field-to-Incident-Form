# Adding a Custom Field to an Incident Form

## Overview
This repository demonstrates how to add an existing custom field to a core Incident form using Form Builder in ServiceNow. The focus is on modifying the Default view of the Incident form and ensuring the field is displayed correctly for end users.

This project builds on a previously created custom field and simulates a common administrative task performed by system administrators during form configuration.

## Use Case
A system administrator needs to enhance the Incident form by adding a previously created custom field so that analysts can capture additional information during Incident creation and review.

This project simulates updating the Incident form layout to support improved data visibility while maintaining consistency with existing form structure.

## Features
- Form configuration using Form Builder
- Use of the Default Incident form view
- Placement of a custom True/False field
- Validation of form layout changes
- Reloading and verifying form updates

## Technologies Used
- ServiceNow Platform
- Incident Management
- Form Builder
- IT Service Management (ITSM)

## Implementation Walkthrough

### Objective
Add the Pilot custom field to the Incident form and verify it displays correctly in the Default view.

### Step 1: Navigate to the Incident Table
The Incident list was accessed using the application navigator.

Navigation path:
- All > Incident > Open

The list was confirmed to be using the **Default** view.

### Step 2: Open a New Incident Record
A new Incident record was created by selecting **New** from the Incident list.

This opened the Incident form in a new browser tab.

### Step 3: Open Form Builder
The form header was right-clicked and **Configure > Form Builder** was selected.

A notification appeared indicating the form was in a different application scope.  
The option to edit in the original scope was **not** selected.

### Step 4: Confirm the Default View
Within Form Builder, the view selector was reviewed to confirm the form was being edited in the **Default** view.

This ensures the field will be visible in the standard Incident experience.

### Step 5: Locate the Pilot Field
Under the Description section of the form layout, the **Pilot** field created in the previous lab was located in the available components.

### Step 6: Add the Pilot Field to the Form
The **Pilot** field was selected and dragged directly below the **Configuration item** field.

This placement aligns the field logically with related configuration data.

<img width="1915" height="965" alt="Screen Shot 2026-01-29 at 7 18 32 PM" src="https://github.com/user-attachments/assets/032b8edc-5a0d-447b-989f-bdc4d1e42980" />

### Step 7: Save Form Changes
The form layout changes were saved using the **Save** option in Form Builder.

### Step 8: Reload the Incident Form
The browser tab containing the Incident record was revisited.

Using the Additional actions menu (or by right-clicking the form header), **Reload form** was selected to refresh the layout.

### Step 9: Verify Field Placement
The Incident form was reviewed to confirm that the **Pilot** field displays correctly below the Configuration item field.

The field was verified as a checkbox and visible in the Default view.

<img width="1915" height="527" alt="Screen Shot 2026-01-29 at 7 20 45 PM" src="https://github.com/user-attachments/assets/7c808dee-f9b3-4544-ad21-20e66e556079" />

## Lessons Learned
- Form Builder allows controlled customization of core forms
- Editing the correct form view is critical for visibility
- Custom fields must be manually added to forms after creation
- Reloading the form is required to reflect layout changes
- Thoughtful field placement improves usability for analysts
