# fakegcc

Thes are shell scripts to fake [Homebrew](https://brew.sh) into thinking `gcc` is installed.

Copy one of these to `/usr/bin/gcc` and then Homebrew thinks `gcc` is installed and won't ask to install it. This is useful when installing only bottles or formula that do not need compilation. Without this, installing a formula shows an error, even when no compilation is required:

```
Error: An exception occurred within a child process:
  CompilerSelectionError: <formula> cannot be built with any available compilers.
Install Clang or run `brew install gcc`.
```

Installing a compiler on a Linux server is not always desirable.

## Version Mapping


| Operating System       | `fakegcc` Version |
| ---------------------- | ----------------- |
| Ubuntun 16.04 (xenial) | `fakegcc-5`       |
| Ubuntun 18.04 (bionic) | `fakegcc-7`       |
