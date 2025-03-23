# VAG - Vanquish Allegiance Glancer

VAG is a lightweight, browser-based tool for viewing and analyzing Asheron's Call allegiance hierarchies. It provides a clean, visual representation of allegiance structures with the ability to easily identify online and offline members.

## Purpose

VAG takes the `scanresult.json` output from [AllegianceSkimmer](https://github.com/amoeba/AllegianceSkimmer) (a Decal plugin for Asheron's Call) and presents the allegiance data in a cleaner, more user-friendly format. While AllegianceSkimmer handles the collection of allegiance data, VAG focuses on visualization and analysis of that data.

## Features

- **Hierarchical Tree View**: Displays the complete allegiance structure in a clean, vertical tree layout
- **Online/Offline Tracking**: Clearly shows which members are online with color-coding and status indicators
- **Statistics**: Provides key metrics including total members, online percentage, and more
- **Player Search**: Quickly find specific members with the built-in search function
- **Online Players List**: View a simple alphabetical list of all online members
- **Collapsible Nodes**: Expand or collapse branches to focus on specific parts of the hierarchy
- **Responsive Design**: Works on desktop and mobile devices
- **No Installation Required**: Run directly in your browser without any dependencies

## How to Use

1. **Get the scanresult.json file**:
   - Use [AllegianceSkimmer](https://github.com/amoeba/AllegianceSkimmer) to scan your allegiance in Asheron's Call
   - Save the generated `scanresult.json` file

2. **Download VAG**:
   - Save `VAG.html` to your computer

3. **Open the Viewer**:
   - Double-click on `VAG.html` to open it in your web browser
   - Click the "Choose File" button to select your `scanresult.json` file

4. **View Your Allegiance**:
   - The hierarchy will automatically load and display
   - Use the buttons to expand/collapse branches, filter for online players, etc.
   - Use the search box to find specific members

## Controls

- **Expand All**: Expands all branches in the tree view
- **Collapse All**: Collapses all branches in the tree view
- **List Online Players**: Shows a flat, alphabetical list of all online members
- **Show All**: Returns to the full hierarchy view

## Requirements

- Any modern web browser (Chrome, Firefox, Edge, Safari)
- A valid `scanresult.json` file from AllegianceSkimmer

## JSON Format

The allegiance data from AllegianceSkimmer should be in the following format:

```json
{
  "name": "Monarchy Owner",
  "is_online": true,
  "children": [
    {
      "name": "Vassal 1",
      "is_online": false,
      "children": []
    },
    {
      "name": "Vassal 2",
      "is_online": true,
      "children": [
        {
          "name": "Sub-Vassal",
          "is_online": false,
          "children": []
        }
      ]
    }
  ]
}
```

## Privacy & Security

This tool runs entirely in your browser. No data is sent to any servers, and your allegiance data never leaves your computer.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details. 