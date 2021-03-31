## README

### sim-bpred

```bash
$ cd ../../benchmarks
```

- ANAGRAM

```bash
# to run:               
$ ../simplesim-3.0/sim-bpred -bpred taken anagram.alpha words < anagram.in > OUT

$ ../simplesim-3.0/sim-bpred -bpred nottaken anagram.alpha words < anagram.in > OUT

$ ../simplesim-3.0/sim-bpred -bpred bimod anagram.alpha words < anagram.in > OUT

# to test output:       
$ diff OUT anagram.out
```

- GO

```bash
# to run:               
$ ../simplesim-3.0/sim-bpred -bpred taken go.alpha 50 9 2stone9.in > OUT

$ ../simplesim-3.0/sim-bpred -bpred nottaken go.alpha 50 9 2stone9.in > OUT

$ ../simplesim-3.0/sim-bpred -bpred bimod go.alpha 50 9 2stone9.in > OUT

# to test output:       
$ diff OUT go.out
```

- COMPRESS95:

```bash
# to run:               
$ ../simplesim-3.0/sim-bpred -bpred taken compress95.alpha < compress95.in > OUT

$ ../simplesim-3.0/sim-bpred -bpred nottaken compress95.alpha < compress95.in > OUT

$ ../simplesim-3.0/sim-bpred -bpred bimod compress95.alpha < compress95.in > OUT

# to test output:       
$ diff OUT compress95.out
```

- GCC

```bash
# to run:               
$ ../simplesim-3.0/sim-bpred -bpred taken cc1.alpha -O 1stmt.i

$ ../simplesim-3.0/sim-bpred -bpred nottaken cc1.alpha -O 1stmt.i

$ ../simplesim-3.0/sim-bpred -bpred bimod cc1.alpha -O 1stmt.i

# to test output:       
$ diff 1stmt.s 1stmt.s.ref
```

| Benchmark      | Taken <br />Branch Address Prediction Rate | Not Taken<br />Branch Address Prediction Rate | Bimod(2bit  prediction)<br />Branch Add Prediction Rate |
| -------------- | ------------------------------------------ | --------------------------------------------- | ------------------------------------------------------- |
| anagram.alpha  | 0.6874                                     | 0.6149                                        | 0.9613                                                  |
| go.alpha       | 0.6221                                     | 0.5689                                        | 0.7848                                                  |
| compress.alpha | 0.9728                                     | 0.0594                                        | 0.9615                                                  |
| gcc.alpha      | 0.6005                                     | 0.6357                                        | 0.8682                                                  |



### sim-outorder

```bash
$ cd ../../benchmarks
```

- ANAGRAM

```bash
# to run:               
$ ../simplesim-3.0/sim-outorder -config ../labs/lab5-alpha-bpred/taken-bpred.cfg -ptrace ../labs/lab5-alpha-bpred/taken-bpred.trc 0:1024 -redir:sim ../labs/lab5-alpha-bpred/sim_taken_bpred.out anagram.alpha words < anagram.in > OUT

$ ../simplesim-3.0/sim-outorder -config ../labs/lab5-alpha-bpred/nottaken-bpred.cfg -ptrace ../labs/lab5-alpha-bpred/nottaken-bpred.trc 0:1024 -redir:sim ../labs/lab5-alpha-bpred/sim_nottaken_bpred.out anagram.alpha words < anagram.in > OUT

$ ../simplesim-3.0/sim-outorder -config ../labs/lab5-alpha-bpred/bimod-bpred.cfg -ptrace ../labs/lab5-alpha-bpred/bimod-bpred.trc 0:1024 -redir:sim ../labs/lab5-alpha-bpred/sim_bimod_bpred.out anagram.alpha words < anagram.in > OUT

# to test output:
$ diff OUT anagram.out
```

- COMPRESS95:

```bash
# to run:
$ ../simplesim-3.0/sim-outorder -config ../labs/lab5-alpha-bpred/taken-bpred.cfg -ptrace ../labs/lab5-alpha-bpred/taken-bpred.trc 0:1024 -redir:sim ../labs/lab5-alpha-bpred/sim_taken_bpred.out compress95.alpha < compress95.in > OUT

$ ../simplesim-3.0/sim-outorder -config ../labs/lab5-alpha-bpred/nottaken-bpred.cfg -ptrace ../labs/lab5-alpha-bpred/nottaken-bpred.trc 0:1024 -redir:sim ../labs/lab5-alpha-bpred/sim_nottaken_bpred.out compress95.alpha < compress95.in > OUT

$ ../simplesim-3.0/sim-outorder -config ../labs/lab5-alpha-bpred/bimod-bpred.cfg -ptrace ../labs/lab5-alpha-bpred/bimod-bpred.trc 0:1024 -redir:sim ../labs/lab5-alpha-bpred/sim_bimod_bpred.out compress95.alpha < compress95.in > OUT

# to test output:       
$ diff OUT compress95.out
```


| Benchmark      | Taken <br />Branch Address Prediction Rate | Not Taken<br />Branch Address Prediction Rate | Bimod(2bit  prediction)<br />Branch Add Prediction Rate |
| -------------- | ------------------------------------------ | --------------------------------------------- | ------------------------------------------------------- |
| anagram.alpha  | 0.9549                                     | 0.9619                                        | 0.4572                                                  |
| compress.alpha | 0.7814                                     | 0.7822                                        | 0.5571                                                  |
