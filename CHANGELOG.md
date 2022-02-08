# 0.8.3

- Dropped support for GHC < 7.8.
- Tested with GHC 7.8 - 9.2.
- new module `System.Clock.Seconds`. This is a wrapper type for `TimeSpec` that behaves similarly to `Data.Fixed.Nano` or `Double`. `fromInteger 1` is 1 second.
- The multiplication of the `Num TimeSpec` instance was changed so `2 * 2 == 4`. Before, it reduced to `0`. Also `signum` was changed to match, it returns ±1 nanosecond.
- TODO: other changes
