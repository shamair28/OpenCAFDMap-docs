+++
title = "The names format"
weight = 1
+++

Tab-separated, UTF-8, one name per row:

```
cafd_id   address  start  end  mask       value_hex  name                    comment
00007083  3024                                       Batteryguard            BimmerCode expert mode group list
00007083  3221     13     13   11111111b             FesComfortWorldMode2    mapped E-Sys tree screenshot
00007083  3221     12     12   11111111b  05         mode Comfort+           drive-mode IDs from a coding guide
00007083  3221     9      9    11111111b                                     comment only: what this byte does
```

| Row type | Fill in |
|---|---|
| Group name | `cafd_id`, `address`, `name` |
| Function name | + `start`, `end`, `mask` |
| Value name | + `value_hex` |
| Comment only | function columns + `comment`, empty `name`. Use it when you know what a function does but not its BMW name. |

- **cafd_id**: 8 hex digits (`00007083`). **address**: the datagroup, 4 hex digits (`3221`).
- **start / end / mask**: the function's position. Copy them from the Backup Editor's detail pane
  (`byte 9  mask 11111111b`), or from the placeholder name: `PfFesMaster_9_9_255` is start 9, end 9, mask 255 =
  `11111111b`. Write the mask in binary with a trailing `b`.
- **name**: BMW's own name if you know it (`FesSportPlusMode`, `INBAND_RINGING`). Otherwise a short, clear
  description.
- **comment**: **where the name comes from** (screenshot of tool X, BimmerCode diff, coding table, forum thread).
  This lets others judge and verify it.

Names don't depend on the software version. A row applies to every version of that CAFD that has a function with
exactly that address, byte range and mask.
