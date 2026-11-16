+++
title = "Command line"
weight = 4
+++

```
python ocm\bc_tool.py list
python ocm\bc_tool.py show latest:BDC_BODY3 --group 3221
python ocm\bc_tool.py values latest:BDC_BODY3 3221:12:12:11111111b
python ocm\bc_tool.py set latest:BDC_BODY3 "3221:12:12:11111111b=mode Comfort+" --note "test"
python ocm\bc_tool.py apply latest:HU_MGU workspace\bimmercode\edits\my_changes.tsv
python ocm\bc_tool.py diff <backup A> <backup B>
```

`<backup>` is `latest:<ECU name | 0x63 | CAFD id>` or any unique part of a file name. Values can be hex, a label, or
`wert_NN`. Values outside the CAFD's list are refused unless you add `--allow-custom`.
