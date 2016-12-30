# Solutions for regexcrossword.com

## Notes

* When you see `\s` in an answer box, it means you actually need to press the spacebar.

### Tutorial

#### (1) the OR symbol

|                 | A&#124;B |
|:---------------:|:--------:|
| <b>A&#124;Z</b> | A        |

#### (2) a range of characters

|              | [ABC] |
|:------------:|:-----:|
| <b>[BDF]</b> | B     |

#### (3) characters NOT to include

|              | [^AB] |
|:------------:|:-----:|
| <b>[ABC]</b> | C     |

#### (4) zero or more

|            | A* |
|:----------:|:--:|
| <b>A</b>   | A  |
| <b>AB+</b> | A  |

#### (5) zero or one

|                 | A?B? |
|:---------------:|:----:|
| <b>A&#124;C</b> | A    |
| <b>B</b>        | B    |

#### (6) one or more

|                 | A+ |
|:---------------:|:--:|
| <b>A&#124;B</b> | A  |
| <b>A&#124;Z</b> | A  |

#### (7) backreference

|                 | (A)\1 |
|:---------------:|:-----:|
| <b>A&#124;B</b> | A     |
| <b>A&#124;B</b> | A     |

#### (8) specific amount

|                 | A{2,} |
|:---------------:|:-----:|
| <b>A{1}</b>     | A     |
| <b>B&#124;A</b> | A     |

#### (9) space

|           | A&#124;\s |
|:---------:|:---------:|
| <b>\s</b> | \s        |
