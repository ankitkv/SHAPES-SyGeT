# SHAPES-SyGeT

SHAPES-SyGeT (**SHAPES** **Sy**stematic **Ge**neralization **T**est) is a split of the SHAPES dataset [1] that can be used to evaluate systematic generalization.

## Templates

#### Train templates:
 1. is a `COLOR` shape `TRANSFORM` a `COLOR` shape
2. is a `SHAPE` `TRANSFORM` a `COLOR` shape
3. is a `SHAPE` `TRANSFORM` `TRANSFORM` a `COLOR` shape
4. is a `SHAPE` `TRANSFORM` `TRANSFORM` a `SHAPE`
5. is a `COLOR` shape a `SHAPE`
6. is a `SHAPE` `COLOR`
7. is a `SHAPE` a `SHAPE`
#### Evaluation templates:
8. is a `COLOR` shape `TRANSFORM` `TRANSFORM` a `COLOR` shape
9. is a `COLOR` shape `TRANSFORM` a `SHAPE`
10. is a `COLOR` shape `TRANSFORM` `TRANSFORM` a `SHAPE`
11. is a `SHAPE` `TRANSFORM` a `SHAPE`
12. is a `COLOR` shape `COLOR`

`COLOR` can take values in 'red', 'green', 'blue'
`SHAPE` can take values in 'circle', 'triangle', 'square'
`TRANSFORM` can take values in 'above', 'below', 'left of', 'right of'

## Splits

`Train` and `Val-IID` use train templates. `Val-OOD` uses evaluation templates.

`Train` size: 7560
`Val-IID` size: 1080
`Val-OOD` size: 6976

## References

[1] Jacob Andreas, Marcus Rohrbach, Trevor Darrell, and Dan Klein. “Neural module networks.” In: *Proceedings of the IEEE conference on computer vision and pattern recognition.* 2016, pp. 39–48.
