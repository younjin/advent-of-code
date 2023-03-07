# Day 1: Calorie Counting

[Link to problem](https://adventofcode.com/2022/day/1)

- Input: **Calories** that each Elf is carrying
- Each line is either the number of Calories an item contains, or a blank line (that separates the inventory of one Elf from another)
- Output: the total number of Calories the Elf carrying the most Calories is carrying

## Initial thoughts

- just for my sanity, we're going to zero-index the Elves
- open file `f` of food items
- create a list `l` where:
    - index `i` corresponds to the `i`th Elf
    - `l[i]` corresponds to the total # of Calories the `i`th Elf is carrying
- create a variable `m` set to `0`
- iterate through the items in `f`
    - set the index counter `c` to `0` 
    - if the line contains an item, add the amount to `f[c]`
    - if the line is a empty line:
        - if `f[c] > m`, set `m` to `f[c]`
        - increment the counter `c` by 1
- end result should be:
    - list `l` with the sum items carried by the `len(l)` elves
    - max total `m` with the total number of Calories the Elf carrying the most Calories is carrying
- return `m`