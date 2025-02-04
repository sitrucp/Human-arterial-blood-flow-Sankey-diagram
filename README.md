# Human Arterial Blood Flow Sankey Diagram

This project visualizes the human arterial vessel flow hierarchy starting from the heart to the capillaries using a D3.js Sankey chart. Blood vessel data is sourced from Wikipedia and transformed into two columns, one for the parent vessel and another for the child vessel.

Human arterial vessel flow hierarchy starting from heart to capilliaries generated with D3.js Sankey chart.
Blood vessel data from Wikipedia and transformed into two columns, one for parent vessel, another for child vessel.

More details about this chart are on the blog post at:

[http://009co.com/?p=1]

## Features
- **Interactive Visualization:** Hover over any link to highlight the link and see the artery-source names and relative flow values.
- **Node Interaction:** Click on any node (e.g., artery name) to highlight the upstream and downstream links. Click again to remove the highlighting (or refresh the page). Multiple nodes can be clicked simultaneously.
- **Drag and Drop:** Nodes (e.g., artery names) can be dragged along the vertical axis to reposition them for better readability.

## Demo
More details about this chart can be found on the blog post [here](http://009co.com/?p=1).

## Usage

To run this project locally:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/sitrucp/Human-arterial-blood-flow-Sankey-diagram.git
    cd Human-arterial-blood-flow-Sankey-diagram
    ```

2. **Open the `index.html` file:**
    Simply open the `index.html` file in your preferred web browser. No additional server setup is required.

## Data
The data for this project is stored in a CSV file (`data/blood_sankey.csv`). The CSV file contains the following columns:
- `source`: The parent artery.
- `target`: The child artery.
- `value`: The relative volume of blood flow.

### Data Source
The arterial data is sourced from Wikipedia and represents a hierarchical structure of human arterial blood vessels. The data was transformed to fit the requirements of a Sankey diagram, which illustrates the flow of blood from the heart through various arteries to the capillaries.

## Code Overview
- **index.html:** The main HTML file that sets up the page and includes the D3.js scripts.
- **d3/d3.v3.js:** The D3.js library used for creating the Sankey diagram.
- **js/sankey.js:** Custom JavaScript for setting up and rendering the Sankey diagram.

### Key JavaScript Functions:
- **dragmove(d):** Handles the dragging of nodes to reposition them.
- **highlight_node_links(node, i):** Highlights the links connected to a clicked node.
- **highlight_link(id, opacity):** Adjusts the opacity of a link to highlight or de-highlight it.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.# Human-arterial-blood-flow-Sankey-diagram


