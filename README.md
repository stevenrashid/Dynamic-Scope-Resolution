# Dynamic Scope Resolution

A starting point for documentation about dynamic scope: resolving a variable by examining the active chain of function calls.

## Repository status

This repository currently contains this README only. No implementation, dependency configuration, or tests are included here.

The related Python implementation is available in [Dynamic-Scope-Resolution-Code](https://github.com/stevenrashid/Dynamic-Scope-Resolution-Code).

## Concept

Under dynamic scope, a function looks for a name in its caller's active environment, then continues outward through the call stack. The closest binding wins.

Python normally resolves names lexically. The related project explores dynamic lookup explicitly by inspecting stack frames and building a mapping of visible function-local bindings; it does not change Python's normal name-resolution rules.

## Explore the implementation

See the related repository for `DynamicScope`, `get_dynamic_re()`, usage examples, and notes on shadowed or unbound local variables.
