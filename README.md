# Makefiles for newbies

[Source](https://habr.com/ru/post/155201/)

## Manual compilation

```bash
g++ main.cpp hello.cpp factorial.cpp -o hello
```

## Anatomy of a Makefile

```text
target: dependencies
[tab] command

# This is a comment

# Defining a variable
KEY=value

# Using a variable
blah-blah $(KEY)
```

## How to build

```bash
make -f ${PATH_TO_MAKEFILE}
```

Makefiles:

- Makefile-1 - the simplest Makefile, which contains the only one target
- Makefile-2 - this Makefile contains multiple targets with its dependencies
- Makefile-3 - more advanced version with variables and comments
- Makefile-4 - more universal Makefile
