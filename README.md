# 013-debugging

Day 13 of Udemy's *100 Days of Code: Python Pro Bootcamp*: finding and fixing
bugs in Python code.

All exercises live in [`src/main.py`](src/main.py), each commented out with the
fix noted beside it. Uncomment one at a time to run it.

## Exercises

| Exercise | Bug | Fix |
| --- | --- | --- |
| Describe the Problem | `range(1, 20)` never reaches 20, because the upper bound is excluded | Use `range(1, 21)` |
| Reproduce the Bug | `dice_imgs[dice_num]` raises `IndexError` when the roll is 6 | Index with `dice_num - 1` |
| Play Computer | A birth year of exactly 1994 matches no branch | Use `>=` in the `elif` |
| Fix the Errors | `input()` returns a string, so `age > 18` fails; the `print` is not indented | Convert with `int()`; indent the `print` |
| Print is Your Friend | `==` compares instead of assigning, so `word_per_page` stays 0 | Use `=` |
| Use a Debugger | `b_list.append(new_item)` sits outside the loop, so only the last item is kept | Indent it into the loop |

## Debugging approach

1. Describe the problem in your own words.
2. Reproduce the bug.
3. Play computer: step through the code by hand.
4. Fix the errors the interpreter reports.
5. Use `print()` to inspect values.
6. Use a debugger to step through execution.

## Running

Requires Python 3.

```bash
python src/main.py
```
