# Dagmor's Final Fantasy Adventure Musings

This is the default 'landing' branch for hosting GitHub Pages and Issue Templates.

[Check out the website for more details](https://dagmorland.github.io/FFA-Musings/)

## Style Guide for Modifications to Disassembly

1. Retain 5 character spacing between instructions and arguments
2. Use capital letters for registers and conditions
3. Moved original code should append an `#` after the `;;` in the comment; e.g., `;;# 00:1746 $fa $a1 $c0`
4. Modified code in the original location should append an `X` after the `;;` in the comment; e.g., `;;X 01:67e3 ??????`
5. New code (or modified code in a new location) should remove trailing `;;` comments
6. Prefer use of `call` and `ret` instead of `jp` at end of functions when possible
