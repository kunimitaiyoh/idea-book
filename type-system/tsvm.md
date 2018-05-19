# TypeScript Virtual Template

*JSX*, a format for *Virtual DOM* document is suitable for describing normal HTML.
In JSX, however, because any dynamic content must be represented as a JavaScript's *expression*, it is hard to describe control statements simply like `if` or `for`.

[jsx-control-statements](https://github.com/AlexGilleran/jsx-control-statements) solves this problem well. jsx-control-statements allows you to describe such control statements as one of DOM element, it rapidly imporoves the readability.

## Milestones

- create extensions for text editors (especially *VS Code*)
- syntax parser and highlight
- appropriate conversion to TypeScript or JavaScript
- support webpack
- statically analysis: diagnostics and code completion on Language Server Protocol

## TODO

1. [ ] implement simple parser with PEG
2. [ ] generate TypeScript code with AST
3. [ ] develop extension for VS Code implementing Language Server
