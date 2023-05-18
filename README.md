We welcome contributions to this open-source project. 

If you'd like to contribute to the main Siteglide Theme Module, the master branch is protected, so for new contributions, please create a new branch and create a pull request containing the changes you'd like to make. Don't forget to also update the changelog with what you have changed- list your new version number as "pending".

If you'd like to build your own version of the module entirely, please create a fork and register as your own Module in the Siteglide Marketplace.

## Changelog

### 1.4.0

Added dynamic API key fetching for textarea layout components. Requires SiteBuilder 4.7.2
### 1.3.0

- Improvements to forms
  - All form components to use the `{{field_id}}` (plus any appropriate suffix) for their ID, instead of name (same for label for attributes). This should simplify any JS or CSS referencing it.
  - All required fields will have an asterisk " *" added after their labels by default. This can be changed in components.
  - All inputs will be given data-attributes containing the text of their human-readable label `data-sg-validation-label` and the main field ID for their field `data-sg-validation-id` (note this may be different from the ID of the element if there are multiple form elements responsible for controlling a field, e.g. checkboxes). These can be useful when writing custom validation rules.
  - If the error message from Siteglide validation references a field by ID, we will change the error message to be more human-friendly. The default is a generic message asking the user to complete missing fields, but a commented out alternative allows you to print the human-readable name of the first missing field. Likewise, we've added a more human-friendly error message when a captcha fails. These messages can be edited in the form layout JS.
  - Improvements for Date, File and Image fields when marked as required.
  - Improvements for rich-text textarea type fields when marked as required.
  - Added minimum value to date fields so they do not add a date which is out of range of Siteglide's date field. Siteglide dates must be within the unix epoch.
  - Improved animation transition on form progress bars.

### 1.2.0

- Improvements to forms, adding easier paramter for setting custom redirects.

### 1.1.3

- Improvements to forms, adding RTE support and fixes for date fields

### 1.1.0

- Added support for Sliders Module (you will need to update to version 4.4.0 of SiteBuilder to use this.)

### 1.0.2

- Updated SCSS files to use /dist and /src folders.
- Improved Header Layout responsiveness
- Added LinkedIn to the Footer Layout

### 1.0.1

- Initial Release
