# Due Date Tracker LWC

A Salesforce Lightning Web Component (LWC) to display due dates on record pages, the Due Date Tracker simplifies tracking deadlines directly within your Salesforce org.

![Due Date Tracker Screenshot](https://github.com/thedhanawada/SFDC-Due-Date-Tracker/assets/13751641/f65491b7-4e5b-478e-8805-138abf762670)

*Screenshot generated by [SuperbShot](https://superbshot.dev).*

## Installation

Install this package directly into your Salesforce org using this link: [DueDateTrackerPackage Installation](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tQE0000003Flh).

For manual installation, deploy the LWC and associated Apex class using your preferred Salesforce deployment tool.

## Features

- Dynamically fetches record data.
- Calculates remaining or elapsed time relative to due dates.
- Applies conditional styling to display status messages.

## Configuration

To configure the Due Date Tracker:

1. Add the component to a record page in Lightning App Builder.
2. Set the component properties:

   | Property                | Description                            |
   | ----------------------- | -------------------------------------- |
   | `Object Name`           | API name of the Salesforce object.     |
   | `Field to Compare`      | API name of the reference date field.  |
   | `Comparison Date Field` | API name of the due date field.        |

   **Example**:

   - Object Name: `Campaign`
   - Field to Compare: `startDate`
   - Comparison Date Field: `endDate`

## Usage

After configuration, the component will automatically display due date statuses on the record page.

## Customization

Style the component using SLDS classes or custom CSS by editing the `recordDue.css` file.

## Components

Included files:

- `recordDue.js` - Controller logic.
- `recordDue.html` - UI template.
- `recordDue.css` - Style definitions.
- `recordDue.xml` - Metadata for the component.

## Apex

`RecordDataService` is the Apex class that retrieves data for the LWC.

## Testing

Comprehensive test classes ensure reliable operation and deployment readiness. Confirm test coverage before deploying.

## Support

For issues, raise a ticket in this repository's [Issues section](https://github.com/thedhanawada/SFDC-Due-Date-Tracker/issues).

## Notes

Verify that the field API names used in the component match those in your Salesforce org configuration.
