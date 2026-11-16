+++
title = "Coverage"
weight = 1
+++

![Coding names by chassis: every CAFD is named, with verified BMW names where they exist and dynamically calculated names for the rest](coverage.svg)

Every CAFD is named. BMW's untrimmed names cover about 149,000 functions, 274,000 values and 5,400 groups across 164
CAFD ids, for G- and F-chassis ECUs. For G020 and F030, about 89% of functions across every CAFD version carry these
verified names.

OpenLauncher dynamically calculates the rest: functions are named from their group, byte and mask, and values are
labelled with their coding rules. Untrimmed dumps of CAFDs your series doesn't share with G020 or F030 raise its
coverage the most; see [Contributing](@/contributing/_index.md).

OpenLauncher works with any main series: set it in [Settings](@/getting-started/settings.md).
