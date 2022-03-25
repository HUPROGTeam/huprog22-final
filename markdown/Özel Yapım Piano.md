# Özel Yapım Piano
           

Oğuzhan müziği ve müzik aletlerini çok seven ünlü bir sanatçıdır. Birçok farklı müzik aleti çalar ve artık sadece kendinin çalabileceği özel bir piyano üretmek ister.

Ürettiği 88 tuşlu piyanonun özellikleri şöyledir;

-   Her tuş 0 ile 87 (0 ve 87 dahil) arasındaki numaralarla temsil edilir.
-   Piyano sadece tuşlarına çift olarak bastığınızda ses çıkarır.
-   Bir tuşa bastığınızda piyano ses çıkarmaz. Ses için bir tuşa daha basmanız gerekir. İkinci tuş için herhangi bir tuşa basabilirsiniz ve piyano ses çıkarır.

Kendi ürettiği piyanoda yeni albüm çıkarmak isteyen Oğuzhan, bir kağıda rasgele yazdığı piyano tuşu numaralarını albümün bir müziğine çevirmek istiyor. Müzik kulağına güvenen Oğuzhan için en önemli şey albüm müziklerinin desibel olarak olabilecek en düşük seviyede kalmasıdır.

Müziği çalarken uyguladığı kurallar şöyledir;

-   Piyanonun herhangi iki tuşuna basıldığında piyanonun ürettiği sesin desibeli, $tuş1 * tuş2$ şeklinde hesaplanır.
-   Müziği çalmaya başladığı ilk adımda rastgele numaralardan bir tuş çifti seçer.
-   Sonraki adımda basılacak tuş çiftindeki tuşlardan biri $((tuş1 + tuş2) \text{ mod  88})$ numaralı tuştur.

Örneğin kağıda yazdığı rastgele 80,81,82 numaralarıyla çıkartacağı minimum desibelli müziği çalarken;

-   İlk olarak rasgele tuş çifti seçerek çalmaya başlıyor. 80 ve 81’i seçti diyelim.
-   Piyanoyu çalmaya 80. ve 81. tuş çiftine basarak başladıktan sonra, bir sonraki tuş çiftinde $80+81\text{ mod }88=73$ numaralı $tuş$a ve rastgele numaralardan geriye kalan 82 numaralı tuşa basmalıdır. Geriye basması gereken $73+82\text{ mod }88=67$ numaralı tuş kaldı ama tek başına basıldığında ses çıkartamayacağı için müzik bitti.
-   (80,81,82 -> (81,82),80 -> 75,80 -> 67) desibel = $81*82 = 6642 + 75*80 = 12642$
-   (80,81,82 -> (80,82),81 -> 74,81 -> 67) desibel = $80*82 = 6560 + 74*81 = 12554$
-   (80,81,82 -> (80,81),82 -> 73,82 -> 67) desibel = $80*81 = 6480 + 73*82 = 12466$ (minimum desibel)

Oğuzhan rastgele numaraların yanına çıkan minimum desibelleri not etmek istemektedir. Albüm birçok şarkıdan oluşacağı için bütün olasılıkları denemek onun için zorlaşmıştır. Ona rastgele numaralardan oluşacak müziğin minimum desibelini bulmada yardım etmeniz gerekiyor.

80,81,82 -> 12466

## Input Format
İlk satır n = çalınacak müzik için kağıda yazılan rastgele tuş sayısı.

İkinci satır n tane tuşu temsil eden rastgele numaralar.

## Output Format
Minimum desibel

## Constraints
- $2\le n \le 120$
- $0 \le tuş \le 87$

## Sample Input 1
```
2
33 37
```

## Sample Output 1
```
1221
```

## Sample Input 2
```
3
44 22 66
```

## Sample Output 2
```
1452
```

## Explanation 2
44\. ve 66. tuşlara basarsak, 44*66 = 2904 desibel ses çıkar ve bir sonraki adımda basmamız gereken tuşlardan birinin numarası ((44+66)mod88) = 22dir. 22. tuşa iki kere basarsak, 22 * 22 = 484 desibel ses çıkar. Toplamda 3388 desibel ses çıkmıştır.

22\. ve 44. tuşlara basarsak, 22*44 = 968 desibel ses çıkar ve bir sonraki adımda basmamız gereken tuşlardan birinin numarası ((22+44)mod88) = 66dir. 66. tuşa iki kere basarsak, 66 * 66 = 4356 desibel ses çıkar. Toplamda 5324 desibel ses çıkmıştır.

22\. ve 66. tuşlara basarsak, 22*66 = 1452 desibel ses çıkar ve bir sonraki adımda basmamız gereken tuşlardan birinin numarası ((22+66)mod88) = 0dır. 0. ve 44. tuşlara basarsak, 0 * 44 = 0 desibel ses çıkar. Toplamda 1452 desibel ses çıkmıştır minimum desibeli bulduk.