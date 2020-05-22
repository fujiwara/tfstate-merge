# tfstate-merge

A tool to merge tfstate files.

This is pre alpha version. Do not use to production environments.

## Usage

```console
$ tfstate-merge [-i.bak] dest.tfstate src.tfstate
```

tfstate-merge adds resources in src.tfstate into dest.tfstate.

## Requirements

Ruby

## Limitations

- Src and dest tfstate files must have same "version" and "terraform_version".
- Resource addresses must be unique in each state files.
  - Except for data resources which have same attributes.

## LICENSE

MIT
