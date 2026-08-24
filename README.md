# Circleus Contract

Public contract repository for Circleus, the reusable Circles/group-Space
extension. It owns the wire and contract-facing surfaces consumed by the
Circleus implementation; this repository is still partly scaffold-derived and
its `template` paths have not yet all been renamed.

`frontend/` is the sole owner and publisher of the Circleus contract package.
Until the scaffold rename is completed, its generated package name remains
`@sneat/extension-template-contract`. The paired implementation/app repository
is [`circleus`](https://github.com/sneat-co/circleus); it consumes this package
and owns runtime/app code.

## Layout

```text
typespec/   # frozen wire contract
backend/    # contract-facing Go definitions and checks
frontend/   # @sneat/extension-<id>-contract workspace
```
