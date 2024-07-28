# Hextiles

Hex grid geomorph dungeon tiles for roleplaying games.

## Introduction

Geomorphs are map segments that can be arranged in multiple ways to create a larger, coherent map.

These hex-based geomorphs are based on hexes and half-hexes with a 25mm hex size (from centre to centre).

### Base tiles

The [base tiles](base-tiles) are 4 hexes in size (100mm from centre to centre), consisting of 13 full hexes and 6 half-hexes. This is enough for a 3x3 room, a short segment of corridor, or a segement of a larger room.

A half-hex base tile is 2 hexes high and consists of 5 full hexes and 6 half-hexes.

### Tile groups

The base geomorphs can then be grouped into larger [tile groups](tile-groups), such as a long corridor, a large room, or a layout with a cluster of small rooms/corridors.

Tile groups up to 2 base tiles high and three base tiles wide fit nicely on a printed A4 landscape page at 200mm high and 289mm wide.

This configuration consists of 5 full base tiles and 2 half-tiles. It is 8 hexes high and 12 hexes on the diagonal.

You can easily join two large tile groups together along the flat side, or combine them with other tile groups or individual base tiles.

Including the half-tiles in the system allows for efficient placement of corridors running across the hexes (a lot of construction uses right angles).

## Tools

[Inkscape](https://inkscape.org/) is used to create and manage the vector-based tiles.

## Instructions

### Creating a base tile

* Use `hex-master-1.svg` to turn on or off the relevant elements (walls, etc) that make up the tile.
* When you have what you want, make sure no layers are locked (so they can be selected), and select all the elements on the page.
* Use the export tool to export the Document (not Page), making sure that Export Selected only is ticked.
* This will trim items that are not display (not selected) from the export, keeping it simple.

Corridor connections between base tiles use the centre hex of each face, for consistent connection points.

#### Naming conventions

* Name the tile with the flat edges on the top and bottom.
* Corridor connections are labelled A-F, starting from the top going clockwise.
* Tiles can be rotated, so orient them so the first opening is the earliest letter, e.g. `room-1-exit-a` instead of `room-1-exit-d` (rotated 180 degrees)
* There is no need to name the primary exits separate from the primary feature, e.g. `vertical-1-door-b` has a door exit in the top right face but doesn't bother to name the A and D ends of the corridor.  

TODO: Naming conventions for room sections (i.e. not a corridor connection).

### Combining base tiles

To combine base tiles into a tile group that fits on an A4 page, create a new document in Inkscape, import the needed tiles, rotate if needed, and place at the following locations:

* Tile 0101: x=5, y=5
* Tile 0102: x=5, y=105 
* Half 0201: x=91.603, y=5
* Tile 0202: x=91.603, y=55 
* Half 0203: x=91.603, y=155
* Tile 0301: x=178.205, y=5
* Tile 0302: x=178.205, y=105 

This gives a 5mm margin around the tile group.

To create a PDF you can use Print to PDF (on Windows), or you can export the Page.

## 15mm hex grid

There is also a 15mm hex grid, suitable for overland mapping.

This allows 3 tiles high by 5 tiles wide to fit on an A4 page (with half-tiles along the top and bottom).

Scale up by factors of 4 if you want to be consistent with the base tiles.

e.g. If hexes are 5 feet each, then a base tiles are 20 feet (from centre to centre).

There is a sample map in `15mm\sample` that uses 80 feet hexes (i.e. 4x base tile) and 320 feet larger groupings.

This map is around 1,000 x 1,500 feet, suitable for a town or village and surrounds.

## Folders

* master : Master Inkscape for for creating base tiles (and half-tiles), with layers and groups for different wall segments.
* base-tiles : Exported base tiles in various configurations. Tiles may be rotated as needed, or reversed (if printing on paper you need to print the reversed tiles as well)
* tile-groups : Larger groups of tiles, up to A4 in size. Combine this with individual base tiles as needed.

## Copyright

<img src="by-sa.png" alt="CC BY-SA 4.0" style="width:6rem">

Hextiles © 2024 by Sly Gryphon is licensed under Creative Commons Attribution-ShareAlike 4.0 International. To view a copy of this license, visit <https://creativecommons.org/licenses/by-sa/4.0/>
