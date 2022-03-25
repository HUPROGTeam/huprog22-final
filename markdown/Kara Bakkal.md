# Kara Bakkal

Kara Bakkal'ın sahibi Bay Kara, aylık malzeme stoğunu yenilemek için farklı satıcıların fiyatlarını karşılaştırmaktadır. Kara Bakkal'ın kendince belirlediği bir aylık bütçesi $B$ vardır. Kara Bakkal'ın bulunduğu şehirde $N$ adet satıcı vardır ve Kara Bakkal da bütçesine en uygun şekilde mallarını onlardan almayı planlamaktadır. Alması gereken malzeme miktarlarının _ortalama değeri_ en az olan satıcıyı seçecektir. Eğer alışveriş yaptığı satıcıdaki ürünler Kara Bakkal'ın malzeme ihtiyacını karşılamıyorsa, o satıcıdan **ihtiyacı kadarını** aldıktan sonra aynı şekilde başka bir satıcı seçip ihtiyaç listesindeki bütün malzemeleri almaya çalışacaktır.

Ortalama fiyat hesabı **her bir satıcı için** şöyle hesaplanır :

-   O satıcıdaki her bir ürün için :
    -   Eğer satıcının elindeki ürün miktarı Kara Bakkal'ın ihtiyacı olan mal miktarı'ndan az veya eşit ise **satıcının elindeki miktar** ile satıcının o ürüne biçtiği fiyat çarpılır.
    -   Eğer satının elindeki ürün miktarı Kara Bakkal'ın ihtiyacı olan mal miktarı'ndan fazla ise Kara Bakkal'ın ihtiyacı olduğu miktar ile satıcının ürün için biçtiği fiyat çarpılır. Bu işlem **sadece Kara Bakkal'ın ihtiyacı olan ürünler** için yapılır ve tüm bu çarpımlar toplanır. Sonunda da bu toplam **Kara Bakkal'ın ihtiyacı olan ürün sayısına** bölünür. Böylece o satıcının ortalama fiyat hesabı bulunmuş olur.
-   Eğer satıcıdaki bir malın sayısı ihtiyaç olandan daha az ise, **satıcıdaki miktar** kadar alır ve kalan ihtiyaçlarını tamamlamak için başka satıcılara yönlenir.

Listedeki tüm malzemeler alındıktan sonra Kara Bakkal'ın ne kadar bütçesi kaldığını bulunuz.

## Input Format
$B$ - Bütçe

$N$ - İhtiyacı olan malzeme sayısı

Sonraki $N$ satır, ihtiyacı olan malzeme miktarlarını verir

$k$ - kaç satıcı olduğu bilgisini verir.

Sonraki $k * N$ satır, sırasıyla her satıcının, her bir ürün için elinde olan ürün miktarını ve o ürünün birim fiyatını verir.

## Output Format
İhtiyacı olan tüm malzemeleri aldıktan sonra elinde kalan bütçesini yazdırınız.

## Constraints
Listenin tamamlanmayıp paranın bittiği bir durum olmayacaktır.

$0 \le N \le 10^3$

$0 \le k \le 10^3$

$0 \le B \le 10^5$

## Sample Input 1

```
20
2
5
5
3
5 2
2 2
5 10
5 2
10 5
10 8
```

## Sample Output 1
```
0
```

## Explanation 1
-   20 (Bütçe)
-   2 (İhtiyaç olan malzeme türü sayısı n)
-   5 (1. Malzeme ihtiyacı)
-   5 (2. Malzeme ihtiyacı)
-   3 (Farklı satıcı sayısı k)
-   5 2 (1. Satıcının 1. Malzeme miktarı ve birim fiyatı)
-   2 2 (1. Satıcının 2. Malzeme miktarı ve birim fiyatı)
-   5 10 (2. Satıcının 1. Malzeme miktarı ve birim fiyatı)
-   5 2 (2. Satıcının 2. Malzeme miktarı ve birim fiyatı)
-   10 5 (3. Satıcının 1. Malzeme miktarı ve birim fiyatı)
-   10 8 (3. Satıcının 2. Malzeme miktarı ve birim fiyatı)

1.  Satıcının ortalama birim fiyatı: \[(5 x 2) + (2 x 2)\] / 7 = 2
2.  Satıcının ortalama birim fiyatı: \[(5 x 10) + (5 x 2)\] / 10 = 6
3.  Satıcının ortalama birim fiyatı: \[(5 x 5) + (5 x 8)\] / 20 = 6.5 (Satıcıda bulunan malzeme miktarları 10 olduğu halde her malzemeden 5 adet lazım olduğu için ortalama alınırken ihtiyacı olduğu malzemelere bakılır)
4.  Satıcının ortalama fiyatı en düşük olduğu için seçilir. Bütçeden 14 lira eksilir, yeni bütçe 6 lira.
5.  Malzemeden 0 adet, 2. malzemeden 3 adet ihtiyaç kalmıştır.
    
Yeniden ortalamalar hesaplanır.

1.  Satıcı ortalama listesine alınmaz çünkü elindeki tüm ürünler bitmiştir ve 1. Malzemeden hiç ihtiyaç kalmadığı için ortalama hesaplanırken hesaba katılmaz.
2.  Satıcının ortalama birim fiyatı: (3 x 2) / 3 = 2 (Satıcıda bulunan 2. malzeme miktarı 5 olduğu halde 2. malzemeden 3 adet lazım olduğu için ortalama alınırken sadece ona bakılır)
3.  Satıcının ortalama birim fiyatı: (3 x 8) / 3 = 8 (Satıcıda bulunan 2. malzeme miktarı 10 olduğu halde 2. malzemeden 3 adet lazım olduğu için ortalama alınırken sadece ona bakılır)
4.  satıcı seçilir. Bütçeden 6 lira eksilir, yeni bütçe 0 lira. Başka malzemeye ihtiyaç yoktur. Cevap 0