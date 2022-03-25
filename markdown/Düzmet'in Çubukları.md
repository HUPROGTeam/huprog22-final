# Düzmet'in Çubukları
Düzmet düz bir insandır ve çok düz aktiviteler yapmaktadır. Son aktivitesinde Düzmet elindeki $n$ kadar özdeş çubuğu uç uca eklemiştir. Bu uçlar oynar eklemdir ve herbir çubuk birbiri üstüne katlanabilir. Ayrıca çubuklar o kadar incedir ki ardı ardına birbirileri üstüne katlanmaları için fiziksel bir engel bulunmamaktadır. Düzmet oluşturduğu çubuk sırasının bir ucunu sabitler. Diğer ucundan ise bir sonraki çubuğun ya sağına ya soluna katlamaya başlar. Bu işlemi bütün çubuklar yan yana gelene kadar tekrarlar. Her seferinde o ana kadar katladığı çubuk yığıntısını bir sonraki çubuğun sağına mı soluna mı katlayacağını seçer. Ancak Düzmet'in aklına bir soru takılır. Başta $i.$ sırada olan çubuğun katlamalar sonucunda oluşan sırada $f.$ olma durumlarının sayısı nedir?(Baştaki çubuk dizgesinde katlanılmaya başlanılan uçtan sıralanır. Sondaki dizgede ise soldan sıralanır.) Ancak Düzmet çok düz biri olduğu için bu soruyu çözememektedir. Düzmet'e yardım ediniz.

## Input Format
Tek satırda; çubuk sayısı $n$, başlangıçtaki sıra $i$, sondaki sıra $f$

## Output Format
Şartları sağlayan durumların sayısı $m$ % $(10^{9} + 7)$

## Constraints
1 $\leq$ $i$, $f$ $\leq$ $n$ $\leq$ $10^{4}$

## Sample Input 1
```
3 1 2
```

## Sample Output 1
```
2
```

## Explanation 1
Burada 3 çubuktan ilk durumda 1. sırada olan çubuğun son durumda 2. olduğu durumların sayısı soruluyor. 3 çubuk olduğu için 2 kez katlanabilir. İlk katlanma sola, ikinci katlanma sola ve ilk katlanma sağa, ikinci katlanma sağa durumları şartları sağlamaktadır. Yani 2 durum bulunmaktadır.