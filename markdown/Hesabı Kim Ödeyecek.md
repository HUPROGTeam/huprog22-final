# Hesabı Kim Ödeyecek

![](sarimsak-sucuk.jpg)

Berat ve Şura sarımsak soslu sucuklu pizza yemeye giderler. Fakat aralarındaki anlaşma gereği hesabı ayrı ayrı ödemek yerine her zaman tek bir kişi ödeyecektir. Hesabı ödeyeni belirlemek için alışılmışın dışında "Hesabı kim ödeyecek" isimli yeni bir şans oyunu bulurlar. Bu oyunda her tur için belirli bir $n$ sayısı ve 1'den $n$'e kadar numaralandırılmış kart destesi vardır. Ayrıca $m$ tane elemanı olan bir $a$ sayı dizisi vardır. Oyun şöyle ilerler: 

Berat $m$ tane, her biri diğerleriyle aralarında asal olan sayıları kağıtlara yazıp bir kutuya atar. Numaralandırılmış sayıların katları olan kartlar desteden çıkarılır. Bu işlemden sonra destede kalan kart sayısına göre hesabı kimin ödeyeceğini belirleyeceklerdir. Fakat kalan kart sayısını hızlı hesaplamaları gerekir.

Örneğin;

$n$ sayısı 30 olsun. $m$ sayısı 3 olsun ve $m$ tane sayı sırasıyla 7 3 2 olsun.

Desteden 2, 3, 4, 6, 7 8, 9, 10, 12, 14 ,15, 16, 18, 20, 21, 22, 24, 26, 27, 28, 30 sayılarını çıkarınca destede 9 adet kart kalır.

Bu problemi büyük sayılar için teker teker hesaplamak zor olacağından, bir algoritma yazmaya karar verirler. Bu algoritmayı yazmakta yardımcı olun.

## Input Format
- İlk satırda $n$ ve $m$ sayıları verilmiştir
- İkinci satırda $a$ dizisinin elemanları verilmiştir

## Output Format
İşlemler yapıldıktan sonra destede kalan kart sayısı.

## Constraints
- $0 \leq  n  \leq  10^{9}$
- $0  \leq  m  \leq  100$
- $0  \leq  a[i]  \leq  1000$

## Sample Input 1
```
50 5
2 7 5 51 19
```

## Sample Output 1
```
16
```
