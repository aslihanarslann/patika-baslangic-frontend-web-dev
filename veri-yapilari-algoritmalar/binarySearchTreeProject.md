# Binary Search Tree Project

Bu dosya [patika.dev](https://www.patika.dev/tr)'e ait olan ["Veri Yapıları ve Algoritmalar"](https://academy.patika.dev/courses/veri-yapilari-ve-algoritmalar) dersinin [**Binary Search Tree**](https://academy.patika.dev/courses/veri-yapilari-ve-algoritmalar/binary-search-tree) proje ödevini içermektedir.

***
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

**Yanıt:**

Bir düğüm her iki tarafa da referans verebiliyor. Sağ ve sol olarak. Sağ tarafından kendinden büyük elemanlar, sol tarafında ise kendinden küçük elemanlar bulunacak.


Root = 7

> - 1.Adım: Root = 7 'dir.

                    7



> - 2 .Adım: 5 ekleme =>  Root'un solunda 5 bulunur.
    
                    7
                  /
                5

> - 3 .Adım: 1 ekleme => Root'un solunda 5 bulunur ve 5'in solunda 1 bulunur.
                    7
                  /
                5
              /
            1 

 > - 4.Adım: 8 ekleme => Root'un sağında 8 bulunur.

                    7
                  /   \
                5       8
              /
            1 

 > - 5.Adım: 3 ekleme => Root'un solunda 5,  5' in solunda 1, 1'in sağında ise 3 bulunur.
                    7
                  /   \
                5       8
              /
             1 
               \
                 3


> - 6.Adım: 6 ekleme => Root'un solunda 5,  5' in solunda 1, 5'in sağında ise 6 bulunur.

                    7
                  /   \
                5       8
              /   \
             1     6
              \
                3


> - 7.Adım: 0 ekleme => Root'un solunda 5,  5' in solunda 1, 1'in solunda ise 0 bulunur.

                    7
                  /   \
                5       8
              /   \
             1     6
            / \
           0   3

> - 8.Adım: 9 ekleme => Root'un sağında 8, 8'in sağında ise 9 bulunur.

                    7
                  /   \
                5       8
              /   \      \
             1     6      9
            / \
           0   3


> - 9.Adım: 4 ekleme => Root'un solunda 5, 5'in solunda 1, 1'in sağında 3, 3'ün sağında 4 bulunur.

                    7
                  /   \
                5       8
              /   \      \
             1     6      9
            / \
           0   3
                \
                 4


> - 10.Adım: 2 ekleme => Root'un solunda 5, 5'in solunda 1, 1'in sağında 3, 3'ün sağında 4, 3'ün solunda 2 bulunur.

                    7
                  /   \
                5       8
              /   \      \
             1     6      9
            / \
           0   3
              / \
             2   4
