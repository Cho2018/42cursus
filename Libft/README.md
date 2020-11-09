# Libft
1. Libc functions</br>
      - [x] memset
      - [x] bzero
      - [x] memcpy
      - [x] memccpy
      - [x] memmove
      - [x] memchr
      - [x] memcmp
      - [x] atoi
      - [x] calloc
      - [x] strdup
      - [x] strlen
      - [x] strlcpy
      - [x] strlcat
      - [x] strchr
      - [x] strrchr
      - [x] strnstr
      - [x] strncmp
      - [x] isalpha
      - [x] isdigit
      - [x] isalnum
      - [x] isascii
      - [x] isprint
      - [x] toupper
      - [x] tolower</br></br>
2. Additional functions</br>
      - [x] ft_substr
      - [x] ft_strjoin
</br></br>
---
### man
1. memccpy</br> 
- copy string until character found
- void *memccpy(void *restrict dst, const void *restrict src, int c, size_t n);
- copies bytes from string src to string dst
- If the character c (as converted to an unsigned char) occurs in the string src, the copy stops and a pointer to the byte after the copy of c in the string dst is returned
- Otherwise, n bytes are copied, and a NULL pointer is returned

2. memmove</br>
- copy byte string
- void *memmove(void *dst, const void *src, size_t len);
- copies len bytes from string src to string dst
- The two strings may overlap; the copy is always done in a non-destructive manner
- return : the original value of dst

3. memchr</br>
- locate byte in byte string
- void *memchr(const void *s, int c, size_t n);
- locates the first occurence of c (converted to an unsigned char) in string s
- return : a pointer to the byte located, or NULL if no such byte exists within n bytes

4. memcmp</br>
- compare byte string
- int memcmp(const void *s1, const void *s2, size_t n);
- compares byte string s1 against byte string s2
- both strings are assumed to be n bytes long
- return : zero if the two strings are identical
- Otherwise returns the difference between the first two differing bytes (treated as unsigned char values)
- zero-length strings are always identical

5. atoi</br>
- convert ascii string to integer
- int atoi(const char *str);
- converts the initial portion of the string pointed to by str to int representation

6. calloc</br>
- memory allocation
- void *calloc(size_t count, size_t size);
- contiguously allocates enough space for count objects that are size bytes of memory each and returns a pointer to the allocated memory
- The allocated memory is filled with bytes of value zero

7. strdup</br>
- save a copy of a string
- char *strdup(const char *s1);
- allocates sufficient memory for a copy of the string s1, does the copy, and returns a pointer to it
- If insufficient memory is available, NULL is returned and errno is set to ENOMEM
