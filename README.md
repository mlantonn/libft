# Libft
Reproduction of libc functions, addition of new ones.<br />
This was my first school project, don't use it, it's mostly trash.<br />

## Installation

### Unix operating systems
Pull the repository and run `make` inside to compile the library `libft.a`.<br />
```
$ make path/to/repo
```
### Windows and other operating systems
Not implemented.<br />

## Usage
Include the header in your files and compile with library flags.<br />
```C
#include "libft.h"
```
```
$ gcc -L path/to/lib -lft
```

## Functions
### Libc functions
```C
void	*ft_memset(void *p, int c, size_t n);
void	ft_bzero(void *p, size_t n);
void	*ft_memcpy(void *dst, void const *src, size_t n);
void	*ft_memccpy(void *dst, void const *src, int c, size_t n);
void	*ft_memmove(void *dst, void const *src, size_t n);
void	*ft_memchr(void const *s, int c, size_t n);
int	ft_memcmp(void const *s1, void const *s2, size_t n);
size_t	ft_strlen(char const *s);
char	*ft_strdup(char const *src);
char	*ft_strcpy(char *dst, char const *src);
char	*ft_strncpy(char *dst, char const *src, size_t len);
char	*ft_strcat(char *s1, char const *s2);
char	*ft_strncat(char *s1, char const *s2, size_t n);
size_t	ft_strlcat(char *dst, char const *src, size_t size);
char	*ft_strchr(char const *s, int c);
char	*ft_strrchr(char const *s, int c);
char	*ft_strstr(char const *s1, char const *s2);
char	*ft_strnstr(char const *s1, char const *s2, size_t len);
int	ft_strcmp(char const *s1, char const *s2);
int	ft_strncmp(char const *s1, char const *s2, size_t n);
int	ft_atoi(char const *str);
int	ft_isalpha(int c);
int	ft_isdigit(int c);
int	ft_isalnum(int c);
int	ft_isascii(int c);
int	ft_isprint(int c);
int	ft_toupper(int c);
int	ft_tolower(int c);
```
### Original functions
```C
void	*ft_memalloc(size_t size);
void	ft_memdel(void **ap);
char	*ft_strnew(size_t size);
void	ft_strdel(char **as);
void	ft_strclr(char *s);
void	ft_striter(char *s, void (*f)(char *));
void	ft_striteri(char *s, void (*f)(unsigned int, char *));
char	*ft_strmap(char const *s, char (*f)(char));
char	*ft_strmapi(char const *s, char (*f)(unsigned int, char));
int	ft_strequ(char const *s1, char const *s2);
int	ft_strnequ(char const *s1, char const *s2, size_t n);
char	*ft_strsub(char const *s, unsigned int start, size_t len);
char	*ft_strjoin(char const *s1, char const *s2);
char	*ft_strtrim(char const *s);
char	**ft_strsplit(char const *s, char c);
char	*ft_itoa(int n);
void	ft_putchar(char c);
void	ft_putstr(char const *s);
void	ft_putendl(char const *s);
void	ft_putnbr(int n);
void	ft_putchar_fd(char c, int fd);
void	ft_putstr_fd(char const *s, int fd);
void	ft_putendl_fd(char const *s, int fd);
void	ft_putnbr_fd(int n, int fd);
```
### List functions
```C
t_list	*ft_lstnew(void const *content, size_t content_size);
void	ft_lstdelone(t_list **alst, void (*del)(void *, size_t));
void	ft_lstdel(t_list **alst, void (*del)(void *, size_t));
void	ft_lstadd(t_list **alst, t_list *new);
void	ft_lstiter(t_list *lst, void (*f)(t_list *elem));
t_list	*ft_lstmap(t_list *lst, t_list *(*f)(t_list *elem));
```
### Bonus functions
```C
char	*ft_strndup(char const *src, size_t n);
void	*ft_realloc(void *ptr, size_t old, size_t size);
void	ft_showarr(char **tab);
void	ft_arrdel(char ***tab);
char	*ft_read_fd(int fd);
```
### Functions added after submitting project
```C
long long	ft_atoi_base(char const *s, int b);
double		ft_pow(double x, int n);
int		ft_abs(int nb);
void		ft_putnbr_endl(int n);
double		ft_atof(char const *str);
char		**ft_split_white_spaces(char *str);
```
