# Yatık Muzlar

Serhat, bu yaz work and travel programı ile Amerika’ya gitmek istiyor ancak gereken parayı bir türlü bulamıyor. Bu yüzden amcasının yanında manavda çalışmak istiyor ancak amcası onu bir şartla çalıştıracağını söylüyor. Serhat'ın inzva kış kampına katıldığını öğrenen amcası hem onu test etmek için hem de daha çok müşteri çekmek için Serhat'ın manav tezgahını mükemmel düzene sokmasını istiyor. Bu sayede mükemmel düzeni gören müşteriler daha çok ürün almak isteyecekler ve Serhat da inzva kampında öğrendiği muazzam bilgileri gerçek hayata uygulayabildiğini göstermiş olacaktır.

Manav tezgahında sadece 4 tür meyve bulunmaktadır: Elma, armut, sola yatık muz, sağa yatık muz.

Serhat’ın bu tezgahta, meyveler üzerinde yapabileceği işlemler şunlardır:

1. Sadece, yan yana duran iki meyvenin yerini değiştirebilir. Yani bir meyve ile bitişik olmayan başka bir meyvenin yerini değiştiremez. (Değiştirmek istiyorsa, tek tek değiştirmesi gerekiyor)
2. Tezgahtaki herhangi bir elmayı takas edebilir. Bir elma verdiğinde karşılığında 2 adet *sıralı olarak* 1 sola yatık muz ve 1 sağa yatık muz alabiliyor.
3. Tezgahtaki herhangi bir armutu takas edebilir. Bir armut verdiğinde karşılığında 2 adet *sıralı olarak* 1 sağa yatık muz ve 1 sola yatık muz alabiliyor.
4. *Asla* muzları takas edemez ya da muzları ters döndürüp farklı bir muza *dönüştüremez*, sadece muzların yerlerini değiştirebilir. ( Örneğin sola yatık muzu, sağa yatık muza çeviremez )
5. Yeni düzen bittiğinde elinde hiç elma ya da armut kalmamalıdır. Bu meyvelerin hepsini muzlara dönüştürmek zorundadır.

![yatik-muzlar.jpeg](yatik-muzlar.jpeg)

Amcasının Serhat’tan istediği meyveleri tezgaha mükemmel düzen oluşturarak dizmesidir. Mükemmel düzen 3 şekilden oluşabilir:

- Hiç bir meyve olmayabilir, yani boş bir tezgah
- İki ayrı mükemmel düzenden oluşabilir. Yani mükemmel düzen $m$, yine başka 2 mükemmel düzen $m2$ ve $m3$ ‘ den oluşabilir.
- Ya da, sola yatık muz + başka bir mükemmel düzen $m4$ + sağa yatık muz şeklinde olabilir.

Note : $m$, $m2$, $m3$, $m4$ farklı mükemmel düzenleri temsil etmektedir ve temsili olarak verilmiştir.

Serhat'ın tüm tezgahı en az kaç sayıda değiştirme ( swap ) işlemi yaparak mükemmel düzene sokabileceğini bulunuz.

Not : İlk durumda tezgahtaki toplam sola yatık muz sayısı, sağa yatık muz sayısına eşit olarak verilecektir.
Not II : Değiştirme ( swap ) işlemi sadece meyvelerin yerini değiştirirken olmaktadır. Elmayı ya da armutu takas etmek değiştirme ( swap ) sayılmıyor.
Not III : Swap operasyonlarını bitirmeden herhangi bir takas (trade) operasyonu yapamazsınız.

## Input Format
Yalnızca tek satır string $S$'ten oluşmaktadır. Bu satırda sırasıyla meyvelerin tezgahtaki yerleri verilmektedir. $S$ yalnızca belirtilen karakterlerden oluşmaktadır :

- 'L' : Sola yatık muzu temsil ediyor.
- 'R' : Sağa yatık muzu temsil ediyor.
- 'A' : Armutu temsil ediyor.
- 'E' : Elmayı temsil ediyor.

## Output Format
Bir tam sayı ( integer ) : Serhat'ın en az kaç kez değiştirme ( swap ) yaparak tezgahı mükemmel düzene sokabileceğini temsil eden sayı.

## Constraints
$0 \le S \le 8000$
