# gocov2lcov-action
A multi-arch and multi-OS capable gcov2lcov action runner

## Inputs

- `ARCH`: `amd64` or `arm64`
- `OS`: `linux`, `windows`, `freebsd`, or `darwin`
- `INFILE`: path to the Go coverage file to convert
- `OUTFILE`: output path for the generated LCOV file
- `VERSION`: optional upstream release tag to download (defaults to `v1.1.1`)

## Example

```yaml
- uses: twitchel/gocov2lcov-action@v1
  with:
    ARCH: amd64
    OS: linux
    INFILE: coverage.out
    OUTFILE: coverage.lcov
```
