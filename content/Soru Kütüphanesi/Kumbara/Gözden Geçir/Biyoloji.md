
## TYT
#tyt_biyoloji

### Biyoanaliz
#tyt_biyoloji_biyoanaliz 

#### Canlıların Ortak Özellikleri
#tyt_biyoloji_canlıların_ortak_özellikleri
13-2
15-1
19-1

#### Temel Bileşenler
#tyt_biyoloji_temel_bileşenler
30-8
31-1
36-10
39-2,6
47-4
49-3
50-11
56-7
57-7

#### Hücre
#tyt_biyoloji_hücre
70-7
71-1
86-7
88-11
90-10
97-4
101-3
104-8

#### Sınıflandırma
#tyt_biyoloji_sınıflandırma
120-4,7
125-4
126-9
127-3
128-9
131-2
135-7
137-2
146-10
147-5
148-7
150-7,11

#### Hücre Bölünmeleri
#tyt_biyoloji_hüre_bölünmeleri
163-2
165-5
166-10
167-3,4
170-8
174-6
181-1
183-5
186-8,9

#### Kalıtım
#tyt_biyoloji_kalıtım
196-4
198-6
199-1
200-9
201-4
203-7
207-2,3
212-7
223-4
227-1

#### Ekoloji
#tyt_biyoloji_ekoloji
240-6,9
243-3
251-2
255-2


### Biyoanaliz Branş Denemesi
#tyt_biyoloji_biyoanaliz_branş

```dataviewjs
const konular = [  
"Canlıların Ortak Özellikleri",  
"Temel Bileşikler",  
"Hücre",  
"Sınıflandırma",  
"Hücre Bölünmeleri",  
"Kalıtım",  
"Ekoloji"  
];

let file = app.vault.getAbstractFileByPath(dv.current().file.path);
let raw = await app.vault.read(file);

let matches = raw.match(/\d+-\d+-\d+/g) ?? [];

let counts = Array(7).fill(0);

for (let h of matches) {
  let konu = parseInt(h.split("-")[2]) - 1;
  if (konu >= 0 && konu < 7) counts[konu]++;
}

dv.table(
["Konu", "Soru"],
konular.map((k, i) => [k, counts[i]])
);
```

{deneme no} - {soru no} - {konu no}
1-2-2
3-2-4
9-3-5
11-1-4
13-1-7
14-3-5
16-6-4
17-3-5 *
17-6-3
18-4-7

