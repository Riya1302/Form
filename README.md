# Form
# Custom Form Builder

This is a Custom Form Builder application built with HTML, CSS, and JavaScript. It allows users to dynamically create and manage form fields through a user-friendly interface with drag-and-drop functionality.


## Features

- **Drag-and-Drop Form Fields**: Use Dragula library for seamless drag-and-drop functionality.
- **Dynamic Form Field Addition**: Add input, select, and textarea fields dynamically.
- **Editable Labels**: Labels for form fields are editable directly in the UI.
- **Form Field Removal**: Easily remove form fields with a delete button.
- **Save Form Data**: Save the current form state and log it as JSON.

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
Open the index.html file in your web browser to run the application.
Usage
Adding Form Fields: Click on the tool items (Input, Select, Textarea) in the sidebar to add new fields to the form.
Editing Labels: Click on the label text to edit it.
Removing Form Fields: Click the delete (🗑️) button next to each form field to remove it.
Saving Form Data: Click the "Save" button in the navbar to log the form data as JSON in the console.


# Code Explanation

## HTML Structure

The HTML is structured into three main parts: the header (navbar), the tools section (tools), and the form area (form-area). Each part is styled with CSS to provide a clean layout.

## CSS Styling

The CSS provides styling for various elements:
body: Sets up the font and layout.
navbar: Styles the header with a title and save button.
tools: Styles the sidebar containing form element tools.
tool-item: Styles each tool item in the sidebar.
form-area: Styles the main area where the form elements are displayed.
form-wrapper: Styles the container holding the form elements.
form-group: Styles each form element group, including labels, inputs, selects, textareas, and buttons.


## JavaScript Functionality

Drag-and-Drop Initialization: The dragula library is used to enable drag-and-drop functionality for reordering form elements.
saveForm Function: Collects data from the form elements and logs it as JSON in the console. It gathers information such as id, type, label, placeholder, and options for each form element.
addField Function: Adds a new form element (input, select, or textarea) to the form container with editable labels and placeholders.
removeField Function: Removes a form element from the form container.
generateUniqueId Function: Generates a unique ID for each new form element using a random string generator.
