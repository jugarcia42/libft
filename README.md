# Libft

## About

Libft is a custom C library developed as part of the 42 School curriculum. The purpose of this project is to recreate a selection of standard C library functions and implement additional utility functions that can be reused throughout future projects. This library serves as a foundational toolkit, helping to strengthen core programming concepts such as memory management, string manipulation, data structures, and low-level programming in C.

## Features

### Standard C Library Functions

- Character checks: `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`
- Character conversion: `ft_toupper`, `ft_tolower`
- String manipulation: `ft_strlen`, `ft_strlcpy`, `ft_strlcat`, `ft_strchr`, `ft_strrchr`, `ft_strncmp`, `ft_strnstr`, `ft_strdup`
- Memory management: `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`, `ft_memchr`, `ft_memcmp`, `ft_calloc`
- Conversion functions: `ft_atoi`

### Additional Functions

- `ft_substr`
- `ft_strjoin`
- `ft_strtrim`
- `ft_split`
- `ft_itoa`
- `ft_strmapi`
- `ft_striteri`
- `ft_putchar_fd`
- `ft_putstr_fd`
- `ft_putendl_fd`
- `ft_putnbr_fd`

### Bonus: Linked Lists

- `ft_lstnew`
- `ft_lstadd_front`
- `ft_lstsize`
- `ft_lstlast`
- `ft_lstadd_back`
- `ft_lstdelone`
- `ft_lstclear`
- `ft_lstiter`
- `ft_lstmap`

## Project Structure

```text
libft/
├── includes/
│   └── libft.h
├── src/
│   ├── libc/
│   ├── additional/
│   └── bonus/
├── Makefile
└── README.md
```

## Compilation

Compile the mandatory part:

```bash
make
```

Compile the bonus functions:

```bash
make bonus
```

Available Makefile rules:

```bash
make        # Compile mandatory functions
make bonus  # Compile bonus functions
make clean  # Remove object files
make fclean # Remove object files and library
make re     # Rebuild the project
```

The compilation generates the static library:

```bash
libft.a
```

## Usage

Include the header file in your source code:

```c
#include "libft.h"
```

Compile your project with the library:

```bash
cc main.c libft.a -I includes
```

Example:

```c
#include "libft.h"
#include <stdio.h>

int main(void)
{
    printf("%d\n", ft_atoi("42"));
    return (0);
}
```

## Learning Objectives

Through this project, I gained a deeper understanding of:

- How standard C library functions work internally.
- Dynamic memory allocation and management.
- String and character manipulation.
- Creating reusable and modular code.
- Working with linked lists.
- Building and maintaining static libraries.


Developed as part of the 42 School curriculum.
