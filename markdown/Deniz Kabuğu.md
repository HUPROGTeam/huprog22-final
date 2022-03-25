# Deniz Kabuğu
Anthony, Elif ve Yiğit sıcak bir yaz gününde sahilde deniz kabuğu birleştirme oyunu oynamaya karar verirler. Oyun üç nesne içerir, bunlar sağ kabuk parçası, sol kabuk parçası ve çakıl taşıdır. Inputta sol kabuk "(", sağ kabuk ")", çakıl taşı ise "\*" simgesi ile gösterilecektir. Sol kabuk ve sağ kabuk birbirlerini tamamlayıp bir bütün kabuk oluştururken (sadece oyuncu tamamlamak için sağ kabuğu seçtiğinde elinde çoktan sol kabuk bulunuyorsa), çakıl taşının özelliği ise oyuncunun bir önceki tur seçtiği nesneyi elinden bıraktırmasıdır. Çakıl taşının tek özelliği budur, kabuk bütünlemeye yaramayan bir taştır, bu yüzden oyunun sonunda oyuncunun elinde kalan çakıl taşları görmezden gelinir, sayısının da bir önemi olmaz. Oynanacak her turda oyuncuların ellerinde bu üç nesneden biri bulunur ve hiçbir oyuncu bir diğer oyuncu ile aynı nesneyi tutmaz. Oyuna her zaman Anthony başlar. Anthony, oyunun ilk turu bu üç nesneden birini seçer ve sonraki her tur diğer oyuncuların tuttuğu nesnelerden birini seçerek kendi elinde sadece tamamlanmış bütün kabuklar oluşturmaya çalışır. Oyunun başında belirlenen tur sayısı, oyunun kaç kez oynanacağını, yani oyuna başlayan oyuncunun kaç kez seçim yapacağını belirtir. Anthony oyuna bu üç nesneden birini seçerek başlar. Eğer sağ deniz kabuğu parçasını seçmişse, Elif ve Yiğit’ten biri sol parçayı ve diğeri çakıl taşını tutuyor olacaktır. Anthony’nin amacı, oyunun son turuna geldiğinde elinde sadece tamamlanmış kabukların bulunmasını sağlamaktır, bunun için Elif ve Yiğit’ten herhangi birinin tuttuğu nesneyi seçer ve elindeki nesnelere ekler. Anthony’nin seçtiği yeni nesneye göre Elif ve Yiğit de sonraki tur için o nesne harici diğer iki farklı nesneyi bulur ve Anthony bu şekilde seçim yapmaya devam eder. Oyun bu şekilde belirlenen tur sayısı kadar oynanır. Örneğin seçim yaparken Anthony elinde sol kabuğu tutuyor, Elif çakıl taşı tutuyor ve Yiğit sağ kabuğu tutuyorsa, Anthony Yiğit’ten sağ kabuğu alarak kabuğunu tamamlayabilir, eğer Elif’ten çakıl taşını alırsa, elindeki kabuk parçasını atmak zorundadır. Oyunun sonunda, Anthony kaç farklı şekilde elinde sadece tamamlanmış kabuklar tutuyor olacaktır?

## Input Format
Başlangıç simgesi, yani Anthony'nin ilk tur seçtiği nesne $a$ ilk tur dahil olmak üzere tur sayısı $n$

## Output Format
Olası tüm tamamlanmış kabuk durumları $m$ % $(10^{9}+7)$

## Constraints
$a$ sadece "(" , ")" ya da "\*" simgelerinden biri olabilir. 1 $\leq$ n $\leq$ 500

## Sample Input 1
```
(
3
```

## Sample Output 1
```
0
```

## Explanation 1
Bu oyun 3 el oynanacaktır, ve Anthony sol kabuk parçasını seçerek ilk elini oynar. Kalan iki el için, eğer Anthony diğer oyuncuların birinde bulunan çakıl taşını seçerse, elindeki kabuğu bırakmak zorundadır, ve son elde ise elinde sadece alabileceği sağ ya da sol kabuk bulunacağından elinde bütünlenmiş kabuk bulunmayacaktır, eğer sağ kabuk parçasını seçerse, son elde alabileceği ya bir çakıl taşı, ya da bir sol kabuk parçası olacaktır. Çakıl taşı 2. elde aldığı kabuk parçasını bırakmasını gerektirecek, sol kabuk parçasını aldığında ise elinde hepsi bütünlenmiş olan kabuklar değil, yarım bir kabuk parçası da bulunacağından yine hedefine ulaşamamış olur. Anthony hangi hamleyi yaparsa yapsın, 0 yol ile elinde bütünlenmiş kabuklar oluşturabilecektir.