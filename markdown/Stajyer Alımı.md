# Stajyer Alımı
Bir şirket stajyer alımı yapacaktır. **N** tane departmana kapasiteleri kadar alım yapacaktır. Departmanlar binada tek bir koridorda **art arda** dizilmişlerdir. Bu şirketin işe alım konusunda bazı takıntıları vardır.  

* **Komşu olan departmanlara aynı sayıda** stajyer alımı yapmamaktadırlar. 
* Yapacağı alımlarda **kapasitelerin dolma zorunluluğu** yoktur.
*  **En az bir kişi** o departmana stajyer olarak alınmalıdır. Eğer bu mümkün değilse şirkete hiç stajyer alınmaz.

Toplam departman sayısı ve her bir departmanın kapasitesi bilinmektedir. Bu şirket kaç farklı işe alım kombinasyonu yapabileceğini merak etmektedir. Onlara yardımcı olur musunuz?

*Not: Toplam sayıyı mod $10^9+7$ 'ye göre yazdırın.*

## Input Format
İlk satır toplam departman sayısını vermektedir.
İkinci satır her bir yan yana dizilmiş departmanların toplam kapasitelerini $a_1$, $a_2$, ..., $a_n$ olarak verilmiştir.

## Output Format
Tüm farklı işe alımların mod $ 10^9+7 $ 'ye göre çıktısı

## Constraints
$1 \leq n \leq 2⋅10^5$

$1 \leq  a_i  \leq 10^9$

## Sample Input 1
```
2
2 4
```
## Sample Output 1
```
6
```

## Explanation 1
Şirket [1,2], [1,3], [1,4], [2,1], [2,3] ve [2,4] şeklinde işe alım yapabilir. Yani toplamda 6 farklı işe alım durumu oluşur.

## Sample Input 2
```
4
1 1 1 1
```

## Sample Output 2
```
0
```

## Explanation 2
[1,1,1,1] durumu komşu departmanların stajyer sayısı eşit olamayacağından oluşamaz. Yani şirkete stajyer alınamaz. Bu da 0 durum anlamına gelmektedir.