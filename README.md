<a href="#" onclick="return false;"><img alt="42 Logo" src="https://github.com/unisraporelmundo/unisraporelmundo/blob/main/unisraporelmundo/libftbanner.gif"></a>

El primer proyecto en 42, libft, consiste en aprender cómo funcionan las funciones estándar de la programación C escribiéndolas desde cero y creando una biblioteca personal. Este proyecto es vital ya que la biblioteca se utilizará en asignaciones futuras en 42.
Tendrás que programar una [librería](https://github.com/unisraporelmundo/libft/tree/main) en C. Tu librería tendrá un montón de funciones de propósito general en las que se apoyarán tus programas.

[Click aquí](https://github.com/unisraporelmundo/libft/blob/main/es.subject.pdf) para ver el `PDF` del proyecto


# Libft - Tu Primera Biblioteca en C

Libft es un proyecto que desafía a los estudiantes a crear su propia biblioteca de funciones en C, replicando y expandiendo las funcionalidades de la libc estándar. Este es uno de los primeros proyectos dentro del currículo de 42 y sirve como una base sólida para entender y aplicar conceptos fundamentales de programación en C.

## 📘 Resumen del Proyecto

Este proyecto consiste en codificar una biblioteca en C que incluirá un conjunto de funciones de propósito general. Estas funciones serán utilizadas en proyectos posteriores, facilitando el desarrollo de programas más complejos.

## 📄 Instrucciones Generales

- **Lenguaje:** Todo el proyecto debe estar escrito en C.
- **Normativa:** Seguir la normativa de codificación de 42, que incluye la prohibición de variables globales y el uso de `static` para funciones internas.
- **Compilación:** Debe incluirse un Makefile que compilará los archivos fuente con las flags `-Wall`, `-Werror` y `-Wextra`.
- **Seguridad:** No deben producirse fallos abruptos (segfault, bus error, etc.) y toda la memoria asignada debe liberarse adecuadamente.

## 🏗️ Parte Obligatoria

### Funciones de libc

Replicarás funciones estándar de la libc, como `strlen`, `memset`, y `memcpy`, pero con el prefijo `ft_` para denotar que son implementaciones propias.

Debes rehacer las siguientes funciones de la libc con el prefijo `ft_`:

| Función                         | Descripción                                                                     | Prototipo                                                                        |
| -------------------------------- | ----------------------------------------------------------- |-------------------------------------------------------------|                                               
| [ft_isalpha](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_isalpha.c) | Verifica si el carácter `c` es alfabético.                                          | int ft_isalpha(int c);                                                           |
| [ft_isdigit](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_isdigit.c) | Verifica si el carácter `c` es un dígito numérico.                                     | int ft_isdigit(int c);                                                           |
| [ft_isalnum](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_isalnum.c) | Verifica si el carácter `c` es alfanumérico.                                        | int ft_isalnum(int c);                                                           |
| [ft_isascii](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_isascii.c) | Verifica si el carácter `c` es un carácter ASCII.                                  | int ft_isascii(int c);                                                           |
| [ft_isprint](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_isprint.c) | Verifica si el carácter `c` es imprimible.                                           | int ft_isprint(int c);                                                           |
| [ft_strlen](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_strlen.c)   | Calcula la longitud de la cadena `str`.                                        | int ft_strlen(char *str);                                                        |
| [ft_memset](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_memset.c)   | Llena los primeros `size` bytes de `str` con el byte `c`.                        | char *ft_memset(char *str, char c, size_t size);                                 |
| [ft_bzero](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_bzero.c)     | Establece los primeros `size` bytes de `str` a cero.                                   | void ft_bzero(char *str, size_t n);                                              |
| [ft_memcpy](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_memcpy.c)   | Copia `size` bytes de `src` a `dest`.                                       | void *ft_memcpy(void *dest, const void *src, size_t size);                       |
| [ft_memmove](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_memmove.c) | Copia `size` bytes de `src` a `dest`, incluso si se superponen.                 | void *ft_memmove(void *dest, const void *src, size_t size);                      |
| [ft_strlcpy](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_strlcpy.c) | Copia hasta `size` caracteres de `src` a `dest`.                            | size_t ft_strlcpy(char *dest, const char *src, size_t size);                     |
| [ft_strlcat](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_strlcat.c) | Anexa `src` a `dest` hasta alcanzar `size`.                                  | size_t ft_strlcat(char *dst, const char *src, size_t size);                      |
| [ft_toupper](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_toupper.c) | Convierte el carácter `c` a mayúsculas si es minúsculas.                          | int ft_toupper(int c);                                                           | 
| [ft_tolower](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_tolower.c) | Convierte el carácter `c` a minúsculas si es mayúsculas.                          | int ft_tolower(int c);                                                           |
| [ft_strchr](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_strchr.c)   | Localiza la primera ocurrencia de `c` en `str`.                                   | char *ft_strchr(const char *s, int c);                                           |
| [ft_strrchr](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_strrchr.c) | Localiza la última ocurrencia de `c` en `str`.                                   | char *ft_strrchr(const char *s, int c);                                           |
| [ft_strncmp](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_strncmp.c) | Compara los primeros `size` caracteres de `s1` y `s2`.                          | int ft_strncmp(const char *s1, const char *s2, size_t size);                     |
| [ft_memchr](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_memchr.c)   | Localiza la primera ocurrencia de `c` en `str` dentro de un máximo de `size` bytes.  | void *ft_memchr(const void *str, int c, size_t size);                            |
| [ft_memcmp](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_memcmp.c)   | Compara los primeros `size` bytes de `s1` y `s2`.                               | int ft_memcmp(const void *s1, const void *s2, size_t size);                      |
| [ft_strnstr](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_strnstr.c) | Localiza la primera ocurrencia de `needle` en `haystack` dentro de un máximo de `size` bytes. | char *ft_strnstr(const char *haystack, const char *needle, size_t size);|
| [ft_atoi](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_atoi.c)       | Convierte una cadena en un entero.                                                | int ft_atoi(const char *str);                                                    |
| [ft_calloc](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20principales/ft_calloc.c)   | Asigna memoria y la llena con ceros.                                       | void *ft_calloc(size_t nmemb, size_t size);                                      |
| [ft_strdup](https://github.com/unisraporelmundo/libft/blob

/main/Funciones%20principales/ft_strdup.c)   | Duplica una cadena dinámica.                                                     | char *ft_strdup(const char *s1);                                                 |

### Funciones adicionales

Crearás funciones que no se encuentran en la libc o que ofrecen funcionalidades extendidas, tales como `ft_substr` y `ft_split`.

| Función                         | Descripción                                                                     | Prototipo                                                                        |
| -------------------------------- | ------------------------------------------------------------------------------- |--------------------------------------------------------------------------------- |
| [ft_substr](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_substr.c)   | Extrae una subcadena de una cadena.                                             | char *ft_substr(const char *s, unsigned int start, size_t len);                  |
| [ft_strjoin](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_strjoin.c) | Concatena dos cadenas en una nueva.                                        | char *ft_strjoin(const char *s1, const char *s2);                                |
| [ft_strtrim](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_strtrim.c) | Elimina caracteres especificados del principio y final de una cadena.            | char *ft_strtrim(const char *s1, const char *set);                               |
| [ft_split](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_split.c)     | Divide una cadena en palabras.                                                     | char **ft_split(const char *s, char c);                                          |
| [ft_itoa](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_itoa.c)       | Convierte un entero a una cadena.                                                | char *ft_itoa(int n);                                                            |
| [ft_strmapi](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_strmapi.c) | Aplica una función a cada carácter de una cadena.                               | char *ft_strmapi(const char *s, char (*f)(unsigned int, char));                  |
| [ft_striteri](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_striteri.c)| Aplica una función a cada carácter de una cadena, con su índice.              | void ft_striteri(char *s, void (*f)(unsigned int, char*));                       |
| [ft_putchar_fd](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_putchar_fd.c)| Escribe un carácter en un descriptor de archivo.                                   | void ft_putchar_fd(char c, int fd);                                              |
| [ft_putstr_fd](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_putstr_fd.c) | Escribe una cadena en un descriptor de archivo.                                       | void ft_putstr_fd(char *s, int fd);                                              |
| [ft_putendl_fd](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_putendl_fd.c)| Escribe una cadena seguida de un salto de línea en un descriptor de archivo.                | void ft_putendl_fd(char *s, int fd);                                             |
| [ft_putnbr_fd](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20adicionales/ft_putnbr_fd.c)   | Escribe un entero en un descriptor de archivo.                                   | void ft_putnbr_fd(int n, int fd);                                                |

## 🔨 Makefile

El Makefile incluirá reglas como `all`, `clean`, `fclean`, y `re` para gestionar eficientemente la compilación de la biblioteca.

## 🚀 Parte Bonus

Si completas la parte obligatoria con éxito, puedes proceder a implementar funciones adicionales que manejen estructuras de datos como listas enlazadas.

### Funciones Bonus

| Función                         | Descripción                                                                     | Prototipo                                                                        |
| -------------------------------- | ------------------------------------------------------------------------------- |--------------------------------------------------------------------------------- |
| [ft_lstnew_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstnew_bonus.c) | Crea un nuevo elemento de la lista. | t_list *ft_lstnew(void *content); |
| [ft_lstadd_front_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstadd_front_bonus.c) | Añade un nuevo elemento al principio de la lista. | void ft_lstadd_front(t_list **lst, t_list *new); |
| [ft_lstsize_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstsize_bonus.c) | Obtiene el número de elementos en una lista. | int ft_lstsize(t_list *lst); |
| [ft_lstlast_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstlast_bonus.c) | Obtiene el último elemento de una lista. | t_list *ft_lstlast(t_list *lst); |
| [ft_lstadd_back_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstadd_back_bonus.c) | Añade un nuevo elemento al final de una lista. | void ft_lstadd_back(t_list **lst, t_list *new); |
| [ft_lstdelone_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstdelone_bonus.c) | Elimina un nodo de una lista sin eliminar su contenido. | void ft_lstdelone(t_list *lst, void (*del)(void *)); |
| [ft_lstclear_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstclear_bonus.c) | Elimina y libera la memoria de un nodo de la lista y sus consecutivos. | void ft_lstclear(t_list **lst, void (*del)(void *)); |
| [ft_lstiter_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstiter_bonus.c) | Aplica una función a cada elemento de una lista. | void ft_lstiter(t_list *lst, void (*f)(void *)); |
| [ft_lstmap_bonus](https://github.com/unisraporelmundo/libft/blob/main/Funciones%20Bonus/ft_lstmap_bonus.c) | Crea una lista iterando y aplicando una función a una lista existente. | t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *)); |

## 📚 Apuntes

[Click aquí](https://github.com/unisraporelmundo/unisraporelmundo/blob/main/unisraporelmundo/LIBFT%20%20APUNTES%20ISRAEL.pdf) para ver el `PDF` con mis apuntes del proyecto.

