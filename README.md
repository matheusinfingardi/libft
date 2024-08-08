# **LIBFT**

## 📋 Overview

This project is about coding a C library.Libft is a project focused on creating a personal C library. It involves implementing various general-purpose functions from scratch, providing a hands-on challenge in understanding and ensuring the proper functionality of each component.

## ☑️ Common Instructions

-   **Language and Norm Compliance:** The project must be written in C and adhere strictly to the Norm. Any bonus files/functions are included in the Norm check, and non-compliance will result in a zero grade.
    
-   **Error Handling:** Functions should not cause unexpected terminations such as segmentation faults, bus errors, or double frees. Projects exhibiting such errors will be deemed non-functional and will receive a zero during evaluation.
    
-   **Memory Management:** All dynamically allocated memory must be properly freed. Memory leaks are not tolerated.
    
-   **Makefile Requirements:** If applicable, include a Makefile that compiles source files with the flags `-Wall`, `-Wextra`, and `-Werror` using `cc`. The Makefile must contain the rules `$(NAME)`, `all`, `clean`, `fclean`, and `re`. It should not relink.
    
-   **Bonus Files:** For projects with a bonus section, include a `bonus` rule in the Makefile. Bonus files must be separated into a `_bonus.{c/h}` file if not specified otherwise. Mandatory and bonus parts are evaluated separately.
    
-   **Library Usage:** If the project requires using `libft`, place its sources and Makefile in a `libft` folder. Your project’s Makefile should compile the library first using its own Makefile, then compile the project.
    
-   **Testing:** Creating test programs is encouraged for validating your work. While these tests are not graded, they are useful for personal verification and during project defense.
    
-   **Submission:** Submit your work to the assigned Git repository. Only the content within the repository will be graded. Any errors detected during grading by Deepthought will result in the evaluation being halted.

## 📋 Mandatory Part

-   **Program Name:** `libft.a`
-   **Required Files:** `Makefile`, `libft.h`, and `ft_*.c` files.
-   **Makefile Rules:** Must include rules for `NAME`, `all`, `clean`, `fclean`, and `re`.
-   **External Functions:** Use external functions as detailed below.
-   **Libft Authorization:** Not applicable.
-   **Description:** Develop a personal library containing a collection of useful functions. This library will serve as a valuable tool throughout your curriculum.

## 📋 Features

### Libc Functions

In this part, you will reimplement a set of standard libc functions. These functions should follow the prototypes and behaviors defined in their man pages, with the only difference being their names, which should start with `ft_`. Functions that use the `restrict` qualifier from the C99 standard should be implemented without it.

#### Functions to Implement:

-   **isalpha**: `int ft_isalpha(int c);`
-   **isdigit**: `int ft_isdigit(int c);`
-   **isalnum**: `int ft_isalnum(int c);`
-   **isascii**: `int ft_isascii(int c);`
-   **isprint**: `int ft_isprint(int c);`
-   **strlen**: `size_t ft_strlen(const char *s);`
-   **memset**: `void *ft_memset(void *b, int c, size_t len);`
-   **bzero**: `void ft_bzero(void *s, size_t len);`
-   **memcpy**: `void *ft_memcpy(void *dest, const void *src, size_t n);`
-   **memmove**: `void *ft_memmove(void *dest, const void *src, size_t len);`
-   **strlcpy**: `size_t ft_strlcpy(char *dst, const char *src, size_t dstsize);`
-   **strlcat**: `size_t ft_strlcat(char *dst, const char *src, size_t dstsize);`
-   **toupper**: `int ft_toupper(int c);`
-   **tolower**: `int ft_tolower(int c);`
-   **strchr**: `char *ft_strchr(const char *s, int c);`
-   **strrchr**: `char *ft_strrchr(const char *s, int c);`
-   **strncmp**: `int ft_strncmp(const char *s1, const char *s2, size_t n);`
-   **memchr**: `void *ft_memchr(const void *s, int c, size_t n);`
-   **memcmp**: `int ft_memcmp(const void *s1, const void *s2, size_t n);`
-   **strnstr**: `char *ft_strnstr(const char *haystack, const char *needle, size_t len);`
-   **atoi**: `int ft_atoi(const char *str);`

For the following functions, use `malloc()` for memory allocation:

-   **calloc**: `void *ft_calloc(size_t count, size_t size);`
-   **strdup**: `char *ft_strdup(const char *s);`

### Additional Functions

In this section, you will create functions that either extend beyond the libc functions or present them in a different format.

#### Functions to Implement:

-   **ft_substr**
    
    -   **Prototype:** `char *ft_substr(char const *s, unsigned int start, size_t len);`
    -   **Description:** Allocates and returns a substring from the string `s`, starting at index `start` and with a maximum length of `len`.
-   **ft_strjoin**
    
    -   **Prototype:** `char *ft_strjoin(char const *s1, char const *s2);`
    -   **Description:** Allocates and returns a new string which is the result of concatenating `s1` and `s2`.
-   **ft_strtrim**
    
    -   **Prototype:** `char *ft_strtrim(char const *s1, char const *set);`
    -   **Description:** Allocates and returns a copy of `s1` with characters specified in `set` removed from both ends.
-   **ft_split**
    
    -   **Prototype:** `char **ft_split(char const *s, char c);`
    -   **Description:** Allocates and returns an array of strings obtained by splitting `s` using `c` as a delimiter. The array must end with a NULL pointer.
-   **ft_itoa**
    
    -   **Prototype:** `char *ft_itoa(int n);`
    -   **Description:** Allocates and returns a string representing the integer `n`. Handles negative numbers.
-   **ft_strmapi**
    
    -   **Prototype:** `char *ft_strmapi(char const *s, char (*f)(unsigned int, char));`
    -   **Description:** Applies the function `f` to each character of the string `s`, creating a new string with the results.
-   **ft_striteri**
    
    -   **Prototype:** `void ft_striteri(char *s, void (*f)(unsigned int, char*));`
    -   **Description:** Applies the function `f` to each character of the string `s`, passing its index and character by address.
-   **ft_putchar_fd**
    
    -   **Prototype:** `void ft_putchar_fd(char c, int fd);`
    -   **Description:** Outputs the character `c` to the given file descriptor `fd`.
-   **ft_putstr_fd**
    
    -   **Prototype:** `void ft_putstr_fd(char *s, int fd);`
    -   **Description:** Outputs the string `s` to the given file descriptor `fd`.
-   **ft_putendl_fd**
    
    -   **Prototype:** `void ft_putendl_fd(char *s, int fd);`
    -   **Description:** Outputs the string `s` to the given file descriptor `fd`, followed by a newline.
-   **ft_putnbr_fd**
    
    -   **Prototype:** `void ft_putnbr_fd(int n, int fd);`
    -   **Description:** Outputs the integer `n` to the given file descriptor `fd`.

## 💎 Bonus Part 

### Overview

For the bonus part, you'll implement a set of functions to work with linked lists. These functions will build on the mandatory part and provide additional functionality for managing lists. Note that the bonus part will only be evaluated if the mandatory part is perfect and fully functional.

### Functions to Implement

1.  **ft_lstnew**
    
    -   **Prototype:** `t_list *ft_lstnew(void *content);`
    -   **Description:** Allocates and returns a new node with `content` initialized and `next` set to NULL.
2.  **ft_lstadd_front**
    
    -   **Prototype:** `void ft_lstadd_front(t_list **lst, t_list *new);`
    -   **Description:** Adds a new node to the beginning of the list.
3.  **ft_lstsize**
    
    -   **Prototype:** `int ft_lstsize(t_list *lst);`
    -   **Description:** Counts and returns the number of nodes in the list.
4.  **ft_lstlast**
    
    -   **Prototype:** `t_list *ft_lstlast(t_list *lst);`
    -   **Description:** Returns the last node of the list.
5.  **ft_lstadd_back**
    
    -   **Prototype:** `void ft_lstadd_back(t_list **lst, t_list *new);`
    -   **Description:** Adds a new node to the end of the list.
6.  **ft_lstdelone**
    
    -   **Prototype:** `void ft_lstdelone(t_list *lst, void (*del)(void *));`
    -   **Description:** Frees the memory of a node's content and the node itself, using the function `del`.
7.  **ft_lstclear**
    
    -   **Prototype:** `void ft_lstclear(t_list **lst, void (*del)(void *));`
    -   **Description:** Deletes and frees all nodes from the list, setting the list pointer to NULL.
8.  **ft_lstiter**
    
    -   **Prototype:** `void ft_lstiter(t_list *lst, void (*f)(void *));`
    -   **Description:** Iterates through the list, applying function `f` to the content of each node.
9.  **ft_lstmap**
    
    -   **Prototype:** `t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));`
    -   **Description:** Applies function `f` to each node’s content and creates a new list from the results. Uses `del` to free node content if needed.

### Implementation

To complete the bonus part, include the new functions in the `libft.a` archive and update your `Makefile` with a `bonus` rule.

## 📂 Installation & Setup

Instructions for setting up and running the project locally. Include any prerequisites and detailed steps.

## 📜 Code Walkthrough - on Notion

A brief description of the code structure and important components. Include links to specific files or sections of code on GitHub.

-   **File/Function 1:** Description of what it does.
-   **File/Function 2:** Description of what it does.

## 🧩 Challenges & Solutions - on Website

Discuss any significant challenges you faced and how you overcame them.

## 🔗 Links
-   Notion Documentation
-   Website

## 🧑‍💻 Contact

For any questions or inquiries, feel free to contact me:

-   **LinkedIn:**
-   **Email:**
