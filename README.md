# ImprovedFrameStack

Now-obsolete WoW addon to improve the output of the /framestack tooltip.



Improved FrameStack modifies the /framestack tooltip by attempting to resolve any anonymous frames (i.e. those without names, displayed as memory addresses) to their first named ancestor and the path of keys that lead from that ancestor to the frame, if possible:

It will recursively search the tables of each parent in the chain for some path that can lead to the child. This search is done up to a depth of 3, and this can be modified by changing SavedVariable "IFS_MaxDepth" (no configuration tools - just do a /run IFS_MaxDepth = 4 to change it).

If a link between two ancestors can't be established, "[?]" will be shown for that part of the ancestry tree.
