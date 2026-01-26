# 🎬 Product to Social Media Video Generator (2026 Edition)

**Professional AI Video Automation by xCodeWraith DEV.**

Bu workflow, tek bir ürün fotoğrafından profesyonel, sosyal medya odaklı (9:16) reklam videoları üretir. İçerisinde en son AI teknolojilerini (Gemini 2.5, Kling 2.6, Fal AI) barındıran "Enterprise-Grade" bir otomasyondur.

## 🚀 Özellikler

- **Görsel Analiz (Gemini 2.5 Pro):** Ürün fotoğrafını analiz eder, marka kimliğine uygun senaryo yazar.
- **Sinematik Hareket (Kling 2.6 Motion):** Statik görseli profesyonel kamera hareketleriyle (Push-in, Orbit) canlandırır.
- **Ses Tasarımı (Fal Audio v2):** Markaya uygun arkaplan müziği ve ses efektleri (ASMR, Ambient) üretir.
- **Otomatik Kurgu (FFmpeg):** Parçaları birleştirir, geçişleri ayarlar ve final videoyu render eder.
- **İnsan Onayı (Telegram):** Üretim aşamasında Telegram üzerinden size önizleme sunar ve onay bekler.

## 🛠️ Gereksinimler

Bu workflow'u çalıştırmak için aşağıdaki n8n credential'larına ihtiyacınız var:

1. **Telegram API:** Bot token'ı. (Onay mekanizması için)
2. **Google Gemini API:** `gemini-2.5-pro` model erişimi.
3. **Fal.ai API:** Kling ve Audio modelleri için.
4. **ImgBB API:** Geçici görsel barındırma için.

## ⚙️ Kurulum

1. **Dosyayı İçe Aktarın:**
   - n8n arayüzünde "Import from File" diyerek `product_video_workflow.json` dosyasını seçin.

2. **Credential'ları Ayarlayın:**
   - Kırmızı yanan node'lara tıklayıp API anahtarlarınızı girin.

3. **Telegram Botunu Başlatın:**
   - Botunuza `/start` komutunu gönderin.

4. **Çalıştırın:**
   - "Execute Workflow" butonuna basın.
   - Telegram botuna ürün fotoğrafınızı gönderin.

## 🤖 Nasıl Çalışır?

1. **Input:** Telegram'dan ürün fotoğrafını alır.
2. **Director Agent:** "Art Director" ve "Motion Designer" ajanları görseli analiz eder ve 2 farklı konsept çıkarır.
3. **Gen:** Kling AI ile 2 farklı 5 saniyelik video üretilir.
4. **Sound:** Videonun atmosferine uygun müzik bestelenir.
5. **Output:** FFmpeg ile birleştirilmiş final video Telegram'dan size döner.

---

> **Not:** Bu workflow 2026 standartlarına göre optimize edilmiştir. Eski node tipleri güncellenmiş ve performans iyileştirmeleri yapılmıştır.

**Developer:** xCodeWraith DEV.
# XCodeWraith-Edition
