#postgres-vm

##What's this
This is an in-development branch of postgres fork that compiles WHERE clauses to immediate codes and executes them with JIT compiler.

##How to use
./configure && make && sudo make install

In psql,
set vm_level to 2(or 0, 1)

- vm_level 0 is normal postgres with no immediate code and jit.
- vm_level 1 executes with immediate code compilation.
- vm_level 2 enables JIT compiler.
