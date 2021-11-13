# parallely: Run commands in parallel while saving and summarizing command results.

<!--
EDIT README.template.md, not README.md directly.
Use `make build-readme to update the README file
-->

## Usage

```
<HELP_STRING>
```

## Installation

### Option 1:

1. Download [raw.githubusercontent.com/roguh/parallely/main/parallely](https://raw.githubusercontent.com/roguh/parallely/main/parallely).
2. Make executable and move to your preferred binary location.

```
chmod +x parallely
sudo cp parallely /usr/bin/parallely
```

### Option 2:

```
git clone https://github.com/roguh/parallely.git
cd parallely
make install
```

OR

```
git clone https://github.com/roguh/parallely.git
cd parallely
make install-to-user
```

OR

```
git clone https://github.com/roguh/parallely.git
cd parallely
make install-symlink-to-user
```

<!-- TODO
## Integration Testing

If the test script fails, the tests have failed.
Also read the output to determine if `parallely` is behaving correctly.

Note the `test-integration-all-shells.sh` script runs the `test-integration.sh` script using the test shell itself.

### Linux: Running tests for many shells at once

```
make test-on-linux
```

### MacOS: Running tests for many shells at once

```
make test-on-macos
```

### Running tests for stricter POSIX shells

```
make test-on-strict-posix-shells
```

### Running tests one shell at a time

Run the following commands:

```
./tests/test-integration.sh sh
./tests/test-integration.sh dash
./tests/test-integration.sh bash
BASH_COMPAT=31 ./tests/test-integration.sh bash
./tests/test-integration.sh zsh
```

### Test results

### Linux

Tested using GNU coreutils 9.0 in these shells:

- dash 0.5
- bash 5.1
- bash 5.1 in bash 3.1 compatibility mode BASH_COMPAT=31
- zsh 5.8
- yash 2.52
- ksh version 2020.0.0

### MacOS

Not tested on MacOS, yet. It should work fine.
-->

## Linting and Compatibility Check

Use shellcheck to check shellscripts.

```
make check
```