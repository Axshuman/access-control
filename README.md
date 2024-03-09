# Access-Control-Project

This folder contains source code that explains about access control in Cadence Language.
`SomeContract` demonstrates the use of variables and functions with different Solidity visibility settings. Here, we break down the access and modification scopes for four variables (`a`, `b`, `c`, `d`) and the callability of three functions (`publicFunc`, `contractFunc`, `privateFunc`) within different contexts.

## Variables

- `a` (public): Readable and writable from **anywhere**. Both within the contract, by other contracts, and by external transactions.
- `b` (internal): Readable and writable from **within this contract** and **contracts derived from it**. It's not accessible for external contracts directly.
- `c` (private): Readable and writable **only within this contract**. Even derived contracts cannot access it.
- `d` (external): This type doesn't apply to variables, so assuming you meant a public or internal variable, the scopes for `a` or `b` would apply accordingly.

## Functions

- `publicFunc`: Callable **from anywhere** - inside the contract, from other contracts, and through transactions.
- `contractFunc` (assuming it's `internal`): Callable **within this contract and derived contracts**. Not accessible from external transactions directly.
- `privateFunc`: Callable **only within this contract**. Neither derived contracts nor external entities can call it.

## Author

Axshuman

## License

This project is licensed under the [MIT License](LICENSE).
