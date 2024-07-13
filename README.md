# Welcome to urfave/cli-docs/v3

[![Run Tests](https://github.com/urfave/cli-docs/actions/workflows/main.yml/badge.svg)](https://github.com/urfave/cli-docs/actions/workflows/main.yml)
[![Go Reference](https://pkg.go.dev/badge/github.com/urfave/cli-docs/v3.svg)](https://pkg.go.dev/github.com/urfave/cli-docs/v3)
[![Go Report Card](https://goreportcard.com/badge/github.com/urfave/cli-docs/v3)](https://goreportcard.com/report/github.com/urfave/cli-docs/v3)

urfave/cli-docs/v3 is an extended documentation library for use with urfave/cli/v3.

## Start using

1. Add the dependency to your project

```sh
 go get github.com/urfave/cli-docs/v3@latest
 ```

2. Add it as import

```diff
 import (
+  docs "github.com/urfave/cli-docs/v3"
 )
```

3. Now use it e.g. to generate markdown docu from a command

```go
func main() {
    app := newApp()
    md, err := docs.ToMarkdown(app)
    if err != nil {
        panic(err)
    }

    fi, err := os.Create("cli-docs.md")
    if err != nil {
        panic(err)
    }
    defer fi.Close()
    if _, err := fi.WriteString("# CLI\n\n" + md); err != nil {
        panic(err)
    }
}
```
