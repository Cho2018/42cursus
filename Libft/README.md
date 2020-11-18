# Libft
1. Libc functions</br>
      ✅ memset</br>
      ✅ bzero
      - [x] memcpy
      - [x] memccpy
      - [x] memmove
      - [x] memchr
      - [x] memcmp</br>
      ✅ atoi
      - [x] calloc
      - [x] strdup</br>
      ✅ strlen
      - [x] strlcpy
      - [x] strlcat</br>
      ✅ strchr
      - [x] strrchr
      - [x] strnstr
      - [x] strncmp</br>
      ✅ isalpha</br>
      ✅ isdigit</br>
      ✅ isalnum</br>
      ✅ isascii</br>
      ✅ isprint</br>
      ✅ toupper</br>
      ✅ tolower
      </br></br>
2. Additional functions</br>
      - [x] ft_substr
      - [x] ft_strjoin
      - [x] ft_strtrim
      - [x] ft_split
      - [x] ft_itoa
      - [x] ft_strmapi</br>
      ✅ ft_putchar_fd</br>
      ✅ ft_putstr_fd</br>
      ✅ ft_putendl_fd</br>
      ✅ ft_putnbr_fd
</br></br>
---
### man
1. memset : 주어진 길이만큼 주어진 값으로 채움
</br>b is interpreted as arrays of unsigned char
</br>c is interpreted as unsigned char
2. bzero : 주어진 길이만큼 0으로 채움
</br>s is interpreted as arrays of unsigned char
3. toupper : 소문자를 대문자로 (글자 아니면 패스)
4. tolower : 대문자를 소문자로 (글자 아니면 패스)
5. atoi : 스트링을 int로 변환
</br>ex) number / sign | number / whitespace | number / whitespace | sign | number
6. strlen : 스트링 길이 반환
7. strchr : 스트링에서 c가 처음으로 나오는 포인터 반환
8. isalpha : 알파벳인지 확인
9. isdigit : 숫자인지 확인
10. isalnum : 알파벳이나 숫자인지 확인
11. isascii : 아스키 문자인지 확인
12. isprint : 프린트 가능인지 확인
---
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
