## README

### sim-outorder

```bash
$ ln -s ../../simplesim-3.0/sim-outorder soo
$ ln -s ../../simplesim-3.0/pipeview.pl pv

$ ln -s ../../simplesim-3.0/tests-pisa/bin.little/test-math

$ ./soo -config config_a.cfg -ptrace config_a.trc 0:1024 -redir:sim sim_config_a.out ./test-math

$ ./soo -config config_b.cfg -ptrace config_b.trc 0:1024 -redir:sim sim_config_b.out ./test-math
```

