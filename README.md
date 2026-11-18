# Replicube Solutions

Replicube is a game by [Walaber Entertainment](https://www.walaber.com/replicube) about writing code to replicate 3D voxel objects. Each puzzle shows you a target shape, which is made of smaller colored cubes.

Your job in the game is to write a small program (in Lua) that reproduces it exactly. It's comparable to [Picross 3D](https://en.wikipedia.org/wiki/Picross_3D), but with coding instead of clicking.

When you submit code, it is graded on code size and on cycles, and then put on a leaderboard to be compared to all other submitted solutions.

This repository contains my solutions to the challenges provided by the game. Each challenge contains two solutions in the file, one optimized for code size, and one for cycles (efficiency). Unless—of course—they are the same.

# Repository Layout

The structure is ordered chronologically, based on the progress of the game. Starting off with tutorial projects, going up to increasing difficulties. The overall structure can be summarized as show below:

```
root/
|- 001-tutorial-projects/             # Solutions to the "tutorial projects" challenges
|  |- 001-[project].lua               # Code file containing solution(s)
|  |- 001-[project]_size.png          # Image of the result (optimized for size)
|  |- 001-[project]_efficiency.png    # Image of the result (optimized for efficiency)
|- README.md
```

<sub>*P.S. If an image has no `_suffix`, then it is a combined result*</sub>



The code files have the following structure _(example)_:

```lua
-- code size: 10 | cycles/voxel: 4.000 | optimized for: size
return -- code here

-- code size: 30 | cycles/voxel: 3.000 | optimized for: efficiency
return -- code here
```

Each project containing challenges also contains a table with an overview in its corresponding README. This way a visitor can quickly glance at what they need. If there are multiple images shown in the table, the size is on the left and the efficiency is on the right, just like the headings.

# Usage

1. Open the puzzle in Replicube
2. Copy the contents of the matching .lua file into the code editor
3. Run it and check the results against the target(s)

# Disclaimer

*This is a showcase/fun project and has no affiliation with Walaber Entertainment. Replicube is available on Steam for Windows, Mac and Linux.*