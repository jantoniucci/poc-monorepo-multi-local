PoC on how to include a local monorepo into another
---

* Description

This is an oversimplified example on how to include a local monorepo into another.

architecture-monorepo holds a common class used in functional-domain-monorepo.

functional-domain-monorepo includes architecture-monorepo by declaring a local_repository in the WORKSPACE file (look at the end)

* How to run it
```sh
cd functional-domain-monorepo
bazel build //domains/customer:build
```
