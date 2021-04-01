## README

### sim-outorder

```bash
$ ln -s ../../simplesim-3.0/sim-cache

$ ln -s ../../simplesim-3.0/tests-alpha/bin/test-math

$ ./sim-cache -config lab1_cache_1a.cfg -redir:sim sim_lab1_cache_1a.out ./test-math

$ ./sim-cache -config lab1_cache_2a.cfg -redir:sim sim_lab1_cache_2a.out ./test-math
```

| Miss  Ratio (I-Cache) | 1-way  | 2-way  | 4-way  | 8-way  |
| --------------------- | ------ | ------ | ------ | :----- |
| 32  sets              | 0.2488 | 0.2408 | 0.2327 | 0.1802 |
| 64  sets              | 0.2431 | 0.2265 | 0.1782 | 0.0624 |
| 128 sets              | 0.2230 | 0.1757 | 0.0836 | 0.0320 |
| 256 sets              | 0.1792 | 0.1005 | 0.0353 | 0.0309 |
| 512  sets             | 0.1392 | 0.0615 | 0.0315 | 0.0308 |


| Miss  Ratio (D-Cache) | 1-way  | 2-way  | 4-way  | 8-way  |
| --------------------- | ------ | ------ | ------ | :----- |
| 32  sets              | 0.2370 | 0.1390 | 0.0789 | 0.0497 |
| 64  sets              | 0.1815 | 0.1038 | 0.0542 | 0.0468 |
| 128 sets              | 0.1423 | 0.0776 | 0.0474 | 0.0459 |
| 256 sets              | 0.0836 | 0.0500 | 0.0460 | 0.0459 |
| 512  sets             | 0.0700 | 0.0473 | 0.0459 | 0.0459 |
