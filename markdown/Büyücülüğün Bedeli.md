# Büyücülüğün Bedeli

Arda boş zamanlarında MMORPG temalı bir bilgisayar oyunu oynamaktadır. Bu oyunda 4 ayrı karakter sınıfı vardır: Savaşçı, okçu, düzenbaz ve büyücü. İsteyen her oyuncu eğer doğru eşyaları koordineli bir şekilde kullanırsa istediği sınıfın özelliklerine erişebilmektedir.

Arda'nın daha önce oynamadığı tek sınıf büyücüdür. Büyücülerin özelliklerine erişmek içinse **4 adet eşyaya** ihtiyaç vardır: **Asa**, asayı aktif hale getiren **büyü taşı**, büyü taşını aktif hale getiren **element yüzüğü** ve element yüzüğünü aktif hale getiren **element kitabı**.

Arda'nın belli bir oyun parası karşılığında alabileceği:

-   $x_1$ adet asa ($i$. sıradaki $a_i$ tutarında)
-   $x_2$ adet büyü taşı ($i$. sıradaki $b_i$ tutarında)
-   $x_3$ adet element yüzüğü ($i$. sıradaki $c_i$ tutarında)
-   $x_4$ adet element kitabı ($i$. sıradaki $d_i$ tutarında) bulunmaktadır.

Büyücü oynamak isteyen bir oyuncunun aklında bulundurması gereken başka bir şey ise birbirini aktif hale getiren eşyaların birbiriyle uyumlu olması zorunluluğudur: Asa ve büyü taşı, büyü taşı ve element yüzüğü, element yüzüğü ve element kitabı birbiriyle uyumlu bir şekilde çalışmalıdır.

Oyunda uyumlu olmayan:

-   $n_1$ adet asa ve büyü taşı
-   $n_2$ adet büyü taşı ve element yüzüğü
-   $n_3$ adet element yüzüğü ve element kitabı vardır.

Arda sırasıyla asa, büyü taşı, element yüzüğü ve element kitabı eşyalarını oyundaki parasını en az şekilde harcayarak alıp büyücü sınıfını oynamak istemektedir. Ona yardım edin!

## Input Format
-   İlk satırdaki 4 sayı sırasıyla asa çeşidi sayısı($x_1$), büyü taşı çeşidi sayısı($x_2$), element yüzüğü çeşidi sayısı($x_3$) ve element kitabı çeşidi sayısını($x_4$) vermektedir.
-   Ondan sonraki gelen 4 satırda sırasıyla asaların tutarı($a_1$, $a_2$,...$a_{x_1}$), büyü taşlarının tutarı($b_1$, $b_2$,...$b_{x_2}$), element yüzüklerinin tutarı($c_1$, $c_2$,...$c_{x_3}$) ve element kitaplarının tutarı($d_1$, $d_2$,...$d_{x_4}$) verilmektedir.
-   Sonraki satır birbiriyle uyumlu olmayan asa ve büyü taşı sayısını veren bir sayı içermektedir($n_1$). Sonraki $n_1$ satırda iki tane sayı verilmektedir: İlk sayı ($j_i$) asanın sırasını, ikinci sayı ($k_i$) ise büyü taşının sırasını vermektedir. Verilen sıralardaki asa ve büyü taşları birbirleriyle uyumlu değildir. Her $j_i$, $k_i$ ikilisi birbirinden farklıdır.
-   Birbiriyle uyumlu olmayan büyü taşı ve element yüzüğü($n_2$), element yüzüğü ve element kitabı($n_3$) için de yukarıdaki kural geçerlidir.

## Output Format
Uyumlu olmayan eşya çiftleri haricinde bir eşya alınamıyorsa $-1$ yazdırın. Onun dışında Arda'nın büyücü sınıfını oynayabilmesi için gereken minimum tutarı yazdırın.

$Önemli$ $Not$ : Büyücü sınıfını oynamak için bütün eşya çiftlerinin uyumlu olması gerekmektedir. Yani herhangi bir eşya çifti bile uyumlu değilse büyücü sınıfı oynanamamaktadır.

## Constraints
-   $1\leq x_i \leq100$
-   $1\leq a_i, b_i ,c_i, d_i \leq10^4$
-   $0\leq n_i \leq x_i * x_{i+1} \leq 10^4$
-   $1 \leq  j_i  \leq  x_i$ **ve** $1 \leq k_i \leq x_{i+1}$

## Sample Input 1
```
4 3 2 1
4 3 2 1
7 5 6
8 9
10
2
4 2
4 3
2
1 2
1 1
1
1 1
```

## Sample Output 1
```
26
```

## Explanation 1
![Resim](https://imagizer.imageshack.com/img924/9114/41Vv2m.png)

Oklar uyumlu olmayan eşya çiftlerini göstermektedir. Buna göre en iyi seçenek 3. sıradaki asayı(2 tutarında), 2. sıradaki büyü taşını(5 tutarında), 2. sıradaki element yüzüğünü(9 tutarında) ve 1. sıradaki element kitabını(10 tutarında) almaktır.

## Sample Input 2
```
5 1 1 5
1 2 3 4 5
6
7
8 9 10 11 12
0
1
1 1
0
```

## Sample Output 2
```
-1
```

## Explanation 2
Alınabilecek tek bir büyü taşı-element yüzüğü ikilisi vardır ve onlar da uyumlu değildir.