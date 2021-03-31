## README

### alpha

```bash
$ cd ../../benchmarks
```

- ANAGRAM

```bash
# to run:               
$ ../simplesim-3.0/sim-profile -iclass anagram.alpha words < anagram.in > OUT
# to test output:       
$ diff OUT anagram.out
```

- GO

```bash
# to run:               
$ ../simplesim-3.0/sim-profile -iclass go.alpha 50 9 2stone9.in > OUT
# to test output:       
$ diff OUT go.out
```

- COMPRESS95:

```bash
# to run:               
$ ../simplesim-3.0/sim-profile -iclass compress95.alpha < compress95.in > OUT
# to test output:       
$ diff OUT compress95.out
```

- GCC

```bash
# to run:               

$ ../simplesim-3.0/sim-profile -iclass cc1.alpha -O 1stmt.i
# to test output:       
$ diff 1stmt.s 1stmt.s.ref
```

| Benchmark      | Total of Instructions | Load% | Store% | Uncond Branch% | Cond Branch% | Integer Computation% | Floating pt Computation% | trap |
| -------------- | --------------------- | ----- | ------ | :------------- | ------------ | -------------------- | ------------------------ | ---- |
| anagram.alpha  | 25597588              | 25.36 | 9.93   | 4.46           | 10.30        | 44.63                | 5.31                     | 0.01 |
| go.alpha       | 545811962             | 30.62 | 8.17   | 2.58           | 10.96        | 47.64                | 0.03                     | 0.00 |
| compress.alpha | 88154                 | 1.59  | 79.21  | 0.19           | 5.72         | 13.26                | 0.00                     | 0.02 |
| gcc.alpha      | 337341130             | 24.67 | 11.47  | 4.12           | 13.33        | 46.30                | 0.11                     | 0.00 |
