# Proje 2

## [16,21,11,8,12,22] -> Merge Sort

- Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
- Big-O gösterimini yazınız.

# Cevaplar

- Merge sort yaparken diziyi, tek elemanlı diziler elde edene dek parçalara ayırıp birleştirirken sıralıyoruz.

    ```
         [16,21,11,8,12,22]
      [16,21,11]     [8,12,22]
     [16,21] [11]   [8] [12,22]
    [16] [21] [11] [8] [12] [22]
    [16,21] [11]   [8,12] [22]
      [11,16,21]     [8,12,22]
         [8,11,12,16,21,22]
    ```
- Merge sort ile sıralama yaparken her basamakta diziyi 2'ye ayırdığımız için 2^x=n yani x=logn işlem ve her bir ayrılan parçayı birleştirmemiz de n işlem aldığından Big-O gösterimimiz:

    ```
    O(nlogn)
    ```

    şeklindedir.