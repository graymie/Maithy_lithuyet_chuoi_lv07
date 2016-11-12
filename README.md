# Maithy_lithuyet_chuoi_lv07
# **CHUỖI**
## *1. khái niệm*
- chuỗi là 1 dãy kí tự
- kiểu char
- \0 = null = kết thúc chuỗi.Thực tế, bạn không đặt ký tự null tại vị trí cuối cùng của biến hằng số. Bộ biên dịch C tự động thêm.

## *2.Khai báo*

char ten_chuoi[] ;

hoặc char *ten_chuoi;
## *3.thao tác*
### - Dùng thư viện string.h:
- `strcpy(s1, s2);`
Sao chép chuỗi s2 cho chuỗi s1.
- `strcat(s1, s2);`
Nối chuỗi s2 vào cuối chuỗi s1.
- `strlen(s1);`
Trả về độ dài của chuỗi s1.
- `strcmp(s1, s2);`
Trả về 0 nếu s1 và s2 là như nhau; nhỏ hơn 0 nếu s1<s2; lớn hơn 0 nếu s1>s2.

- `strchr(s1, ch);`
Trả về con trỏ tới vị trí đầu tiên của ch trong s1.
- `strstr(s1, s2);`
Trả về con trỏ tới vị trí đầu tiên của chuỗi s2 trong chuỗi s1.

### -Ví dụ:

*\#include <iostream>

\#include <cstring>

using namespace std;

int main ()
{
   char chuoi1[10] = "Hello";
   
   char chuoi2[10] = "Christmas";
   
   char chuoi3[10];
   
   int  len ;

   // sao chep chuoi1 vao trong chuoi3
   
   strcpy( chuoi3, chuoi1);
   
   cout << "strcpy( chuoi3, chuoi1) : " << chuoi3 << endl;

   
   // noi hai chuoi: chuoi1 va chuoi2
   
   strcat( chuoi1, chuoi2);
   
   cout << "strcat( chuoi1, chuoi2): " << chuoi1 << endl;

   
   // tong do dai cua chuoi1 mot sau khi thuc hien noi chuoi
   
   len = strlen(chuoi1);
   
   cout << "Dung ham strlen(chuoi1) de tinh do dai chuoi1: " << len << endl;

   return 0;
}*

## *4.Mảng và chuỗi ký tự*
Khai báo theo mẫu.


type *pointer_array[size];

