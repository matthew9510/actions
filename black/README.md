# Black Code Formatter GitHub Action

Adapted from [lgeiger/black-action](https://github.com/lgeiger/black-action]) to
have pinned versions.

A GitHub action that runs [black code formatter](https://github.com/ambv/black) for Python.

## Example Workflow

```workflow
workflow "Example Workflow" {
  on = "push"
  resolves = ["Lint"]
}

action "Lint" {
  uses = "fritzlabs/actions/black@master"
  args = ". --check"
}
```

For a full list of possible `args` checkout the [black docs](https://github.com/ambv/black#command-line-options).
