# Style changes (stylesheets, css, colors)
- moved `stylesheet` string into external `.css` files
    - select between them using `formatter.get_stylesheet(...)` e.g. inside `wiked-diff.py`
    - [ ] convert stylesheet options into flags

# Block-move functionality changes
- added `--ignoreBlockMoves` (default=False)
    - Ignore whether block is unique when keeping short blocks. 
    - Using true `True` reduces false postiives for block moves
    - see L1532 in diff.py for logic change
    - ultimately, intended to debug logic for marking blocks as unique to assess root-cause
