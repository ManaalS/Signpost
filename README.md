# Signpost
Project 0 in my CS61B class (Data Structures). 

Signpost is a puzzle game of sorts. 

The puzzle itself is quite simple. It is played on a W×H rectangular grid of square cells. Every square on the board is annotated with an arrow pointing horizontally, vertically, or diagonally. One special square, the goal, is not annotated with an arrow, but instead is annotated with a star. The goal square also contains the number W⋅H. Another special square, the start, always contains the number 1. By default, the start and the goal will appear in the top-left and bottom-right corners of the board, respectively. Alternatively, the puzzle may be set to have free ends, in which case the start and the goal squares may appear anywhere on the board. The bottom-left corner of the board has the coordinates (0,0), with the positive x-axis running horizontally to the right, and the positive y-axis running vertically upwards.

The player's goal is to assign each unnumbered square a sequence number so that the squares form a chain following the arrows from 1 to W⋅H, using up all numbers in between. We say that square A is connectable to square B if B is one queen move away from A in the direction specified by A's arrow (here, "queen move" refers to the queen move in chess.) 

If A and B are both already numbered, their numbers must be consecutive for them to be considered connectable. To connect two connectable squares, press and hold on the first in sequence and drag to the second. We say that the first is now the predecessor of the second, and the second is now the successor of the first. Whenever a square is numbered, any connected square also becomes numbered with the next or previous consecutive number, as appropriate. To disconnect two connected squares, press and hold on the first, drag to a position off the grid, and release.

If a square initially has a number on the unsolved board, it must be the number of that square in the sequence of connected squares. Such squares are said to be fixed. The start and the goal are always fixed.

When playing the game, the player is not obligated to start forming the sequence from the start. Two connectable squares can be connected even if they are unnumbered. That is, we can form groups of connected squares on the board, which may be connected later to form the solution sequence. If a group does not contain a numbered square, its squares are assigned a letter and an offset. For example, a, a + 1, a + 2 for the 1st, 2nd, and 3rd squares in the group's sequence. Once an unnumbered group is connected to a group whose squares are numbered, the members of the unnumbered group become numbered appropriately.

### More details about the project [here!](https://inst.eecs.berkeley.edu/~cs61b/sp20/materials/proj/proj0/index.html)
#### Note: we were provided skeleton code

