# install-cfn-lookup-action

Composite run steps action for installing [fujiwara/cfn-lookup](https://github.com/fujiwara/cfn-lookup).

## Usage

Action cohalz/install-cfn-lookup-action@v1 installs cfn-lookup binary for Linux into /usr/local/bin. This action runs install only.

Pass the parameter "latest" to use the latest version of cfn-lookup.



```yml
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: cohalz/install-cfn-lookup-action@v1
        with:
          version: v0.0.2 # or latest
```
