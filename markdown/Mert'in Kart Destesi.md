           

# Mert’in Kart Destesi
Mert, sonunda Kore'ye gitmiştir ama zaman su gibi akmıştır ve dönüş günü gelmiştir. Dönmeden önce hatıra olarak imzalı K-Pop kartları almaya karar verir. Böylece geri döndüğünde arkadaşı Emre'ye hava atabilecektir.

Kart almak için gittiği dükkânda alabileceği $n$ sayıda kart destesi vardır. Ama bu dükkânda garip bir kural vardır. Kartları sadece destenin üstünden alabilmektedir ve destenin arasından kart alması yasaktır. Ayrıca bir desteden kart almaya başladığı zaman diğer desteden kart alamaz. Eğer kart almaya başladığı destede alttaki bir kartlardan birini almak istiyorsa en üstten o karta kadar olan kartların hepsini almak zorundadır. Ama en üstteki kartı her zaman almak zorunda değildir, çünkü o sırada dükkâna gelen başka biri o kartı alabilir ve Mert alttaki kartlardan birinden itibaren almaya başlayabilir.

Kartların her birinin üzerinde K-Pop'ta ünlü olan ve o dükkân sahibinin seçtiği $26$ ünlüden birinin resmi ve imzası vardır. Ayrıca, bu $26$ K-Pop yıldızının herkes tarafından bilinen popülerlik sıralaması vardır.

**Kızların Popülerlik Sıralaması:**

Miyeon > Soyeon > Minnie > Yuqi > Shuhua > Sana > Jihyo > Dahyun > Nayeon > Chaeyoung > Sieun > Sumin > Seeun > Jayoon > Yeeun > Seojin > Yeseo > Lisa > Jisoo > Rose > Jennie > Hwasa > Moonbyul > Wheein > Yongsun > Kyujin

Mert en mantıklı seçimi yapmak ister, bu nedenle satın alabileceği tüm olasılıkları yazmaya karar verir. Mert, mağazanın tuhaf kurallarının yetmezmiş gibi kartları en verimli şekilde satın almak için olasılıkları sıralarken bazı kurallar uydurur.

Bu sıralama görevinin kuralları aşağıdaki gibidir:

- Seçilen bir deste daha popüler bir kişiye sahip bir kartla başlıyorsa, diğer destelerden önce gelmelidir.

**Örnek:** [Miyeon, Soyeon], [Yuqi, Soyeon]'dan önce gelir

- Her iki deste aynı kişi ile başlıyorsa, sıralama için ikinci kart dikkate alınmalıdır. Destelerin ilk iki kartı aynıysa, sıralama için üçüncü kart dikkate alınmalıdır.

**Örnek:** [Soyeon, Miyeon] [Soyeon, Lisa]'dan önce gelir ve [Soyeon, Miyeon, Lisa] da [Soyeon, Miyeon, Moonbyul]'dan önce gelir

- Seçilen destenin en üstünde aynı karttan daha fazla varsa, bu durum bu destenin daha az aynı karta sahip olandan daha az popüler olduğu anlamına gelir. Çünkü Mert aynı parayla farklı kartlar alabilir, bu yüzden aynı karttan daha fazla almak para harcaması açısından verimsizdir.

**Örnek:** [Rose], [Rose, Rose]'dan önce gelir

- Olasılık listesinde bir destenin birden fazla kopyası varsa, bunlardan biri listeye yazılır.

- Sıralama için desteleri karşılaştırırken, bir destenin sonuna gelindiyse, bitmiş deste uzun desteden önce yazmalıdır.

**Örnek:** [Jayoon, Seeun, Dahyun] [Jayoon, Seeun, Dahyun, Yeseo]'dan önce gelir

Bu sıralanmış olasılıklar listesini yaptıktan sonra Mert, hangi olasılığın daha iyi olduğunu çözmek için rastgele sorgu numaralarını deneyerek gelen sayının olasılık listesindeki karşılığına bakar. Mert'in bu sorunu bir algoritma ile çözmesine yardımcı olabilir misiniz?

## Input Format

İlk satır, alabileceği kart destesi sayısı olan $n$ verir.

$n$ tane satır destelerin içerdiği kartların listesini $string$ olarak verir.

Sonraki satır yapılacak sorgu sayısı olan $s$ verir.

$s$ tane satır sorulan olasılığın numarasını içerir.

## Output

$s$ tane alt alta yazılmış sorgu cevapları olan kart grubunu içerir. Eğer yapılan sorgu geçersiz ise $INVALID$ yazısı return edin.

## Constraints

$1 \le n \le 50$

$1 \le$ bir destede olabilecek kart sayısı $\le 2000$

$1 \le s \le 500$

$1 \le$ olasılık numarası $\le 10^9$

