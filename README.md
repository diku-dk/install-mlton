# Install MLton

This action installs MLton in a Linux-based GitHub Actions runner.
The compiler is installed in `$HOME/.local`, which means it will be on
the `$PATH` of a standard setup.

Currently always installs the `amd64-linux-glibc2.31` binaries.  Feel
free to issue a Pull Request if you need something else.

## Inputs

`version`

The full version to install as a string (e.g. `'20210117'`), or the
string `'latest'`.

## Example usages

```
      - uses: diku-dk/install-mlton@v1
        with:
          version: '20210107'
```

```
      - uses: diku-dk/install-mlton@v1
```

```
      - uses: diku-dk/install-mlton@v1
        with:
          version: 'latest'
```
