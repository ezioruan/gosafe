# gosafe

A Go tool to safely compile and run Go programs by only allowing importing of whitelisted packages.

## Why

To enable running any piece of Go code (even if it comes from unknown sources) with ease and safety.

## How

Use `Compiler.Allow` to allow given packages, then run code with `Compiler.Run` or `Compiler.RunFile`.

See https://github.com/zond/gosafe/blob/master/examples/example.go

## More

Use `gosafety.Stdin()`, `gosafety.Stdout()` and `gosafety.Stderr()` in https://github.com/zond/gosafety to communicate with the child processes via structured data. See https://github.com/zond/gosafe/blob/master/testfiles/test3.go for an example.
