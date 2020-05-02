 # Duplicate lines in a text file

Remove duplicate lines from a file without changing the order

`awk '!_[$0]++' file.txt`

Show only duplicates

`awk '_[$0]++' file.txt`

show unique by an individual column

`awk '!_[$1]++' file.txt`


### references

[@M_C_Stott](https://twitter.com/M_C_Stott/status/1255388471977484288)
[(backup)](https://archive.is/g7cod)
