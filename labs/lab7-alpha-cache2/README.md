## README

### sim-outorder

```bash
$ ln -s ../../simplesim-3.0/sim-cache

$ ln -s ../../simplesim-3.0/tests-alpha/bin/test-math

$ ./sim-cache -config cache_unified.cfg -redir:sim sim_cache_unified.out ./test-math

$ ./sim-cache -config cache_split.cfg -redir:sim sim_cache_split.out ./test-math
```

| Sets/Assoc | I-Cache Miss No(N/2 sets)+ | D-Cache Miss No(N/2 sets) | Effective Combined      Cache Miss Rate | Unified Cache Miss Rate |
| ---------- | -------------------------- | ------------------------- | --------------------------------------- | :---------------------- |
| 128/1      | 12075/49679                | 2577/14197                | 0.2294                                  | 0.2371                  |
| 128/2      | 10993/49679                | 1473/14197                | 0.1952                                  | 0.1840                  |
| 128/4      | 7929/49679                 | 769/14197                 | 0.1362                                  | 0.0983                  |
| 2048/1     | 3932/49679                 | 891/14197                 | 0.0755                                  | 0.0559                  |
| 2048/2     | 1887/49679                 | 655/14197                 | 0.0398                                  | 0.0343                  |
| 2048/4     | 1654/49679                 | 652/14197                 | 0.0361                                  | 0.0342                  |
| 4096/1     | 2528                       | 766                       | 0.05156                                 | 0.0395                  |
| 4096/2     | 1605                       | 652                       | 0.0353                                  | 0.0342                  |
| 4096/4     | 1563                       | 652                       | 0.0347                                  | 0.0342                  |
| 4096/8     | 1550                       | 652                       | 0.0345                                  | 0.0342                  |

>  effective combined cache miss rate = (data misses + inst misses)/((data accesses + inst accesses)


### Bonus part

| Sets/Assoc | CPI Unified Cache | CPI Split Cache |
| ---------- | ----------------- | --------------- |
| 128/1      |                   |                 |
| 128/2      |                   |                 |
| 128/4      |                   |                 |
| 2048/1     |                   |                 |
| 2048/2     |                   |                 |
| 2048/4     |                   |                 |

