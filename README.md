# actions-setup-gcc

[![Test](https://github.com/Dup4/actions-setup-gcc/actions/workflows/test.yml/badge.svg)](https://github.com/Dup4/actions-setup-gcc/actions/workflows/test.yml)


## Usage

Use it in your workflow like this:

```yaml
- name: Set up GCC
    uses: Dup4/actions-setup-gcc@v1
    with:
    version: latest
```

## API

| Input   | Value  | Default | Description                                               |
| ------- | ------ | ------- | --------------------------------------------------------- |
| version | latest | ✓       | Install the latest version available in the repository.   |
|         | *any*  |         | Install a specific version if it's available (see below). |
| cc      | true   | ✓       | Set up `cc`/`gcc`/`c++`/`g++`/`gcov` executables.         |
|         | false  |         | Don't set up the executables.                             |
| env     | true   | ✓       | Set up `CC`/`CXX`/`GCOV` environment variables            |
|         | false  |         | Don't set up the environment variables                    |
