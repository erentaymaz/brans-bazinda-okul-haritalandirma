# Branş Bazında Okul Haritalandırma

Bu proje, öğretmen adaylarının atama döneminde ihtiyaç duyduğu okul listelerini tek bir harita üzerinde interaktif şekilde görüntülemesini sağlayan bir uygulamadır. Millî Eğitim Bakanlığı tarafından paylaşılan branşa özel okul listeleri temel alınarak okulların konum bilgileri işlenir ve harita üzerinde görselleştirilir.

okulharitalandirma.netlify.app

## 🎯 Proje Hakkında

Önceki Python tabanlı Server-Side Rendering (SSR) projesinin eksiklerinden yola çıkılarak geliştirilmiş bu uygulama, Next.js ile **Static Site Generation (SSG)** kullanarak tamamen statik olarak üretilmektedir. Bu sayede:

- ⚡ **Daha hızlı yükleme süreleri** - Tüm sayfalar build zamanında oluşturulur
- 🚀 **Daha iyi performans** - Statik dosyalar CDN'lerde kolayca cache'lenebilir
- 💰 **Düşük hosting maliyetleri** - Herhangi bir statik hosting servisinde çalışabilir
- 🔒 **Daha güvenli** - Sunucu tarafında kod çalıştırma gerektirmez

## ✨ Özellikler

- ✅ **Tek Harita Üzerinde Tüm İlçeler** - Tüm okullar tek bir harita üzerinde görüntülenir
- ✅ **İlçe Bazlı Filtreleme** - Sağ üst köşedeki filtreleme alanı ile seçilen ilçedeki okullar görüntülenir
- ✅ **İnteraktif Harita** - OpenStreetMap ve Leaflet kullanılarak oluşturulmuş interaktif harita
- ✅ **Okul Detayları** - Marker'lara tıklanarak okul bilgileri görüntülenir
- ✅ **Otomatik Zoom** - Seçilen ilçedeki okullara otomatik zoom yapılır
- ✅ **Static Site Generation (SSG)** - Build zamanında tamamen statik HTML oluşturulur
- ✅ **TypeScript Desteği** - Tip güvenliği ile geliştirilmiştir
- ✅ **Responsive Tasarım** - Mobil ve masaüstü cihazlarda uyumlu çalışır

## 🛠️ Teknolojiler

- **Next.js 14** - React framework (SSG)
- **React 18** - UI kütüphanesi
- **TypeScript** - Tip güvenliği
- **Leaflet** - Harita kütüphanesi
- **React-Leaflet** - React için Leaflet wrapper'ı
- **OpenStreetMap** - Harita tile sağlayıcısı

## 📋 Gereksinimler

- Node.js 18.x veya üzeri
- npm veya yarn

## 🚀 Kurulum

1. **Projeyi klonlayın:**

```bash
git clone <repository-url>
cd brans-bazinda-okul-haritalandirma
```

2. **Bağımlılıkları yükleyin:**

```bash
npm install
```

3. **Geliştirme modunda çalıştırın:**

```bash
npm run dev
```

Uygulama şu adreste çalışacak: http://localhost:3000

## 📦 Build ve Production

### Statik Site Oluşturma

Proje SSG modunda çalıştığı için build zamanında tamamen statik dosyalar oluşturulur:

```bash
npm run build
```

Build edilen statik dosyalar `out` klasöründe oluşturulur. Bu dosyalar herhangi bir statik hosting servisine deploy edilebilir.

### Production Modunda Çalıştırma

```bash
npm run build
npm start
```



## 🗺️ Kullanım

1. **Ana Sayfa:** Tüm okullar haritada gösterilir
2. **İlçe Filtreleme:** Sağ üst köşedeki dropdown menüden ilçe seçerek sadece o ilçedeki okulları görüntüleyebilirsiniz
3. **Okul Detayları:** Haritadaki marker'lara tıklayarak okul bilgilerini görüntüleyebilirsiniz
4. **Harita Navigasyonu:** Mouse ile sürükleyerek haritayı hareket ettirebilir, zoom yapabilirsiniz

## 📊 Veri Formatı

Okul verileri `okullar-gaziantep.json` dosyasında saklanmaktadır. Her okul şu bilgileri içerir:

```json
{
  "id": 735292,
  "adi": "Kazım Karabekir İlkokulu",
  "il": "GAZİANTEP",
  "ilce": "ŞAHİNBEY",
  "latitude": "37.046139",
  "longitude": "37.400639",
  "zorunlu_hizmet": "1/5"
}
```

## 🔄 Önceki Projeden Farklar

### Python SSR → Next.js SSG

**Önceki Proje (Python SSR):**
- Server-side rendering kullanıyordu
- Her istekte sunucu tarafında render ediliyordu
- API endpoint'leri gerektiriyordu
- Sunucu maliyeti yüksekti

**Yeni Proje (Next.js SSG):**
- Static Site Generation kullanıyor
- Build zamanında tamamen statik HTML oluşturuluyor
- API endpoint'leri gerektirmiyor
- Herhangi bir statik hosting'de çalışabilir
- Daha hızlı ve daha ucuz

### Yeni Özellikler

- ✅ Tek harita üzerinde tüm ilçelerin görüntülenmesi
- ✅ Sağ üst köşede ilçe bazlı filtreleme
- ✅ Daha iyi performans ve hız
- 

## 🤝 Katkıda Bulunma

Pull request'ler memnuniyetle karşılanır! Büyük değişiklikler için lütfen önce bir issue açarak neyi değiştirmek istediğinizi tartışalım.

Bu proje, öğretmen adaylarının atama sürecinde okul seçimlerini kolaylaştırmak amacıyla geliştirilmiştir.




