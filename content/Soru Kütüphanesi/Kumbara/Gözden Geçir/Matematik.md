
# AYT 
#ayt_mat

### Barış Fonksiyon Logaritma Dizi
#ayt_mat_barış_fonk_deneme

```dataviewjs
const sectionHeader = "Barış Fonksiyon Logaritma Dizi";

const konular = [
  "Foksiyonlar",
  "Logaritma",
  "Dizi"
];

const file = app.vault.getAbstractFileByPath(dv.current().file.path);
const raw = await app.vault.read(file);
const lines = raw.split("\n");

// find the exact ### header
const start = lines.findIndex(line => line.trim() === `### ${sectionHeader}`);

if (start === -1) {
  dv.paragraph(`Section not found: ${sectionHeader}`);
  return;
}

// stop at the next heading of any level
let end = lines.length;
for (let i = start + 1; i < lines.length; i++) {
  if (/^#{1,6}\s+/.test(lines[i])) {
    end = i;
    break;
  }
}

const sectionText = lines.slice(start + 1, end).join("\n");
const matches = sectionText.match(/\d+-\d+-\d+/g) ?? [];

let counts = Array(konular.length).fill(0);

for (let h of matches) {
  const konu = parseInt(h.split("-")[2]) - 1;
  if (konu >= 0 && konu < counts.length) counts[konu]++;
}

dv.table(
  ["Konu", "Soru"],
  konular.map((k, i) => [k, counts[i]])
);
```

{deneme no} - {soru no} - {konu no}
1-5-2 *
1-12-3
2-1-1
2-2-1
2-3-1
2-9-2
3-2-1
3-5-2
4-5-2
5-3-1
5-9-3
7-5-2 *
7-9-3 *
8-2-1 *
8-9-3
9-5-2
10-1-1
11-4-1 *
11-7-2
12-12-3
13-2-1
13-3-1
13-5-2
14-2-1
14-11-3
15-7-2 *
15-8-2 *
15-12-3 *
16-5-2
16-6-2
17-3-1
18-4-1 *
18-6-2
18-9-2
18-12-3
19-5-1 *
19-7-2
19-10-3
19-12-3

### Barış Polinom, 2° Denklemler, Karmaşık Sayılar, Parabol, 2° Eşitsizlikler Denemeleri
#ayt_mat_barış_pol_deneme

```dataviewjs
const sectionHeader = "Barış Polinom, 2° Denklemler, Karmaşık Sayılar, Parabol, 2° Eşitsizlikler Denemeleri";

const konular = [
  "Polinomlar",
  "2° Denklemler",
  "Karmaşık Sayılar",
  "Parabol",
  "2° Eşitsizlikler"
];

const file = app.vault.getAbstractFileByPath(dv.current().file.path);
const raw = await app.vault.read(file);
const lines = raw.split("\n");

// find the exact ### header
const start = lines.findIndex(line => line.trim() === `### ${sectionHeader}`);

if (start === -1) {
  dv.paragraph(`Section not found: ${sectionHeader}`);
  return;
}

// stop at the next heading of any level
let end = lines.length;
for (let i = start + 1; i < lines.length; i++) {
  if (/^#{1,6}\s+/.test(lines[i])) {
    end = i;
    break;
  }
}

const sectionText = lines.slice(start + 1, end).join("\n");
const matches = sectionText.match(/\d+-\d+-\d+/g) ?? [];

let counts = Array(konular.length).fill(0);

for (let h of matches) {
  const konu = parseInt(h.split("-")[2]) - 1;
  if (konu >= 0 && konu < counts.length) counts[konu]++;
}

dv.table(
  ["Konu", "Soru"],
  konular.map((k, i) => [k, counts[i]])
);
```

1-2-1
1-6-2
1-13-3
2-1-1
2-3-1
2-7-2
2-9-4
3-3-1
4-1-1
4-5-2 *
4-6-2 *
4-9-4
5-1-1
5-4-2
5-6-2
7-3-1
7-6-2 *
7-7-4
8-1-1 *
8-8-4 *
9-1-1
10-2-1
10-9-4 *
10-11-5 *
11-7-2
11-8-4
11-9-4 *
12-1-1
12-12-2 *
13-5-2
13-7-4
14-3-1
14-6-2
14-7-4
14-8-4
14-12-5
15-2-1
15-4-2
15-6-2
15-11-5
16-2-1
16-4-2
16-5-2
16-8-4
16-11-5
17-2-1
17-6-2
17-7-4
18-2-1 *
18-5-2
18-12-5
18-13-3
19-1-1
19-9-4 *

## Orjinal AYT


# TYT
