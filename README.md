# gocov2lcov-action
A multi-arch and multi-OS capable gocov2lcov action runner

## Inputs

- `ARCH`: `amd64` or `arm64`
- `OS`: `linux`, `windows`, `freebsd`, or `darwin`
- `INFILE`: path to the Go coverage file to convert
- `OUTFILE`: output path for the generated LCOV file

## Example

```yaml
- uses: twitchel/gocov2lcov-action@main
  with:
    ARCH: amd64
    OS: linux
    INFILE: coverage.out
    OUTFILE: coverage.lcov
```
