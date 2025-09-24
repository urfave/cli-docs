## CLI interface - greet

Description of the application.

Some app.

> app [first_arg] [second_arg]

Usage:

```bash
$ app [GLOBAL FLAGS] [COMMAND] [COMMAND FLAGS] [ARGUMENTS...]
```

Global flags:

| Name                        | Description        | Type   | Default value |  Environment variables  |
|-----------------------------|--------------------|--------|:-------------:|:-----------------------:|
| `--socket="…"` (`-s`)       | some 'usage' text  | string |    `value`    |         *none*          |
| `--flag="…"` (`--fl`, `-f`) |                    | string |               |         *none*          |
| `--another-flag` (`-b`)     | another usage text | bool   |    `false`    | `EXAMPLE_VARIABLE_NAME` |

### `config` command (aliases: `c`)

another usage test.

Usage:

```bash
$ app [GLOBAL FLAGS] config [COMMAND FLAGS] [ARGUMENTS...]
```

The following flags are supported:

| Name                        | Description        | Type   | Default value | Environment variables |
|-----------------------------|--------------------|--------|:-------------:|:---------------------:|
| `--flag="…"` (`--fl`, `-f`) |                    | string |               |        *none*         |
| `--another-flag` (`-b`)     | another usage text | bool   |    `false`    |        *none*         |

### `config sub-config` subcommand (aliases: `s`, `ss`)

another usage test.

Usage:

```bash
$ app [GLOBAL FLAGS] config sub-config [COMMAND FLAGS] [ARGUMENTS...]
```

The following flags are supported:

| Name                                | Description     | Type   | Default value | Environment variables |
|-------------------------------------|-----------------|--------|:-------------:|:---------------------:|
| `--sub-flag="…"` (`--sub-fl`, `-s`) |                 | string |               |        *none*         |
| `--sub-command-flag` (`-s`)         | some usage text | bool   |    `false`    |        *none*         |

### `info` command (aliases: `i`, `in`)

retrieve generic information.

Usage:

```bash
$ app [GLOBAL FLAGS] info [ARGUMENTS...]
```

### `some-command` command

Usage:

```bash
$ app [GLOBAL FLAGS] some-command [ARGUMENTS...]
```

### `usage` command (aliases: `u`)

standard usage text.

> Usage for the usage text
> - formatted:  Based on the specified ConfigMap and summon secrets.yml
> - list:       Inspect the environment for a specific process running on a Pod
> - for_effect: Compare 'namespace' environment with 'local'
> ```
> func() { ... }
> ```
> Should be a part of the same code block

Usage:

```bash
$ app [GLOBAL FLAGS] usage [COMMAND FLAGS] [ARGUMENTS...]
```

The following flags are supported:

| Name                        | Description        | Type   | Default value | Environment variables |
|-----------------------------|--------------------|--------|:-------------:|:---------------------:|
| `--flag="…"` (`--fl`, `-f`) |                    | string |               |        *none*         |
| `--another-flag` (`-b`)     | another usage text | bool   |    `false`    |        *none*         |

### `usage sub-usage` subcommand (aliases: `su`)

standard usage text.

> Single line of UsageText

Usage:

```bash
$ app [GLOBAL FLAGS] usage sub-usage [COMMAND FLAGS] [ARGUMENTS...]
```

The following flags are supported:

| Name                        | Description     | Type | Default value | Environment variables |
|-----------------------------|-----------------|------|:-------------:|:---------------------:|
| `--sub-command-flag` (`-s`) | some usage text | bool |    `false`    |        *none*         |
