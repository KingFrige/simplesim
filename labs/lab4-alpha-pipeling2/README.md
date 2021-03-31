## README

### sim-outorder

```bash
$ ln -s ../../simplesim-3.0/sim-outorder soo
$ ln -s ../../simplesim-3.0/pipeview.pl pv

$ ln -s ../../simplesim-3.0/tests-alpha/bin/test-math

$ ./soo -config config_c.cfg -ptrace config_c.trc 0:1024 -redir:sim sim_config_c.out ./test-math

$ ./soo -config config_d.cfg -ptrace config_d.trc 0:1024 -redir:sim sim_config_d.out ./test-math
$ ./soo -config config_d1.cfg -ptrace config_d1.trc 0:1024 -redir:sim sim_config_d1.out ./test-math

$ ./soo -config config_e.cfg -ptrace config_e.trc 0:1024 -redir:sim sim_config_e.out ./test-math

$ ./soo -config config_f.cfg -ptrace config_f.trc 0:1024 -redir:sim sim_config_f.out ./test-math

$ ./soo -config config_g.cfg -ptrace config_g.trc 0:1024 -redir:sim sim_config_g.out ./test-math

$ ./soo -config config_h.cfg -ptrace config_h.trc 0:1024 -redir:sim sim_config_h.out ./test-math

$ ./pv config_c.trc | less
```

