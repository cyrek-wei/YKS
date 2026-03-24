## AYT
#ayt_fizik

### ESŞ Fizik
#ayt_fizik_esş

Vektörler
#ayt_fizik_vektörler
17-2

İş Güç Enerji
#ayt_fizik_enerji
56-5
62-6

İtme ve Momentum
#ayt_fizik_momentum
67-1
68-6

Basit Makineler
#ayt_fizik_basit_makineler
89-2

Elektrik Alan
#ayt_fizik_elektrik_manyetizma
96-8
97-1,4

Manyetik Alan
#ayt_fizik_elektrik_manyetizma 
112-5
113-2

Alternatif Akım
#ayt_fizik_elektrik_manyetizma 
122-5
124-8
126-8

Çembersel Hareket
#ayt_fizik_çembersel_hareket
129-2
131-1
132-5
136-7
141-1
142-7

Kepler
#ayt_fizik_kepler
149-3
153-3,4
154-8
156-8
160-7

Dalga Mekaniği
#ayt_fizik_dalgalar
165-4
170-6

Radyoaktivite
#ayt_fizik_radyoaktivite
188-9

Fotoelektrik Olay
#ayt_fizik_fotoeletrik_olay
197-4

Modern Fizik Uygulamaları
#ayt_fizik_modern_fizik
205-3
206-7
210-8

### Apotemi Modern Fizik
#ayt_fizik_apotemi_modern_fizik

Çembersel Hareket
23-5
24-9
26-9,10
28-11
31-5
32-7,9
33-1
40-6
41-3
42-5,6,7
45-2,4,5
48-10
49-3
50-6
51-3,4
55-4,6
56-7
60-7

Harmonik Hareket
78-7
84-9


## TYT
#tyt_fizik

### ESŞ Branş Denemesi
#tyt_fizik_esş_branş

```dataviewjs
const konular = [
"Fizik Bilimine Giriş",
"Madde ve Özellikleri",
"Hareket",
"Kuvvet",
"Enerji",
"Isı Sıcaklık",
"Elektrostatik",
"Devreler",
"Manyetizma",
"Basınç",
"Kaldırma Kuvveti",
"Dalgalar",
"Aydınlanma",
"Aynalar",
"Işığın Kırılması",
"Mercekler",
"Renk ve Prizma"
];

let file = app.vault.getAbstractFileByPath(dv.current().file.path);
let raw = await app.vault.read(file);

let matches = raw.match(/\d+-\d+-\d+/g) ?? [];

let counts = Array(17).fill(0);

for (let h of matches) {
  let konu = parseInt(h.split("-")[2]) - 1;
  if (konu >= 0 && konu < 17) counts[konu]++;
}

dv.table(
["Konu", "Soru"],
konular.map((k, i) => [k, counts[i]])
);
```

{deneme no} - {soru no} - {konu no}
1-1-1
2-2-4
3-3-5
3-4-6
4-1-1
4-5-12
5-7-15
8-2-7
8-6-14
10-3-5
11-1-1
11-3-5
15-7-9

