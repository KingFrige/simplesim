
run
----------------

```bash
$ cd benchmarks

$ ../simplesim-3.0/sim-profile -iclass cc1.alpha -O 1stmt.i

$ ../simplesim-3.0/sim-profile -iclass compress95.alpha < compress95.in > OUT
$ ../simplesim-3.0/sim-profile -all compress95.alpha < compress95.in > OUT
```


sim-outorder
----------------

```bash
$ cd labs/lab-pipeling1
$ ./soo -config config_a.cfg -ptrace config_a.trc 0:1024 -redir:sim sim_configa.out ./test-math

$ cd labs/lab-pipeling2
$ ./soo -config config_a.cfg -ptrace config_a.trc 0:1024 -redir:sim sim_configa.out ./test-math
```


sim-bpred
----------------

```bash
$ cd labs/lab-bpred
$ ./sim-bpred test-math
```


sim-cache
------------

```bash
$ cd labs/lab-cache
$ ./sim-cache -config lab1_cache_1a.cfg test-math
```
