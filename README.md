# Libft

## Descripción

Libft es el primer proyecto del currículo de 42. El objetivo es recrear una biblioteca de funciones básicas de la librería estándar de C, además de implementar funciones adicionales para trabajar con cadenas de caracteres, memoria y listas enlazadas.

Esta biblioteca servirá como base para futuros proyectos.

## Funciones implementadas

### Funciones de la libc

- ft_isalpha
- ft_isdigit
- ft_isalnum
- ft_isascii
- ft_isprint
- ft_strlen
- ft_memset
- ft_bzero
- ft_memcpy
- ft_memmove
- ft_strlcpy
- ft_strlcat
- ft_toupper
- ft_tolower
- ft_strchr
- ft_strrchr
- ft_strncmp
- ft_memchr
- ft_memcmp
- ft_strnstr
- ft_atoi
- ft_calloc
- ft_strdup

### Funciones adicionales

- ft_substr
- ft_strjoin
- ft_strtrim
- ft_split
- ft_itoa
- ft_strmapi
- ft_striteri
- ft_putchar_fd
- ft_putstr_fd
- ft_putendl_fd
- ft_putnbr_fd

### Funciones Bonus (listas enlazadas)

- ft_lstnew
- ft_lstadd_front
- ft_lstsize
- ft_lstlast
- ft_lstadd_back
- ft_lstdelone
- ft_lstclear
- ft_lstiter
- ft_lstmap

## Compilación

Para compilar la biblioteca:

```bash
make
```

Esto generará el archivo:

```bash
libft.a
```

### Reglas disponibles

```bash
make        # Compila la librería
make bonus  # Compila las funciones bonus
make clean  # Elimina archivos objeto
make fclean # Elimina archivos objeto y la librería
make re     # Recompila todo
```

## Uso

Incluye el header en tu proyecto:

```c
#include "libft.h"
```

Y compila enlazando la biblioteca:

```bash
cc main.c libft.a
```

## Autor

Proyecto realizado como parte del programa de formación de 42.
