# with-env

Run any arbitrary command with a `.env` file.

## Why?

`with-env` eliminates the need to load environment variables from a file within your program, eliminating calls that are redundant to production, and separating environment management from the code itself.

## Usage

```sh
with-env <command>
```

Requires a `.env` file in your current working directory.

## Example

### `.env` File (in current working directory)

```
# .env
FOO='bar'
```

### Command

```sh
$ with-env printenv FOO
bar
```
