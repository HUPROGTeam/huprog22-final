# Dairesel Turing Makinesi

Bazı bilgisayar bilimcileri Turing Makinesi fikrinden yararlanarak yeni bir hayali makine yapmaya karar verirler. Makinenin amacı biri hariç diğer tüm hücreleri belli kurallarla elemektir. Bu makine dairesel bir yapıda tasarlanmıştır ancak bu yapıda sonsuz döngü bulunmasından korkmaktadırlar. Böyle bir duruma uğramayacak bir sistem tasarlamaya başlamışlardır. Makinenin okuma ve yazma için kullanılan ve gezebilen bir aygıtı ve üstünde gezdiği dairesel bir hücreler bütünü vardır. Başlangıçta $n$ kadar hücrenin herbirinde o hücrenin numarası yazmaktadır. Aygıt $1$ numaralı hücreden başlayarak okuma, yazma ve gezme işlerini sırasıyla aşağıdaki kurallara göre yapacaktır:

-   Uğradığı hücreye sağ ve solundaki komşu hücrelerdeki değerlerin toplamını yazar.
-   Bulunduğu hücrenin rakamları toplamı sayısında hücre kadar saat yönünde ilerler.
-   İlerlemeye başlamadan önce hücredeki değeri kontrol eder ve eğer $2n$'den ($n$ başlangıçtaki hücre sayısıdır) daha büyük veya eşitse o hücreyi eler/siler.

Ancak bilgisayar bilimcileri bu sistemde belli durumlarda sonsuz döngüden kurtulamadıklarını fark ederler. Yani bazı durumlarda aygıt sürekli belli hücreler arasında gidip gelmektedir. Bu durumlarda döngünün gerçekleştiği bütün hücreleri kaldırıp aygıtı başlangıç hücresine getirmeye karar verirler. (Başlangıç hücresi başta $1$ değeri yazan hücredir. Bu hücrenin silinmesiyle saat yönünde ondan sonraki hücre başlangıç hücresi olur. Bilgisayar bilimcilerine her bir $n$ değeri için son kalan hücredeki değeri bulmada yardımcı olunuz.

## Input Format
Başlangıçtaki hücre sayısı $n$

## Output Format
Son kalan hücredeki değer

## Constraints
$1\leq n \leq10^5$

## Sample Input 1
```
3
```

## Sample Output 1
```
2
```

## Explanation 1

Dairesel düzlemde 1'in solunda 3, sağında 2 bulunmakta. Bu nedenle o hücreye bu iki değerin toplamı olan 5 yazıyoruz. 5 adım sonrası olan 3 değerli hücreye 7 yazıyoruz ancak bu değer 2n'den büyük olduğu için bu hücreyi kaldırıyoruz. Son hücrenin üstündeki değer olan 7 hücre kadar gidip o hücreyi de değiştiriyoruz. Kalan son hücredeki değer 2'dir.