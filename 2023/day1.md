# day 1

## assumptions

- 0 isn't one of the digits
- ~there is always at least 1 number~
  - the box should handle this case (it'll return 0)

--

the box contains three variables (which are integers);

- `first = 0`
  - this holds the first digit in each line, multiplied by 10
- `last = 0`
  - this holds the last (previous) digit that the box has seen
  - if the line only has one number, last = the first number ✔️
- `total = 0`
  - 



As they're making the final adjustments, they discover that their calibration document (your puzzle input) has been amended by a very young Elf who was apparently just excited to show off her art skills. Consequently, the Elves are having trouble reading the values on the document.

The newly-improved calibration document consists of lines of text; each line originally contained a specific calibration value that the Elves now need to recover. On each line, the calibration value can be found by combining the first digit and the last digit (in that order) to form a single two-digit number.

For example:

1abc2
pqr3stu8vwx
a1b2c3d4e5f
treb7uchet
In this example, the calibration values of these four lines are 12, 38, 15, and 77. Adding these together produces 142.

Consider your entire calibration document. What is the sum of all of the calibration values?

To begin, get your puzzle input.

Answer: 
# analysis?

- memory: this should be contant memory, so optimised? ✔️
