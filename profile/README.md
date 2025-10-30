### ASSISTANT
```markdown
# 📋 DAT IntelliJ Assistant

**DAT (Developer AI Tools) IntelliJ Assistant**, IntelliJ IDEA için geliştirilmiş, **Claude AI destekli**, **çift dil (Türkçe/İngilizce)** ve **gelişmiş kod analizi** özelliklerine sahip bir geliştirici yardımcısı eklentisidir.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![IntelliJ Plugin](https://img.shields.io/badge/IntelliJ-Plugin-orange.svg)](https://plugins.jetbrains.com/)
[![Kotlin](https://img.shields.io/badge/Kotlin-1.8+-blue.svg)](https://kotlinlang.org/)
[![Claude AI](https://img.shields.io/badge/Claude-4.0-purple.svg)](https://anthropic.com/)

---

## 🚀 Özellikler

### 🎯 Temel Özellikler
- **🧠 Claude AI Entegrasyonu** - Anthropic'in en gelişmiş modellerini kullanır
- **🌍 Çift Dil Desteği** - Türkçe ve İngilizce arayüz
- **📝 Kod Analizi** - Akıllı kod inceleme ve öneri sistemi
- **🔒 Güvenli API Yönetimi** - IntelliJ'nin PasswordSafe sistemi ile güvenli anahtar saklama
- **⚡ Hızlı Erişim** - Klavye kısayolları ile anında analiz

### 🛠️ Gelişmiş Özellikler
- **1M Token Bağlam Penceresi** - Büyük projelerde kapsamlı analiz
- **🤖 Oto-Onay Sistemi** - Güvenli kod değişiklikleri için otomatik onay
- **📊 Chat Arayüzü** - Kod hakkında interaktif sohbet
- **🎨 Modern UI** - IntelliJ'nin native arayüz bileşenleri
- **⚙️ Özelleştirilebilir Ayarlar** - Kişiselleştirilebilir yapılandırma

---

## 📦 Kurulum

### Yöntem 1: JetBrains Marketplace (Önerilen)
1. IntelliJ IDEA'yı açın
2. `File` → `Settings` → `Plugins`
3. `Marketplace` sekmesinde "DAT Assistant" arayın
4. `Install` butonuna tıklayın
5. IDE'yi yeniden başlatın

### Yöntem 2: Manuel Kurulum
1. [Releases sayfasından](https://github.com/survivorsdev/dat-intellij-assistant/releases) son sürümü indirin
2. `File` → `Settings` → `Plugins` → `⚙️` → `Install Plugin from Disk...`
3. İndirdiğiniz `.zip` dosyasını seçin
4. IDE'yi yeniden başlatın

---

## ⚙️ Yapılandırma

### API Anahtarı Kurulumu
1. [Anthropic Console](https://console.anthropic.com/)'a gidin
2. API anahtarınızı oluşturun
3. IntelliJ'de: `File` → `Settings` → `Tools` → `DAT Assistant`
4. API anahtarınızı girin ve ayarları kaydedin

### Temel Ayarlar
```
🔧 DAT Assistant Ayarları
├── 🔐 API Yapılandırması
│   ├── API Sağlayıcı: Anthropic
│   ├── API Anahtarı: [Güvenli şekilde saklanır]
│   ├── Temel URL: https://claude.gg (özelleştirilebilir)
│   └── 1M Bağlam Penceresi: ✅ Etkin
├── 🎯 Model Seçimi
│   ├── Claude Sonnet 4.5 (Önerilen)
│   ├── Claude 3 Opus
│   └── Claude 3 Sonnet
└── 🌍 Dil Ayarları
    ├── Türkçe (tr)
    └── English (en)
```

---

## 🎮 Kullanım

### 1. Kod Analizi
```kotlin
// Kodu seçin ve Ctrl+Alt+D'ye basın
fun calculateSum(a: Int, b: Int): Int {
    return a + b  // DAT bu kodu analiz edecek
}
```

**Yöntemler:**
- **Menü:** `Tools` → `DAT Assistant` → `Kodu Analiz Et`
- **Kısayol:** `Ctrl+Alt+D` (Windows/Linux) veya `Cmd+Alt+D` (Mac)
- **Sağ Tık:** Editörde sağ tık → `DAT ile Analiz Et`

### 2. Chat Arayüzü
1. Sağ kenardaki **DAT** panelini açın
2. Kod hakkında sorularınızı sorun
3. Gerçek zamanlı öneriler alın

### 3. Desteklenen Dosya Türleri
- ✅ **Java** - Tam destek
- ✅ **Kotlin** - Tam destek  
- ✅ **Python** - Tam destek
- ✅ **JavaScript/TypeScript** - Tam destek
- ✅ **C/C++** - Temel destek
- ✅ **Go** - Temel destek
- ✅ **Diğer diller** - Genel kod analizi

---

## 🏗️ Geliştirici Rehberi

### Proje Yapısı
```
src/main/kotlin/com/survivorsdev/dat/
├── 🎯 actions/          # IntelliJ aksiyonları
├── 🧠 core/            # Claude API ve temel servisler
├── 🎨 ui/              # Kullanıcı arayüzü bileşenleri
├── ⚙️ settings/        # Plugin ayarları
├── 🌍 i18n/           # Çoklu dil desteği
└── 🖥️ computer/       # Güvenli sistem erişimi
```

### Yerel Geliştirme
```bash
# Projeyi klonlayın
git clone https://github.com/survivorsdev/dat-intellij-assistant.git

# Proje dizinine gidin
cd dat-intellij-assistant

# Gradle ile build edin
./gradlew build

# Test IDE'yi çalıştırın
./gradlew runIde
```

### Testler
```bash
# Tüm testleri çalıştır
./gradlew test

# Sadece UI testleri
./gradlew test --tests "*UI*"

# Plugin doğrulaması
./gradlew verifyPlugin
```

---

## 📊 Model Karşılaştırması

| Model | Bağlam Penceresi | Max Çıktı | Görüntü Desteği | Fiyat (1M token) |
|-------|------------------|-----------|-----------------|------------------|
| **Claude Sonnet 4.5** ⭐ | 1.000.000 | 64.000 | ✅ | $6.00 / $22.50 |
| Claude 3 Opus | 200.000 | 4.096 | ✅ | $15.00 / $75.00 |
| Claude 3 Sonnet | 200.000 | 4.096 | ✅ | $3.00 / $15.00 |

> **💡 Öneri:** Günlük kullanım için **Claude Sonnet 4.5** ideal seçimdir.

---

## 🔒 Güvenlik

### Veri Gizliliği
- ✅ API anahtarları IntelliJ'nin güvenli kasasında saklanır
- ✅ Kod sadece analiz için Anthropic'e gönderilir
- ✅ Hiçbir kod yerel olarak saklanmaz
- ✅ GDPR ve veri koruma yönetmeliklerine uyumludur

### İzinler
```xml
<permissions>
  <!-- Sadece gerekli izinler -->
  <permission>Editor Access</permission>
  <permission>Project Files (Read Only)</permission>
  <permission>Network (API Calls)</permission>
  <permission>Settings Storage</permission>
</permissions>
```

---

## 🐛 Sorun Giderme

### Sık Karşılaşılan Sorunlar

#### ❌ "API Anahtarı Bulunamadı" Hatası
```
Çözüm:
1. Settings → Tools → DAT Assistant
2. Geçerli bir Anthropic API anahtarı girin
3. "Test Connection" ile bağlantıyı doğrulayın
```

#### ❌ "Model Yanıt Vermiyor"
```
Kontrol Listesi:
□ İnternet bağlantınız aktif mi?
□ API anahtarınızda yeterli kredi var mı?
□ Seçili metin çok büyük değil mi? (1M token sınırı)
□ Anthropic servisleri çalışıyor mu?
```

#### ❌ "Plugin Yüklenmiyor"
```
Adımlar:
1. IntelliJ sürümünüz 2023.1+ olmalı
2. Plugin'i deaktif edip tekrar aktif edin
3. IDE'yi tamamen yeniden başlatın
4. Sorun devam ederse logları kontrol edin
```

### Debug Modu
```kotlin
// Debug logları etkinleştir
System.setProperty("dat.debug", "true")
```

### Log Dosyaları
- **Windows:** `%APPDATA%\JetBrains\IntelliJIdea\log\idea.log`
- **macOS:** `~/Library/Logs/JetBrains/IntelliJIdea/log/idea.log`
- **Linux:** `~/.cache/JetBrains/IntelliJIdea/log/idea.log`

---

## 🤝 Katkıda Bulunma

### Geliştirme Süreci
1. 🍴 Projeyi fork edin
2. 🌿 Feature branch oluşturun: `git checkout -b feature/amazing-feature`
3. 📝 Değişikliklerinizi commit edin: `git commit -m 'Add amazing feature'`
4. 📤 Branch'inizi push edin: `git push origin feature/amazing-feature`
5. 🔄 Pull Request oluşturun

### Kod Standartları
```kotlin
// Kotlin coding standards
class ExampleService {
    companion object {
        private const val DEFAULT_TIMEOUT = 30_000L
    }
    
    fun processCode(code: String): Result<String> {
        // Implementation
    }
}
```

### Commit Mesajları
```
feat: yeni özellik eklendi
fix: bug düzeltildi  
docs: dokümantasyon güncellendi
style: kod formatlaması
refactor: kod yeniden düzenlendi
test: test eklendi
chore: proje yapılandırması
```

---

## 📝 Değişiklik Geçmişi

### v1.2.0 (2024-11-01)
- ✨ Claude Sonnet 4.5 model desteği
- 🌍 Gelişmiş Türkçe yerelleştirme
- 🔧 1M token bağlam penceresi
- 🐛 API timeout sorunları düzeltildi

### v1.1.0 (2024-10-15)
- ✨ Chat arayüzü eklendi
- ⚙️ Oto-onay sistemi
- 🎨 UI iyileştirmeleri
- 📊 Model karşılaştırma tablosu

### v1.0.0 (2024-10-01)
- 🎉 İlk stabil sürüm
- 🧠 Claude AI entegrasyonu
- 🌍 Türkçe/İngilizce destek
- 📝 Kod analizi özellikleri

---

## 📞 Destek

### İletişim Kanalları
- 📧 **Email:** ben@survivorsdev.com
- 🐛 **Bug Reports:** [GitHub Issues](https://github.com/survivorsdev/dat-intellij-assistant/issues)
- 💬 **Discord:** [SurvivorsDev Community](https://discord.gg/survivorsdev)
- 📚 **Dokümantasyon:** [Wiki](https://github.com/survivorsdev/dat-intellij-assistant/wiki)

### Topluluk
- ⭐ **GitHub Stars:** Bu projeyi desteklemek için yıldız verin
- 🔄 **Contributions:** Katkıda bulunun ve geliştirin
- 📢 **Feedback:** Görüşlerinizi paylaşın

---

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır.

```
MIT License

Copyright (c) 2024 SurvivorsDev

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

---

## 🙏 Teşekkürler

- **Anthropic** - Claude AI API'si için
- **JetBrains** - IntelliJ Platform için
- **Kotlin Community** - Harika dil ve araçlar için
- **Katkıda Bulunanlar** - Projeyi geliştiren herkese

---

<div align="center">

**DAT IntelliJ Assistant ile kodlama deneyiminizi yükseltin! 🚀**

[⬇️ İndir](https://github.com/survivorsdev/dat-intellij-assistant/releases) • [📚 Dokümantasyon](https://github.com/survivorsdev/dat-intellij-assistant/wiki) • [🐛 Sorun Bildir](https://github.com/survivorsdev/dat-intellij-assistant/issues)

Made with ❤️ by [SurvivorsDev](https://survivorsdev.com)

</div>
```

Bu DAT_Asistan_README.md dosyasını projenizin ana dizinine `DAT_Asistan_README.md` olarak kaydedebilirsiniz. Dosya GitHub'da otomatik olarak güzel bir şekilde formatlanacaktır.
![image](https://www.sourcexchange.net/storage/1360/01J5RAWJE2ZRRB680Z2Z7YVNAY.jpg)
