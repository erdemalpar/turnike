# Turnike Geçiş ve Analiz Sistemi

Turnike Geçiş ve Analiz Sistemi, kurum veya şirketinizdeki PDF formatlı turnike raporlarını, dışarıya veri aktarmadan doğrudan tarayıcınızda (`pdf.js` ile) analiz eden; personellerin geliş/gidiş, geç kalma, erken çıkma, fazla mesai ve izin durumlarını otomatik hesaplayan gelişmiş bir web uygulamasıdır. 

## 🚀 Canlı Demo (Live Demo)

Projeyi doğrudan tarayıcı üzerinden test etmek ve kullanmak için aşağıdaki bağlantıyı ziyaret edebilirsiniz:

👉 **[Turnike Sistemi - Canlı Demo (GitHub Pages)](https://erdemalpar.github.io/turnike/)**

---

## ✨ Özellikler

*   **PDF Parse & Analiz:** Harici bir veritabanı veya sunucuya gerek kalmadan, tamamen tarayıcınız üstünde saniyeler içinde binlerce satır PDF analiz edilir.
*   **Otomatik Dizin Okuma (Localhost):** Proje dizininde yer alan `turnike_kayıt` klasörüne PDF raporları attığınızda, uygulama localhost'ta (örn: `npx serve` ile) ayağa kalktığında oradaki tüm dosyaları otomatik çeker.
*   **Akıllı Personel Eşleşmesi:** Kişiler listeye dahil edildiği an (sonradan eklenseler bile) daha önceden işlenmiş olan raporlardaki bilgileri geriye dönük olarak taranıp sisteme getirilir.
*   **İnteraktif Takvim Filtresi:** Sol tarafta bulunan `MiniCalendar` takvim bileşeninden belirli bir günü seçerek, o tarihteki tüm hareketlilik geçmişini tek tıkla filtreleyebilirsiniz.
*   **Arayüzden Yönetim ve Tolerans Ayarları:** Normal mesai ve öğle arası başlangıç/bitiş saatlerini ve tahammül (tolerans) sürelerini dinamik olarak değiştirebilir, arayüzden kişi listeleyebilir, anında isim düzenleyip silebilirsiniz.

## 💻 Kurulum ve Çalıştırma (Lokal Ortam)

Projeyi kendi bilgisayarınızda çalıştırmak için yalnızca herhangi bir statik Web sunucusuna ihtiyacınız vardır.

### Adımlar

1.  Repoyu bilgisayarınıza indirin (clone):
    ```bash
    git clone https://github.com/erdemalpar/turnike.git
    cd turnike
    ```
2.  (Opsiyonel) Otomatik okuma sistemini kullanmak istiyorsanız kök dizinde, örnek raporlarınızın olduğu bir `turnike_kayıt` klasörü oluşturun.
3.  Statik bir sunucu vasıtasıyla projeyi başlatın:
    *   **Python kullanıyorsanız:**
        ```bash
        python -m http.server 8000
        ```
    *   **Node.js (NPM) kullanıyorsanız:**
        ```bash
        npx serve
        ```
    *   VEYA kod editörünüzden (örn: VS Code) *Live Server* eklentisiyle çalıştırın.
4.  Konsolunuzda veya tarayıcınızda yazan adresi (Örn: `http://localhost:3000`) açarak kullanıma başlayabilirsiniz.

---
*Bu sistem vanilla JavaScript (React kütüphaneleri dahil edilerek) ile kodlanmış ve **TailwindCSS** kullanarak modern bir arayüzle giydirilmiştir.*
