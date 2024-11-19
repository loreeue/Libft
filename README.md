## Libft
**Libft** es un proyecto desarrollado en 42 Madrid. Consiste en crear una librería personalizada en C que incluye diversas funciones de propósito general. El objetivo es implementar desde cero funciones estándar de la biblioteca libc y otras utilidades adicionales, sin depender de implementaciones externas

![Logo 42 Madrid](42-Madrid.jpeg)

### PARTE OBLIGATORIA
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

### FUNCIONES ADICIONALES
- ft_substr: Reserva (con malloc(3)) y devuelve una substring de la string ’s’. La substring empieza desde el índice ’start’ y tiene una longitud máxima ’len’.
- ft_strjoin: Reserva (con malloc(3)) y devuelve una nueva
string, formada por la concatenación de ’s1’ y ’s2’.
- ft_strtrim: Elimina todos los caracteres de la string ’set’
desde el principio y desde el final de ’s1’, hasta
encontrar un caracter no perteneciente a ’set’. La
string resultante se devuelve con una reserva de
malloc(3).
- ft_split: Reserva (utilizando malloc(3)) un array de strings
resultante de separar la string ’s’ en substrings
utilizando el caracter ’c’ como delimitador. El
array debe terminar con un puntero NULL.
- ft_itoa: Utilizando malloc(3), genera una string que
represente el valor entero recibido como argumento.
Los números negativos tienen que gestionarse.
- ft_strmapi: Aplica la función ’f’ a cada carácter de la cadena
’s’, pasando su índice como primer argumento y el
propio carácter como segundo argumento. Se crea una
nueva cadena (utilizando malloc(3)) para recoger
los resultados de las sucesivas aplicaciones de
’f’.
- ft_striteri: A cada carácter de la string ’s’, aplica la función
’f’ dando como parámetros el índice de cada
carácter dentro de ’s’ y la dirección del propio
carácter, que podrá modificarse si es necesario.
- ft_putchar_fd: Envía el carácter ’c’ al file descriptor
especificado.
- ft_putstr_fd: Envía la string ’s’ al file descriptor
especificado.
- ft_putendl_fd: Envía la string ’s’ al file descriptor dado,
seguido de un salto de línea.
- ft_putnbr_fd: Envía el número ’n’ al file descriptor dado.

```
typedef struct s_list
{
	*content;
	*next;
}	t_list;
```

### PARTE BONUS
- ft_lstnew: Crea un nuevo nodo utilizando malloc(3). La
variable miembro ’content’ se inicializa con el
contenido del parámetro ’content’. La variable
’next’, con NULL.
- ft_lstadd_front: Añade el nodo ’new’ al principio de la lista ’lst’.
- ft_lstsize: Cuenta el número de nodos de una lista.
- ft_lstlast: Devuelve el último nodo de la lista.
- ft_lstadd_back: Añade el nodo ’new’ al final de la lista ’lst’.
- ft_lstdelone: Toma como parámetro un nodo ’lst’ y libera la
memoria del contenido utilizando la función ’del’ dada como parámetro, además de liberar el nodo. La memoria de ’next’ no debe liberarse.
- ft_lstclear: Elimina y libera el nodo ’lst’ dado y todos los
consecutivos de ese nodo, utilizando la función ’del’ y free(3). Al final, el puntero a la lista debe ser NULL.
- ft_lstiter: Itera la lista ’lst’ y aplica la función ’f’ en el
contenido de cada nodo.
- ft_lstmap: Itera la lista ’lst’ y aplica la función ’f’ al
contenido de cada nodo. Crea una lista resultante
de la aplicación correcta y sucesiva de la función
’f’ sobre cada nodo. La función ’del’ se utiliza
para eliminar el contenido de un nodo, si hace
falta.

### Aclaración

Este proyecto sigue los estándares de la **Norma de 42**.
