notes & formulas
================

### acknowledgements

- [**@jeppes**](https://github.com/jeppes), the best co-conspirator and rubber duck
- [The genius(es) behind the GitHub Docs on syntax formatting](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

---

> [!TIP]
> To maximise the body text:
> - uncheck/delete:
>     - `min-width: 60em` defined on `body`
>     - `min-width: 45em` defined on `article` (in `body` > `main`)
> - delete the `div` named `sidebar` (in `body`, after `header`)

---

## day 1

- given: two (unsorted) lists of location IDs --> `L-unsorted`, `R-unsorted`
     - **[assumption]** the lists are the same length --> `length`
          - if the lists aren't the same length, would `distance` for the unpaired IDs be `0` (or maybe the IDs themselves)?

### part 1

- sort the lists --> `L`, `R`
- `total-distance = 0`
- for `i = [1, length]`:
    - `distance = the absolute value of (L_i - R_i)`
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
