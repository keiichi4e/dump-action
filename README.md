# dump-action
GitHub Actions to dump environments and context.

## Usage

```yml
name: Dump
on: push
jobs:
  debug:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: keiichi4e/dump-action@main
        id: dump
        with:
          enable-context: 'true'
```
