# Nadi Sarı Mali Müşavirlik — Statik Web Sitesi

Soma/Manisa'da faaliyet gösteren **Serbest Muhasebeci Mali Müşavir Nadi Sarı**'nın tanıtım sitesi.
Orijinal WordPress (WordPress.com) sitesinden alınan içerikle, GitHub Pages'te barındırılmak üzere
hazırlanmış tamamen statik (HTML + CSS + JS) bir sitedir.

## Sayfalar

| Dosya | İçerik |
|---|---|
| `index.html` | Ana sayfa (hero, hizmet özetleri, kurum logoları, iletişim şeridi) |
| `hizmetler.html` | 5 hizmet alanının ayrıntılı anlatımı |
| `hakkimizda.html` | Mali Müşavir Nadi Sarı biyografisi ve çalışma ilkeleri |
| `iletisim.html` | Adres, telefon, e-posta, çalışma saatleri ve harita |
| `tevkifat-hesaplama.html` | Tevkifatlı fatura (KDV) hesaplama aracı |
| `404.html` | Sayfa bulunamadı ekranı |

## GitHub Pages'e Yayınlama

1. GitHub'da yeni bir **Public** repo açın (ör. `nadisari-sitesi`).
2. Bu klasörün içindeki tüm dosyaları repoya yükleyin:
   - **GitHub Desktop** kullanıyorsanız: `File → Add local repository` → bu klasörü seçin → `Publish repository`.
   - Ya da komut satırı ile:
     ```bash
     cd Documents/GitHub/nadisari-sitesi
     git init
     git add .
     git commit -m "İlk yükleme: Nadi Sarı Mali Müşavirlik statik sitesi"
     git branch -M main
     git remote add origin https://github.com/KULLANICIADI/nadisari-sitesi.git
     git push -u origin main
     ```
3. Repoda **Settings → Pages → Source: Deploy from a branch → main / root** seçip **Save**.
4. 2-3 dakika sonra site şu adreste yayında olur:
   `https://KULLANICIADI.github.io/nadisari-sitesi/`

> `.nojekyll` dosyası GitHub'ın Jekyll derlemesini devre dışı bırakır; silmeyin.

## Özelleştirme

- **Renkler:** `assets/css/style.css` içindeki `:root` değişkenlerinden (`--blue-600` marka laciverti).
- **İçerik:** Her sayfa doğrudan düzenlenebilir düz HTML'dir; derleme gerekmez.
- **Form:** İleride çalışır bir iletişim formu istenirse [Formspree](https://formspree.io) ücretsiz planıyla eklenebilir.

## İletişim Bilgileri

- 📞 0533 094 11 48
- ✉️ nadisari.smmm@gmail.com
- 🕘 Hafta içi 09.00 – 18.00

> Not: Ofis adresi geçici olarak siteden çıkarılmıştır (güncellenince `index.html`,
> `iletisim.html` ve tüm sayfa footer'larına yeniden eklenecektir). Harita görseli
> `assets/img/harita.png` içinde saklı durmaktadır.
