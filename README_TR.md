# AWS BuildID Otomatik Kayıt - Çok Dilli Destek

Bu fork, orijinal [AWS-BuildID-Auto-For-Ext](https://github.com/Specia1z/AWS-BuildID-Auto-For-Ext) projesine **çok dilli destek (i18n)** ekler.

## 🌍 Desteklenen Diller

- 🇨🇳 **Çince (Basitleştirilmiş)** - zh_CN (Varsayılan)
- 🇬🇧 **İngilizce** - en
- 🇹🇷 **Türkçe** - tr

## 📦 Kurulum

### Kaynak Koddan Kurulum

1. **Repoyu klonlayın:**
```bash
git clone https://github.com/[your-username]/AWS-BuildID-Auto-For-Ext.git
cd AWS-BuildID-Auto-For-Ext
```

2. **Chrome'da yükleyin:**
   - Chrome'u açın
   - `chrome://extensions/` adresine gidin
   - Sağ üstteki **"Geliştirici modu"** açın
   - **"Paketlenmemiş uzantı yükle"** tıklayın
   - Proje klasörünü seçin

3. **Gizli mod iznini etkinleştirin:**
   - Uzantı kartında **"Ayrıntılar"** tıklayın
   - **"Gizli modda izin ver"** seçeneğini açın
   - Uzantıyı yenileyin (🔄 simgesine tıklayın)

## 🌐 Dil Değiştirme

Uzantı, **tarayıcınızın dil ayarlarını** otomatik algılar:

### Chrome Dil Ayarları

1. Chrome Ayarlar → **Diller** (`chrome://settings/languages`)
2. **Tercih edilen diller** listesinde dilinizi en üste taşıyın
3. Chrome'u yeniden başlatın
4. Uzantı artık dilinizde görünecektir

### Desteklenen Dil Kodları

- `zh-CN`, `zh` → Çince
- `en`, `en-US`, `en-GB` → İngilizce
- `tr`, `tr-TR` → Türkçe
- Diğer diller → Çince (varsayılan)

## ✨ Orijinal Özellikler

Tüm orijinal özellikler korunmuştur:

- ✅ Yarı otomatik kayıt
- ✅ Toplu kayıt (1-100)
- ✅ Gmail sınırsız takma ad
- ✅ Gizli mod
- ✅ Token yönetimi
- ✅ Token doğrulama
- ✅ Kiro IDE senkronizasyonu

Detaylı kullanım için [orijinal dokümantasyona](https://github.com/Specia1z/AWS-BuildID-Auto-For-Ext) bakın.

## 🛠️ Geliştirici Notları

### i18n Yapısı

```
_locales/
├── zh_CN/
│   └── messages.json  # Çince çeviriler
├── en/
│   └── messages.json  # İngilizce çeviriler
└── tr/
    └── messages.json  # Türkçe çeviriler
```

### Yeni Dil Ekleme

1. `_locales/[dil_kodu]/messages.json` oluşturun
2. `zh_CN/messages.json` dosyasını kopyalayın
3. Tüm `message` değerlerini çevirin
4. Chrome'u yeniden başlatın

### Yeni Çeviri Anahtarı Ekleme

1. Tüm dil dosyalarına yeni anahtar ekleyin:
```json
{
  "yeniAnahtar": {
    "message": "Çevrilmiş metin"
  }
}
```

2. HTML'de kullanın:
```html
<span data-i18n="yeniAnahtar">Varsayılan metin</span>
```

3. JavaScript'te kullanın:
```javascript
const text = i18n('yeniAnahtar');
```

## 🤝 Katkıda Bulunma

Yeni dil çevirileri veya iyileştirmeler için pull request gönderin!

## 📄 Lisans

MIT License - Orijinal proje ile aynı

## 🙏 Teşekkürler

- Orijinal proje: [Specia1z/AWS-BuildID-Auto-For-Ext](https://github.com/Specia1z/AWS-BuildID-Auto-For-Ext)
- Chrome i18n API: [Chrome Extension i18n](https://developer.chrome.com/docs/extensions/reference/i18n/)

---

**Topluluk tarafından ❤️ ile yapıldı**
