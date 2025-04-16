# Test Cases written by me, made for inital checks for the Inventory system which was made and implemented by my friends

## Test case 1

| Title             | <span style="font-weight:normal">Item Rotation</span>                                                                             |
|:------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Verify that the item rotates 90° as expected.                                                                                     |
| **Preconditions** | Inventory is open; the selected item has a non-square shape (e.g., 2×3) so that rotation is visible.                              |
| **Test data**     | -                                                                                                                                 |

| Action                                                        | Expected result                                                                                                                               |
|:--------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------|
| 1. Select an item from inventory or before placing.           |                                                                                                                                               |
| 2. Press the “Rotate” button (or corresponding hotkey).       |                                                                                                                                               |
| 3. Observe the orientation change.                            | The item rotates 90°. If the item was 2×3, after rotation it should become 3×2. Its position relative to the grid should update accordingly.  |


## Test case 2

| Title             | <span style="font-weight:normal">Green Highlight for Valid Placement</span>                                                      |
|:------------------|:---------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Ensure that valid placement areas are highlighted in green colour.                                                               |
| **Preconditions** | The inventory has enough free grid space, and the item fits in the selected location.                                            |
| **Test data**     | -                                                                                                                                |

| Action                                                        | Expected result                                                                                                |
|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------|
| 1. Select the item to place.                                  |                                                                                                                |
| 2. Hover the cursor over a valid area in the inventory.       |The grid cells under the item are highlighted in green, indicating a valid position.                            |


## Test case 3

| Title             | <span style="font-weight:normal">Red Highlight for Invalid Placement</span>                                                                                                               |
|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Verify that the system properly warns the player when attempting to place an item in an invalid location (e.g., overlaps or insufficient space).                                          |
| **Preconditions** | Some grid cells are already occupied or the placement exceeds the inventory bounds.                                                                                                       |
| **Test data**     | -                                                                                                                                                                                         |

| Action                                                                | Expected result                                                                                   |
|:----------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------|
| 1. Select an item to place.                                           |                                                                                                   |
| 2. Hover the cursor over an area that partially or fully overlaps with another item or doesn't have enough free cells. |      The grid cells are highlighted in red, signaling an invalid placement.   |                   


## Test case 4

| Title             | <span style="font-weight:normal">Blocking Item Placement in Insufficient Space</span>                                               |
|:------------------|:-----------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Ensure that the system blocks item placement if there are not enough grid cells.                                                   |
| **Preconditions** | The item requires e.g., 3 cells, but the hovered area only has 2 free.                                                             |
| **Test data**     | -                                                                                                                                  |

| Action                                                                                                                          | Expected result                                                                                   |
|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------|
| 1. Select the item.                                                                                                             |                                                                                                   |
| 2. Move the cursor to the area with insufficient space.                                                                         |                                                                                                   |
| 3. Try to place the item (click).                                                                                               | The item is not placed; the area is highlighted in red and placement is rejected.                 |


## Test case 5

| Title             | <span style="font-weight:normal">Successful Item Placement</span>                                                                          |
|:------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Confirm that an item can be placed correctly in a valid area.                                                                              |
| **Preconditions** | There’s enough space in the inventory.                                                                                                     |
| **Test data**     | -                                                                                                                                          |

| Action                                                       | Expected result                                                                                              |
|:-------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------|
| 1. Select the item.                                          |                                                                                                              |
| 2. Hover over an area highlighted in green.                  |                                                                                                              |
| 3. Click to confirm placement.                               | The item is placed in the inventory and occupies the appropriate grid cells. The cells become unavailable for future placements. |


## Test case 6

| Title             | <span style="font-weight:normal">Inventory Sorting Functionality</span>                                                         |
|:------------------|:--------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Check if the sort button optimizes inventory layout by minimizing empty space.                                                  |
| **Preconditions** | Items are scattered within the inventory with gaps between them.                                                                |
| **Test data**     | -                                                                                                                               |

| Action                                                       | Expected result                                                                                              |
|:-------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------|
| 1. Click the “Sort Inventory” button.                        |                                                                                                              |
| 2. Observe how items are rearranged.                         | Items are moved to optimize space, minimizing gaps and resulting in a more organized layout.                 |


## Test case 7

| Title             | <span style="font-weight:normal">Inventory Scroll via Sidebar</span>                                                              |
|:------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Verify scrolling works using the sidebar.                                                                                         |
| **Preconditions** | The inventory has more grid cells than can be displayed at once.                                                                  |
| **Test data**     | -                                                                                                                                 |

| Action                                                       | Expected result                                                                                               |
|:-------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------|
| 1. Click and drag the sidebar up and down.                   |                                                                                                               |
| 2. Observe the visible area.                                 | The visible section of the inventory updates correctly as the sidebar moves.                                  |


## Test case 8

| Title             | <span style="font-weight:normal">Inventory Scroll via Mouse Wheel</span>                                                          |
|:------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Ensure the inventory can be scrolled using the mouse wheel.                                                                       |
| **Preconditions** | The inventory contains more grid cells than the visible area.                                                                     |
| **Test data**     | -                                                                                                                                 |

| Action                                                       | Expected result                                                                                                                                                       |
|:-------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1. Scroll the mouse wheel up and down.                       |                                                                                                                                                                       |
| 2. Observe the inventory content.                            | The inventory scrolls smoothly according to the mouse wheel movement.                                                                                                 |


## Test case 9

| Title             | <span style="font-weight:normal">Full 360° Rotation</span>                                                                          |
|:------------------|:------------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Ensure that rotating the item four times returns it to its original orientation.                                                    |
| **Preconditions** | An item is selected and visible.                                                                                                    |
| **Test data**     | -                                                                                                                                   |

| Action                                                       | Expected result                                                                                               |
|:-------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------|
| 1. Rotate the item 90°.                                      |                                                                                                               |
| 2. Repeat 3 more times (total of 4 rotations).               |                                                                                                               |
| 3. Compare the final orientation to the original one.        | The item returns to its original orientation after 4 rotations.                                               |


## Test case 10

| Title             | <span style="font-weight:normal">Prevent Placement on Occupied Grid</span>                                                   |
|:------------------|:-----------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Verify the system prevents placing an item on already occupied grid cells.	                                                 |
| **Preconditions** | Another item is already placed in the grid.                                                                                  |
| **Test data**     | -                                                                                                                            |

| Action                                                       | Expected result                                                                                                                        |
|:-------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| 1. Select a new item to place.                               |                                                                                                                                        |
| 2. Hover over an area with occupied grid cells.              |                                                                                                                                        |
| 3. Try to place the item.                                    | Placement is denied; the area is highlighted red and the item remains unplaced.                                                        |


## Test case 11

| Title             | <span style="font-weight:normal">Canceling Item Placement</span>                                                                      |
|:------------------|:--------------------------------------------------------------------------------------------------------------------------------------|
| **Description**   | Ensure that players can cancel item placement.	 	                                                                                    |
| **Preconditions** | An item is selected and grid highlight is active.                                                                                     |
| **Test data**     | -                                                                                                                                     |

| Action                                                       | Expected result                                                                                               |
|:-------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------|
| 1. While hovering with the item, press “Cancel” or ESC.      |                                                                                                               |
| 2. Observe the grid.                                         | Placement mode exits, highlight disappears, and the item is not added to inventory.                           |
