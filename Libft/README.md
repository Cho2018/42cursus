# Libft
1. Libc functions</br>
      ✅ memset</br>
      ✅ bzero</br>
      ✅ memcpy</br>
      ✅ memccpy</br>
      ✅ memmove</br>
      ✅ memchr</br>
      ✅ memcmp</br>
      ✅ atoi</br>
      ✅ calloc</br>
      ✅ strdup</br>
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
