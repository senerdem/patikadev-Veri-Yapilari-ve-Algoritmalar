# Proje 1

## A) [22,27,16,2,18,6] -> Insertion Sort

 1. Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.
 2. Big-O gösterimini yazınız.
 3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
 4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.


## B) [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

# Cevaplar

## A) [22,27,16,2,18,6] -> Insertion Sort

1. *Insertion sort yapılırken her adımda en küçük sayı bulunarak bulunması gereken sıradaki sayı ile yer değiştiriliyor. Dolayısıyla ilk adımımız 2 ile(en küçük sayı) 22'nin(en küçük sayının, yani 2'nin bulunması gereken sıradaki sayının) yerini değiştirmek. Devamındaki adımlarda da aynı mantık uygulanarak ilerleniyor.*

        - [2,27,16,22,18,6]
        - [2,6,16,22,18,27]
        - [2,6,16,18,22,27]

2. *Big-O gösterimi için her adımda harcadığımız zamanı hesaba katmamız gerekiyor. N tane sayı barındıran bir dizi için en küçük sayıyı bulmamız n işlem alıyor çünkü hepsine bakmamız gerekiyor teker teker. Dolayısıyla bir sonraki adım için n-1, sonraki için n-2 vb. devam ediyor, en sonunda 1 tane kalana kadar. Bu yüzden toplamda n+(n-1)+(n-2)+...+1 yani nX(n+1)/2 işlem yapmış oluyoruz. Sonuç olarak Big-O gösterimimiz:*

    ```
    O(n^2)
    ```

    *oluyor.*

3. *Average Case: Aradığımız sayı ortada ise adımlarda yaptığımız işlem sayısı n/2, n-1/2, n-2/2 şeklinde geriye 1 kalıncaya kadar ilerler. Dolayısıyla toplamda [n+(n-1)+(n-2)+...+1]/2 yani nX(n+1)/4 kadar işlem olmuş olur.*

    ```
    O(n^2)
    ```

    *Worst Case: Yukarıda açıklandı.*

    ```
    O(n^2)
    ```

    *Best Case: Aradığımız sayı her adımda dizinin en başındaysa dizi zaten sıralı anlamına gelir. Bu yüzden dizideki her sayı için bir kez dizi üzerinden geçeceğimizden dolayı n işlem yapılmış olur.*

    ```
    O(n)
    ```

4. Dizinin sıralanmış olması Best Case anlamına geldiği için 18 sayısı sıralandıktan sonra Best Case kapsamına girer.

## B) [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımı:

*En küçük 2, 7 ile yer değiştiriyor.*

    - [2,3,5,8,7,9,4,15,6]

*En küçük 3 olması gereken yerde.*

    - [2,3,5,8,7,9,4,15,6]

*En küçük 4, 5 ile yer değiştiriyor.*

    - [2,3,4,8,7,9,5,15,6]

*En küçük 5, 8 ile yer değiştiriyor.*

    - [2,3,4,5,7,9,8,15,6]