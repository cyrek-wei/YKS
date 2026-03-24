### Deneme Deposu Dil Bilgisi
#türkçe_dil_bilgisi_deneme_deposu

```dataviewjs
const konular = [
"Ses",
"Yazım",
"Noktalama",
"Ad",
"Sıfat",
"Zamir",
"Zarf",
"Edat",
"Bağlaç",
"Ünlem",
"Fiiller",
"Ek Fiiller",
"Fiilimsiler",
"Çatı-Nesne-Özne",
"Cümlenin Ögeleri",
"Cümle Türleri",
"Sözcük Yapısı"
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
1-5-1
1-7-1
2-2-2
2-3-2
3-1-3
3-7-3 *
4-6-3 *
4-7-2 *
4-10-3 *
5-2-2
5-10-2
6-7-4
7-3-5 *
7-5-5
8-4-6
11-1-9
11-3-9
11-5-9
12-10-10
13-5-8
15-6-8


