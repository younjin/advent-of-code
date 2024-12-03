notes & formulas
================

_to maximise the body text:_

- open the AoC site on a half window
- uncheck `min-width: 60em` defined on `body` and `min-width: 45em` defined on `article`
- delete the `div` named `sidebar`

---

## day 1

- given: two lists of location IDs (unsorted) --> `L-unsorted`, `R-unsorted`
     - **assumption**: the lists are the same length

### part 1

- sort the lists --> `L`, `R`
- `total-distance = 0`
- for `i = [1, length of the lists]`:
    - `distance = the absolute value of (L_i - R_i)`
        - if the lists aren't the same length, would `distance` for the unpaired IDs be `0` (or the IDs themselves)?
    - `total-distance = total-distance + distance`
- return `total-distance`

### part 2

- take the sorted right list `R`
- lookup table --> `count`
- for each value `r` in `R`:
    - if `r` isn't a key in `count`:
        - add `r` as a new key, set its value (`r_v`) to `1`
    - else:
        - `r_v = r_v + 1`
- `similarity = 0`
- for each value `l` in `L`:
    - if `l` is in `count`:
        - `similarity = l * l_v` (where `l_v` is the value associated with `l`)
- return `similarity`

---

## day 2

### part 1

### part 2

---
