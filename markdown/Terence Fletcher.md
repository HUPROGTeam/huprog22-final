# Terence Fletcher

Özgün davul çalmayı çok sevmektedir ve eğitmeni Akın'la beraber şarkılardaki davul ataklarını transkript etmek istiyordur. İnceleyecekleri atakların içeriği ve kuralları şöyledir:

- $L$ ve $R$ olmak üzere iki farklı seçenek — Sol el ve sağ el vuruşu
- Single stroke (tekli vuruş) — $L$ veya $R$
- Double stroke (çift vuruş) — $LL$ veya $RR$ 

içermektedir.

- Bir double stroke'tan sonra aynı el ile single / double stroke yapılamaz. (Aynı el ile yapılan ardışık iki single stroke (LL veya RR) double stroke olarak değerlendirilecektir)

Transkript işlemi çok basit olduğundan ötürü Akın, Özgün'e daha ilginç bir soru sormak ister. Bahsedilen kurallara göre oluşturulabilecek $N$ (inceledikleri ataktaki vuruş sayısı) vuruşluk atakları $L$ öncelikli olacak şekilde sıraladıktan sonra, transkript ettikleri atağın kaçıncı sırada olduğunu bulmasını istemektedir. Özgün'e cevabı bulmasında yardım edin.

Örneğin, $N=5$ için $LLRLR$, $LLRRL$, $LRLLR$, $LRLRL$, $LRLRR$, $LRRLL$, $LRRLR$, $RLLRL$, $RLLRR$, $RLRLL$, $RLRLR$, $RLRRL$, $RRLLR$ ve $RRLRL$ olacak şekilde 14 farklı atak oluşturulabilir. 

Büyük $N$ değerlerinde sonuç çok büyük olabileceğinden sonucu $K$ da modunu alıp bastırın.

## Input Format

İlk satırda $N$ tam sayısı — ataktaki vuruş sayısı

İkinci satırda $K$ tam sayısı — mod almak için kullanılacak sayı

Üçüncü satırda $N$ uzunluğunda string — sırası bulunmak istenen atak

## Output Format

Verilen atağın sırasını $K$'da modunu alarak bastırın.

## Constraints
- $1 \leq N \leq 10^6$
- $4 \leq K \leq 10^7$
- Verilen bir stringde yalnızca büyük L ve R harfleri bulunacaktır.