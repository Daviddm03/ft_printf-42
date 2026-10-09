# ft_printf

A custom implementation of the C `printf` function, developed as part of the 42 curriculum.

The project focuses on variadic functions and formatted output while recreating some of the most commonly used `printf` conversions.

## Supported Conversions

The implementation handles:

| Conversion | Output |
| --- | --- |
| `%c` | Character |
| `%s` | String |
| `%p` | Pointer address |
| `%d` / `%i` | Signed decimal integer |
| `%u` | Unsigned decimal integer |
| `%x` | Lowercase hexadecimal |
| `%X` | Uppercase hexadecimal |
| `%%` | Percent sign |

## Getting Started

### Requirements

- GCC or Clang
- Make
- A Unix-like environment

Clone and compile:

```bash
git clone git@github.com:Daviddm03/ft_printf-42.git
cd ft_printf-42
make
```

The Makefile generates:

```text
libftprintf.a
```

Other commands:

```bash
make clean
make fclean
make re
```

## Usage

Include the header:

```c
#include "ft_printf.h"
```

Example:

```c
int main(void)
{
    ft_printf("Hello %s! Number: %d\n", "world", 42);
    return (0);
}
```

Compile it with the library:

```bash
cc main.c libftprintf.a -o test
./test
```

## What I Learned

This project introduced me to variadic functions and gave me a better understanding of how formatted output can be parsed and handled internally.

It also required working with different data types and converting values to decimal, hexadecimal, and pointer representations.

## Tech

C · Variadic Functions · Makefile · Static Libraries
