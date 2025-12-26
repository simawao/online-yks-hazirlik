# YKS Hazırlık Platformu 📚 | SEBA Akademi

Modern ve kullanıcı dostu bir YKS (Yükseköğretim Kurumları Sınavı) hazırlık platformu. Öğrenciler video dersler izleyebilir, konuları takip edebilir ve testler çözebilir. Admin paneli üzerinden tüm içerikler yönetilebilir.

![Platform Screenshot](https://img.shields.io/badge/Platform-YKS%20Hazırlık-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🚀 Hızlı Başlangıç

### Projeyi Çalıştırma

⚠️ **Önemli:** YouTube videoları `file://` protokolünden çalışmaz. Local server kullanmanız gerekir.

```bash
# Proje klasöründe terminal açın
cd yks-hazirlik-platformuaaa

# Python server başlatın (port 8000)
python -m http.server 8000

# Tarayıcıda açın
# http://localhost:8000
```

---

## 👤 Demo Hesaplar

| Rol | E-posta | Şifre |
|-----|---------|-------|
| 🎓 Öğrenci | ogrenci@yks.com | ogrenci123 |
| 👨‍💼 Yönetici | admin@yks.com | admin123 |

---

## 📋 Özellikler

### 🎓 Öğrenci Paneli
- TYT/AYT kategorilerine göre ders seçimi
- Konu bazlı video izleme
- VBO (Video İzleme Oranı) takibi
- İlerleme göstergeleri
- Konu testi çözme

### 👨‍💼 Admin Paneli
- **İçerik Yönetimi:** Birleşik konu ve video yönetimi
- **Konu Sıralama:** ↑↓ butonları ile sıra değiştirme
- **Konu Ekleme/Düzenleme/Silme**
- **Video Ekleme:** YouTube ID, süre (MM:SS formatı)
- **Anlık Güncelleme:** Değişiklikler hemen yansır
- **Sekme Kalıcılığı:** Sayfa yenilenince son sekme hatırlanır
- **Özel Onay Kutuları:** Şık tasarımlı silme onayları
- **Toast Bildirimleri:** Modern bildirim sistemi

---

## 📁 Proje Yapısı

```
yks-hazirlik-platformuaaa/
├── index.html              # Ana sayfa
├── login.html              # Giriş sayfası
├── register.html           # Kayıt sayfası
├── student_dashboard.html  # Öğrenci paneli
├── admin_dashboard.html    # Yönetici paneli ⭐
├── courses.html            # Ders listesi (TYT/AYT)
├── topics.html             # Konu listesi
├── lesson.html             # Video ders sayfası
├── test.html               # Test sayfası
├── catalog.html            # Ders kataloğu
├── features.html           # Özellikler sayfası
├── faq.html                # SSS sayfası
├── seba.png                # Logo
└── README.md               # Bu dosya
```

---

## 🎬 Admin Paneli - İçerik Yönetimi

### Konu Ekleme
1. Admin panele giriş yapın (admin@yks.com / admin123)
2. **📚 İçerik Yönetimi** sekmesine gidin
3. TYT/AYT ve ders seçin
4. **+ Konu Ekle** butonuna tıklayın
5. Formu doldurun ve **Kaydet**

### Video Ekleme
1. Konu listesinden bir konu seçin (tıklayın)
2. **+ Video Ekle** butonuna tıklayın
3. YouTube Video ID girin (örn: `dQw4w9WgXcQ`)
4. Süre formatı: `15:30` veya `1:25:30`
5. **Kaydet**

### Konu Sıralama
- ↑ Yukarı taşı
- ↓ Aşağı taşı
- Değişiklikler öğrenci sayfasında da yansır

---

## 🛠️ Teknolojiler

- **HTML5** - Yapı
- **CSS3** - Stil (Glassmorphism, Dark Theme, Animations)
- **JavaScript (Vanilla)** - Etkileşim
- **YouTube Embed API** - Video oynatma
- **LocalStorage** - Veri saklama

---

## 📐 Form Validasyonları

| Alan | Kural |
|------|-------|
| Konu Başlığı | Boş bırakılamaz |
| Video Başlığı | Boş bırakılamaz |
| YouTube ID | Boş bırakılamaz |
| Süre | MM:SS veya HH:MM:SS formatı (`15:30`, `1:25:30`) |

---

## ⚠️ Sık Karşılaşılan Sorunlar

### Video yüklenmiyor
- Local server kullanın: `python -m http.server 8000`
- Video ID'nin doğru olduğunu kontrol edin
- Video'nun embed'e açık olduğundan emin olun

### Admin değişiklikleri öğrencide görünmüyor
- LocalStorage'daki `adminTopics` ve `adminVideos` verilerini kontrol edin
- Sayfa önbelleğini temizleyin (Ctrl+Shift+R)

---

## 📄 Lisans

Bu proje eğitim amaçlıdır. SEBA Akademi © 2024-2025
