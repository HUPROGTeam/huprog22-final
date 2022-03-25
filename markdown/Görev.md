# Görev
*Şura*, *Berat*, *Aysera* ve *Özgün*'nün yapmaları gereken bir görev vardır. Bu görev *en az X en fazla Y gün* sürebilmektedir. Görevi her gün sadece bir kişi yapabilmektedir. Bu yüzden bir görev sıralaması yapmaya karar verirler. Sıralamada dikkat etmeleri gereken bazı durumlar vardır.
* Bir kişi **art arda görev yapmamalıdır**.
* *Özgün* ve *Berat* **birbiri ardına görev yapamazlar.** Yani sıralamada ÖB veya BÖ yer alamaz.
* İkinci maddedeki durum *Aysera* ve *Şura* için de geçerlidir.
* Bir sıralama ihtimalinin ters sıralaması kendisine eşit olarak düşünülecektir. Yani **BŞÖA <-->AÖŞB sıralamasına eşittir**, bu sebeple **ters sıralamalar durumlara dahil edilmeyecektir**.
* *Şura*, *Berat* ve *Aysera* permütasyonlarının hiçbiri sıralama içerisinde yer almamalıdır. Örneğin; **ÖŞBA** -->sıralaması yer alamaz çünkü **ŞBA** bu üç kişinin sıralamalarıdır.

**X, X+1, .., Y olası günleri** için tüm bu durumlar ele alınarak oluşan bütün permütasyonların sayısı hesaplanacaktır.

## Input Format
X ve Y sayılarını içerir. Olası gün sayısının alt ve üst limitleri sırasıyla X ve Y dir.

## Output Format
Sorudaki koşulları sağlayan ve X'ten Y'ye kadar olan olası tüm günler için farklı, toplam görevi yapma sıralamalarını mod $10^9 + 7$'de yazdırın.

## Constraints
- $1 \leq X \leq Y \leq 10^9$

## Sample Input 1
```
3 4
```

## Sample Output 1
```
23
```

## Sample Input 2
```
1 2
```

## Sample Output 2
```
8
```

## Expalanation 2 
1 gün sürerse oluşabilecek durumlar : B, Ş, Ö, A -->4
2 gün sürerse oluşabilecek durumlar : BŞ, ÖŞ, BA, ÖA -->4
Toplamda 8 olasılık oluşmaktadır.
