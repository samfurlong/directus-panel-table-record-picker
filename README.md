# Directus Panel: Table Record Picker

A Directus panel extension that displays data in a table format and allows users to select a record, storing the selected value in a dashboard variable for use in other panels.

## Features

- **Table Display**: Shows data from any collection in a clean table format
- **Record Selection**: Click to select any record from the table
- **Variable Storage**: Stores the selected record's value in a dashboard variable
- **Configurable Fields**: Choose which fields to display in the table
- **Filtering & Sorting**: Apply filters and sort by any field
- **Responsive Design**: Adapts to different panel sizes

## Installation

1. Download or clone this extension
2. Place it in your Directus `extensions` folder
3. Restart your Directus instance
4. The panel will be available in your dashboard panel options

## Configuration Options

### Required Settings

- **Collection**: Select the collection to display data from
- **Variable Name**: Name of the dashboard variable to store the selected value
- **Value Field**: Which field's value to store when a record is selected
- **Fields**: Choose which fields to display in the table columns

### Optional Settings

- **Sort Field**: Field to sort the table by (defaults to primary key)
- **Sort Direction**: Ascending or descending sort order
- **Filter**: Apply filters to limit which records are shown
- **Limit**: Maximum number of records to display (default: 10)

## Usage

1. Add the "Table View Record Picker" panel to your dashboard
2. Configure the panel settings:
   - Select a collection
   - Set a variable name (e.g., `selected_user`)
   - Choose which field value to store (e.g., `id`, `name`)
   - Select which fields to display in the table
3. Save the panel configuration
4. Click on any row in the table to select that record
5. The selected value will be stored in the specified dashboard variable
6. Other panels can now use this variable (e.g., `{{ selected_user }}`)

## Example Use Cases

- **User Selection**: Display a list of users and select one for detailed views
- **Product Picker**: Show products in a table and select for inventory management
- **Order Dashboard**: List orders and select one to show related data
- **Content Management**: Display articles/pages and select for editing workflows

## Technical Details

- **Type**: Panel Extension
- **Minimum Directus Version**: 11.5.1

- **Framework**: Vue 3 + TypeScript
- **Variable Scope**: Dashboard-level variables

## Development

```bash
# Install dependencies
npm install

# Build for development (with watch mode)
npm run dev

# Build for production
npm run build

# Validate extension
npm run validate

# Link to local Directus instance
npm run link
```

## License

MIT License

## Author

Sam Furlong ([@samfurlong](https://github.com/samfurlong))

## Support

If you encounter any issues or have feature requests, please create an issue in the repository. 