# Libft
>"The aim of this project is to code a C library regrouping usual functions that you’ll be allowed to use in all your other projects."

## 💡 Mandatory part

### Libc functions

- **memory** : `memset` `bzero` `memcpy` `memccpy` `memmove` `memchr` `memcmp` `calloc`

- **string** : `strlen` `strlcpy` `strlcat` `strchr` `strrchr` `strnstr` `strncmp` `strdup` `atoi`

- **is_sth, to_sth** : `isalpha` `isdigit` `isalnum` `isascii` `isprint` `toupper` `tolower`

### Additional functions

- **string** : `ft_substr` `ft_strjoin` `ft_strtrim` `ft_split` `ft_itoa` `ft_strmapi`

- **put_fd** : `ft_putchar_fd` `ft_putstr_fd` `ft_putendl_fd` `ft_putnbr_fd`

## 💡 Bonus part
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
13. memcpy : copy memory area (src에서 dst로 n 바이트 복사)
14. memccpy : .=. memcpy (src에서 c 발견 시, 복사 멈춤)
15. memmove : .=. memcpy (overlap 따져서 복사 진행) (https://hand-over.tistory.com/47?category=828959)
16. memchr : s에서 c가 처음으로 나오는 위치 (포인터) 반환
17. memcmp : compare byte string
18. calloc
</br>memory allocation
</br>allocates enough space for count objects that are size bytes of memory each
</br>the allocated memory is filled with bytes of value zero
19. strdup : 메모리 할당하고 복사
20. strncmp : compare strings (n만큼만 비교)
21. strnstr : haystack에서 처음으로 needle이 나오는 위치 탐색 (len보다 적게 탐색해야 함) 
22. strrchr : s에서 마지막으로 c가 나오는 위치 탐색
23. strlcpy : 
</br>size-bounded string copying and concatenation
</br>copies up to (dstsize - 1) characters from the string src to dst
</br>dstsize != 0 -> NULL로 끝나도록
</br>return : length of src
24. strlcat : 
</br>size-bounded string copying and concatenation
</br>appends string src to the end of dst
</br>append at most (dstsize - strlen(dst) - 1)
</br>return : 결합되는 문자열의 총 길이 (dstsize < strlen(dst) ? strlen(src) + dstsize : strlen(src) + strlen(dst))
