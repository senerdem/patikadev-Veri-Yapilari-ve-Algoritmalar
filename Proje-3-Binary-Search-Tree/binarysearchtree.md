# Proje 3

## [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

- Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

# Cevap

- Root 5 olarak kabul edersek soluna gelecek sayılar bundan küçük olmalı, sağına gelecek sayılar ise büyük olmalı. Bu yüzden 1, 3, 0, 4, 2 rakamları solunda bulunurken 7, 8, 6, 9 rakamları sağında bulunur. Bu mantığı her adımda uygularsak elde edeceğimiz binary search tree budur:

    ```
                 5                 
         1              7
     0       3      6       8
           2   4
    ```