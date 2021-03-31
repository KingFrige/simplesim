## README

### alpha

```bash
$ cd simplesim-3.0
$ ./make clean
$ ./make config-alpha
$ ./make

cd tests-alpha/bin
```

- test-math

```bash
$ ../../sim-profile -iclass test-math
```

  

- test-fmath

```bash
$ ../../sim-profile -iclass test-fmath
```

- test-llong

```bash
$ ../../sim-profile -iclass test-llong
```

- test-printf

```bash
$ ../../sim-profile -iclass test-printf
```


| Benchmark   | Total of Instructions | Load% | Store% | Uncond Branch% | Cond Branch% | Integer Computation% | Floating pt Computation% | trap |
| ----------- | --------------------- | ----- | ------ | :------------- | ------------ | -------------------- | ------------------------ | ---- |
| test-math   | 49421                 | 17.18 | 10.41  | 3.94           | 11.08        | 55.35                | 1.88                     | 0.16 |
| test-fmath  | 19510                 | 17.73 | 12.51  | 4.70           | 11.29        | 53.18                | 0.43                     | 0.16 |
| test-llong  | 10638                 | 17.82 | 14.58  | 5.42           | 12.43        | 49.46                | 0.10                     | 0.19 |
| Test-printf | 983484                | 17.99 | 10.73  | 4.82           | 11.39        | 54.84                | 0.09                     | 0.13 |

### pisa

```bash
$ cd simplesim-3.0
$ ./make clean
$ ./make config-pisa
$ ./make

cd tests-pisa/bin.little
```

- test-math

```bash
$ ../../sim-profile -iclass test-math
```

  

- test-fmath

```bash
$ ../../sim-profile -iclass test-fmath
```

- test-llong

```bash
$ ../../sim-profile -iclass test-llong
```

- test-printf

```bash
$ ../../sim-profile -iclass test-printf
```


| Benchmark   | Total of Instructions | Load% | Store% | Uncond Branch% | Cond Branch% | Integer Computation% | Floating pt Computation% | trap |
| ----------- | --------------------- | ----- | ------ | :------------- | ------------ | -------------------- | ------------------------ | ---- |
| test-math   | 213553                | 15.96 | 10.67  | 4.22           | 13.84        | 54.42                | 0.88                     | 0.01 |
| test-fmath  | 53312                 | 16.17 | 14.47  | 4.24           | 15.08        | 49.90                | 0.11                     | 0.03 |
| test-llong  | 29495                 | 16.38 | 18.11  | 4.37           | 15.40        | 45.70                | 0.00                     | 0.04 |
| Test-printf | 1813745               | 19.22 | 9.28   | 5.13           | 17.01        | 49.33                | 0.01                     | 0.01 |
