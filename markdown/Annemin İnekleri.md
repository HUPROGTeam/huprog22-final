# Annemin İnekleri

Köyde geçimini sürdürmekte olan bir anne, süt, tereyağı ve yoğurt satarak kazandığı parayı oğlu Serhat’a okusun da adam olsun diye yollamaktadır. Oğlu da ileride ailesine bakacağını ve onları yalnız bırakmayacağını biliyor ancak şu anda da onlara yardım etmek istiyor. Bu yüzden annesinin köyde yapması gereken işleri birkaç günlüğüne de olsa o üstleniyor. Köydeki işlerden biri de annesinin göz bebeği ve tüm geçim kaynakları olan inekleri beslemek. İnekler 1’den $N$’e kadar numaralandırılmış besi yerlerinde yemeklerini yiyebiliyorlar ve bir besi yerinde birden fazla inek de beslenebiliyor. Ancak bu ineklerin özel bir isteği var ve ancak bu istek karşılanırsa bol miktarda süt verebiliyorlar : diledikleri besi yerinde yemek yemek. Bu yüzden de annesi Serhat’tan inekleri,  istedikleri besi yerine göre konumlandırmasını istiyor. Yani $i^{th}$ inek başlangıçta $A_i$’nci besi yerinde duruyor ancak $B_i$’nci besi yerinde yemek istemektedir.

Serhat’ın yapabileceği yalnızca tek işlem vardır : Eğer bir besi yerindeki inek sayısı 2 veya 2’nin üzerinde ise onlardan birini alıp başka bir besi yemine götürebilir. 

Ancak bazı inekler çok uyuşuk olduklarından, sürekli yer değiştirmek istemiyorlar bu yüzden Serhat her bir ineğin yerini toplamda en fazla $C_i$ kadar değiştirebilir. Bu $C_i$ sayısı her inekte farklı olabilir. Serhat bu limite uyuduğu taktirde yukarıda belirtilen işlemi istediği inek üzerinde istediği kadar yapabilir. 

Serhat’ın yapması gereken şey ise tüm inekleri istedikleri besi yerine $B_i$ götürmek. Serhat’ın bu görevi başarıp başaramayacağını bulunuz ve eğer bunu başarabilirse en az kaç işlem yaparak başarabileceğini bulunuz.

## Input Format

İlk satır 2 integer $N$ ve $M$ ‘den oluşmaktadır. Onu takip eden $M$ satır ise 3 integer $A_i$, $B_i$ ve $C_i$’den oluşmaktadır. Bunlar:

- $N$ kaç tane besi yeri olduğunu, $M$ ise kaç tane inek olduğunu temsil etmektedir.
- $A_i$, $i$. ineğin hangi besi yerinde bulunduğunu temsil etmektedir.
- $B_i$, $i$. ineğin hangi besi yerinde yemek yemek istediğini temsil etmektedir.
- $C_i$, $i$. ineğin kaç kez hareket ettirilebileceğini temsil etmektedir.

## Output Format

Eger Serhat bu görevi başarabilirse en az kaç adımda başarabileceğini yazdırınız, aksi taktirde -1 yazdırınız.

## Constraints
$1 ≤ N ≤ 10^5$

$1 ≤ M ≤ 10^5$

$1 ≤ A_i, B-i ≤ N$

$1 ≤ C_i ≤ 10^5$

- İstenilen durum başarıldığında her bir besi yerinde 1 ya da daha fazla ineğin olması gerekiyor. Yani bütün i değerleri için ( $1 ≤ i ≤ N$ ),  $B_j = i$ esitligini saglayan  bir $j$ değeri olmalı.