
```dataviewjs
// lesson order
const lessons = ["Türkçe", "Tarih", "Coğrafya", "Felsefe", "Din", "Matematik", "Fizik", "Kimya", "Biyoloji"];

// put the real subject lists here later
const subjectMap = {
  "Türkçe": [
"Sözcükte Anlam",
"Cümlede Anlam",
"Paragrafta Anlatım Teknikleri",
"Paragrafta Düşünceyi Geliştirme Yolları",
"Paragrafta Yapı",
"Paragrafta Konu-Ana Düşünce",
"Paragrafta Yardımcı Düşünce",
"Ses Bilgisi",
"Yazım Kuralları",
"Noktalama İşaretleri",
"Sözcükte Yapı",
"Sözcük Türleri",
"Fiiller",
"Cümlenin Ögeleri",
"Cümle Türleri",
"Anlatım Bozukluğu"
],
"Tarih": [
"Tarih ve Zaman",
"İnsanlığın İlk Dönemleri",
"İlk ve Orta Çağlarda Türk Dünyası",
"İslam Medeniyetinin Doğuşu ve İlk İslam Devletleri",
"Türklerin İslamiyet’i Kabulü ve İlk Türk İslam Devletleri",
"Orta Çağ’da Dünya",
"Yerleşme ve Devletleşme Sürecinde Selçuklu Türkiyesi",
"Beylikten Devlete Osmanlı Siyaseti",
"Devletleşme Sürecinde Savaşçılar ve Askerler",
"Beylikten Devlete Osmanlı Medeniyeti",
"Dünya Gücü Osmanlı",
"Sultan ve Osmanlı Merkez Teşkilatı",
"Klasik Çağda Osmanlı Toplum Düzeni",
"Değişen Dünya Dengeleri Karşısında Osmanlı Siyaseti",
"Değişim Çağında Avrupa ve Osmanlı",
"Uluslararası İlişkilerde Denge Stratejisi (1774-1914)",
"Devrimler Çağında Değişen Devlet-Toplum İlişkileri",
"Sermaye ve Emek",
"XIX. ve XX. Yüzyılda Değişen Gündelik Hayat",
"XX. Yüzyıl Başlarında Osmanlı Devleti ve Dünya",
"Milli Mücadele",
"Atatürkçülük ve Türk İnkılabı"
],
"Coğrafya": [
"Doğa ve İnsan",
"Dünya’nın Şekli ve Hareketleri",
"Coğrafi Konum",
"Harita Bilgisi",
"İklim Bilgisi",
"Dünya’nın Tektonik Oluşumu",
"Jeolojik Zamanlar",
"İç Kuvvetler / Dış Kuvvetler",
"Kayaçlar",
"Türkiye’nin Yer Şekilleri",
"Su – Toprak ve Bitkiler",
"Nüfus",
"Türkiye’de Nüfus",
"Göç",
"Ekonomik Faaliyetler",
"Bölgeler",
"Uluslararası Ulaşım Hatları",
"Çevre ve Toplum",
"Doğal Afetler"
],
"Felsefe": [
"Felsefe’nin Konusu",
"Bilgi Felsefesi",
"Varlık Felsefesi",
"Ahlak Felsefesi",
"Sanat Felsefesi",
"Din Felsefesi",
"Siyaset Felsefesi",
"Bilim Felsefesi",
"İlk Çağ Felsefesi",
"2 . Yüzyıl ve 15. Yüzyıl Felsefeleri",
"15 . Yüzyıl ve 17. Yüzyıl Felsefeleri",
"18 . Yüzyıl ve 19. Yüzyıl Felsefeleri",
"20 . Yüzyıl Felsefesi"
],
"Din": [
"Bilgi ve İnanç",
"Din ve İslam",
"İslam ve İbadet",
"Gençlik ve Değerler",
"İslam Medeniyeti ve Özellikleri",
"Allah İnancı ve İnsan",
"Allah’ın Varlığı ve Birliği",
"Allah’ın İsim ve Sıfatları",
"Kur’an-ı Kerim’de İnsan ve Özellikleri",
"İnsanın Allah İle İrtibatı",
"Kur’an-ı Kerim’de Gençler",
"Bir Genç Olarak Hz. Muhammed",
"Hz. Muhammed ve Gençler",
"Bazı Genç Sahabiler",
"Din ve Aile",
"Din, Kültür ve Sanat",
"Din ve Çevre",
"Din ve Sosyal Değişim",
"Din ve Ekonomi",
"Din ve Sosyal Adalet",
"Ahlaki Tutum ve Davranışlar",
"İslam Düşüncesinde İtikadi, Siyasi ve Fıkhi Yorumlar"
],
"Matematik": [
"Temel Kavramlar",
"Sayı Basamakları",
"Bölme ve Bölünebilme",
"EBOB – EKOK",
"Rasyonel Sayılar",
"Basit Eşitsizlikler",
"Mutlak Değer",
"Üslü Sayılar",
"Köklü Sayılar",
"Çarpanlara Ayırma",
"Oran Orantı",
"Denklem Çözme",
"Sayı Problemleri",
"Kesir Problemleri",
"Yaş Problemleri",
"Yüzde Problemleri",
"Kar Zarar Problemleri",
"Karışım Problemleri",
"Hareket Problemleri",
"İşçi Problemleri",
"Tablo-Grafik Problemleri",
"Rutin Olmayan Problemleri",
"Kümeler",
"Mantık",
"Fonskiyonlar",
"Polinomlar",
"2.Dereceden Denklemler",
"Permütasyon ve Kombinasyon",
"Olasılık",
"Veri – İstatistik",
"Doğruda Açı",
"Üçgende Açı",
"Ek Çizimler",
"Özel Üçgenler",
"Açıortay",
"Kenarortay",
"Üçgende Eşlik – Benzerlik",
"Açı – Kenar Bağıntıları",
"Üçgende Alan",
"Üçgende Merkezler",
"Çokgenler",
"Dörtgenler",
"Deltoid",
"Paralelkenar",
"Eşkenar Dörtgen",
"Dikdörtgen",
"Kare",
"Yamuk",
"Çember ve Daire",
"Analitik Geometri",
"Katı Cisimler"
],
"Fizik": [
"Fizik Bilimine Giriş",
"Madde ve Özellikleri",
"Hareket ve Kuvvet",
"İş, Güç ve Enerji",
"Isı, Sıcaklık ve Genleşme",
"Basınç",
"Kaldırma Kuvveti",
"Elektrostatik",
"Elektrik ve Manyetizma",
"Dalgalar",
"Optik"
],
"Kimya": [
"Kimya Bilimi",
"Atom ve Periyodik Sistem",
"Kimyasal Türler Arası Etkileşimler",
"Maddenin Halleri",
"Doğa ve Kimya",
"Kimyanın Temel Kanunları",
"Kimyasal Hesaplamalar",
"Karışımlar",
"Asit, Baz ve Tuz",
"Kimya Her Yerde"
],
"Biyoloji": [
"Canlıların Ortak Özellikleri",
"Canlıların Temel Bileşenleri",
"Hücre ve Organelleri",
"Hücre Zarından Madde Geçişi",
"Canlıların Sınıflandırılması",
"Mitoz ve Eşeysiz Üreme",
"Mayoz ve Eşeyli Üreme",
"Kalıtım",
"Ekosistem Ekolojisi",
"Güncel Çevre Sorunları"
]
};

// initialize counts
const counts = {};
for (const lesson of lessons) {
  counts[lesson] = Array(subjectMap[lesson].length).fill(0);
}

// get pages with raw data
const pages = dv.pages().where(p => p.data);

for (const page of pages) {
  const lessonBlocks = String(page.data).split(";");

  lessonBlocks.forEach((block, lessonIndex) => {
    const lesson = lessons[lessonIndex];
    if (!lesson || !block.trim()) return;

    const nums = block
      .split(",")
      .map(n => Number(n.trim()))
      .filter(n => !isNaN(n));

    for (const n of nums) {
      const idx = n - 1;
      if (idx >= 0 && idx < counts[lesson].length) {
        counts[lesson][idx] += 1;
      }
    }
  });
}

// output: one row per lesson
const rows = lessons.map(lesson => {
  const subjectText = subjectMap[lesson]
    .map((sub, i) => `${sub}: ${counts[lesson][i]}`)

  return [lesson, subjectText];
});

dv.table(["Lesson", "Subjects"], rows);
```
deneme:: LEK TYT 4
data:: 1,1,9,5,7,7,1;15;8,5;10;;12,28;;8;9

deneme:: ESEN TYT 4
data:: 9
