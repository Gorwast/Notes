Flowcharts are composed of **nodes** (geometric shapes) and **edges** (arrows or lines). The Mermaid code defines how nodes and edges are made and accommodates different arrow types, multi-directional arrows, and any linking to and from subgraphs.

```mermaid
---
title: Node
---
flowchart LR
    id
    id1["This is the text in the box ❤"]
    id2[fa:fa-ban Hola]
    id --- id1 === id2
```


```mermaid
flowchart TD
    Start --> Stop
```

```mermaid
---
title: Use LR for Left and Right orientations
---
flowchart LR
    Start --> Stop
```

Possible FlowChart orientations are:
- TB - Top to bottom
- TD - Top-down/ same as top to bottom
- BT - Bottom to top
- RL - Right to left
- LR - Left to right

## Node Shapes
```mermaid
flowchart TD
	square[Square text] --> roundEdges(Round Edges text)
	roundEdges --> stadiumShape([Stadium Shape text])
	stadiumShape --> Database[(Database Text)]
	Database --> circle((Circle Text))
	asymShape>Asymetric Text]
	asymShape --> rhombus{Rhombus Text}
	rhombus --> hexShape{{hexagon Text}}
	hexShape --> parallShape[/Parallelogram Text/]
	parallShape --> altParallShape[\Alt Parallelogram Text\]
	A[/Christmas\]
```




