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

### Beginner

#### (1) beatles

|                           | [^SPEAK]+ | EP&#124;IP&#124;EF |
|:-------------------------:|:---------:|:------------------:|
| <b>HE&#124;LL&#124;O+</b> | H         | E                  |
| <b>[PLEASE]+</b>          | L         | P                  |

#### (2) naughty

|                             | (A&#124;B&#124;C)\1 | (AB&#124;OE&#124;SK) |
|:---------------------------:|:-------------------:|:--------------------:|
| <b>.&#42;M?O.&#42;</b>      | B                   | O                    |
| <b>(AN&#124;FE&#124;BE)</b> | B                   | E                    |

#### (3) ghost

|                 | [COBRA]+ | (AB&#124;O&#124;OR)+ |
|:---------------:|:--------:|:--------------------:|
| <b>(.)+\1</b>   | O        | O                    |
| <b>[^ABRC]+</b> | O        | O                    |

#### (4) symbolism

|             | .?.+ | .+ |
|:-----------:|:----:|:--:|
| <b>[*]+</b> | *    | *  |
| <b>/+</b>   | /    | /  |

#### (5) airstrip one

|                           | \d[2480] | 56&#124;94&#124;73 |
|:-------------------------:|:--------:|:------------------:|
| <b>18&#124;19&#124;20</b> | 1        | 9                  |
| <b>[6789]\d</b>           | 8        | 4                  |

### Intermediate

#### (1) always remember

|                              | UB&#124;IE&#124;AW | [TUBE]* | [BORF]. |
|:----------------------------:|:------------------:|:-------:|:-------:|
| <b>[NOTAD]*</b>              | A                  | T       | O       |
| <b>WEL&#124;BAL&#124;EAR</b> | W                  | E       | L       |

#### (2) johnny

|                             | [BQW]&#40;PR&#124;LE) | [RANK]+ |
|:---------------------------:|:---------------------:|:-------:|
| <b>[AWE]+</b>               | W                     | A       |
| <b>[ALP]+K</b>              | L                     | K       |
| <b>(PR&#124;ER&#124;EP)</b> | E                     | R       |

#### (3) earth

|                              | .(.)\1 | .*[WAY]+ | [RAM].[OH] |
|:----------------------------:|:------:|:--------:|:----------:|
| <b>CAT&#124;FOR&#124;FAT</b> | F      | O        | R          |
| <b>RY&#124;TY\-</b>          | T      | Y        | -          |
| <b>[TOWEL]*</b>              | T      | W        | O          |

#### (4) encyclopedia

|                      | [JUNDT]* | APA&#124;OPI&#124;OLK | (NA&#124;FE$#124;HE)[CV] |
|:--------------------:|:--------:|:---------------------:|:------------------------:|
| <b>[DEF][MNO]*</b>   | D        | O                     | N                        |
| <b>[^DJNU]P[ABC]</b> | T        | P                     | A                        |
| <b>[ICAN]*</b>       | N        | I                     | C                        |
