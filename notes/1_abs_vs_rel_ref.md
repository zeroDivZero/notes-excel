# ABSOLUTE VS RELATIVE CELL REFERENCE

When copying formula to another cell, if cell refs in formula relative (to position of cell), new formula updated to new cell refs.

E.g., when copying `=E1/B5` to different location, might be updated to `=G1/D5`.

To restrict to absolute cell location: `=E1/$B$5`. When copied: `=G1/$B$5`.

If available, key `F4` toggles among relative, absolute, and mixed refs in formula or function.
