# Service Graph

## Graph Zoom Tool
The graph zoom tool contains buttons that enable the user to zoom the graph in and out as well as fit the zoom to the current view. This tool may optionally contain a trigger for the graph legend as well as a graph layout selector.
![zoom tool on the service graph](img/zoom-tool-full.png)

### Zoom Tool Actions
![zoom tool](img/zoom-tool.png)
- **Zoom in:** Zooms the graph by a factor of 2 (e.g. 50% => 100%, 100% => 200%)
- **Zoom out:** Zooms the graph by a factor of .5 (e.g. 200% => 100%, 100% => 50%)
- **Zoom to fit:** Zooms the graph to fit the current viewport size
- **Legend:** Shows and hides the graph legend

#### Optional Actions
![zoom tool](img/zoom-tool-display-buttons.png)
- **Graph layout toggle:** The graph zoom tool could optionally include buttons to toggle the graph layout. This should only be done if all available graph layouts are able to be described by icons or some other extremely short identifier.

## Service Representation Colors
Nodes in the service graph are colored according to their health. Borders are 1px wide for unselected nodes and 3px for selected nodes. Graph edges are colored similarly, with 1px lines when unselected, and 3px lines when selected. There is no separate hover state for graph edges, but items not directly connected to the hovered edge should be blurred into the background.

### Healthy
![healthy nodes](img/node-status-default.png)
![healthy edges](img/edge-status-healthy.png)
- Grey Stroke: #8b8d8f (pf-black-500)
- White Fill: #ffffff (pf-white)
- Blue Stroke: #39a5dc (pf-blue-300)
- Blue Fill: #def3ff (pf-blue-50)
- Green Stroke: #3f9c35 (pf-green-400)

### Warning
![warning nodes](img/node-status-warning.png)
![warning edges](img/edge-status-warning.png)
- White Fill: #ffffff (pf-white)
- Orange Stroke: #ec7a08 (pf-orange)
- Orange Fill: #fdf2e5

### Error
![error nodes](img/node-status-error.png)
![error edges](img/edge-status-error.png)
- White Fill: #ffffff (pf-white)
- Red Stroke: #cc0000 (pf-red)
- Red Fill: #ffe6e6

### Idle
![idle edges](img/edge-status-idle.png)
- Grey Stroke: #8b8d8f (pf-black-500)

### Unused
![unused nodes](img/node-status-unused.png)
- Grey Stroke: #8b8d8f (pf-black-500)
- White Fill: #ffffff (pf-white)
- Blue Stroke: #39a5dc (pf-blue-300)
- Blue Fill: #def3ff (pf-blue-50)

### TCP Traffic
![TCP traffic edges](img/edge-status-tcp.png)
- Dark Blue Stroke: #004368 (pf-blue-600)

## Traffic Animation options

### Normal traffic
  ![possible traffic animation appearance](img/traffic-1.png)

  ![possible traffic animation appearance](img/traffic-2.png)

  ![possible traffic animation appearance](img/traffic-3.png)

### Failed request
  ![possible traffic animation appearance](img/traffic-4.png)

  ![possible traffic animation appearance](img/traffic-5.png)
