# Verda: Yapay Zeka Tabanlı Mobil Ziraat Asistanı

Bu repository, **Verda: Bitki Hastalıkları Teşhis Sistemi**'nin Flutter ile geliştirilmiş mobil uygulamasını barındırmaktadır. Çiftçilerin tarlada yaprak fotoğraflarını çekerek hastalıkları saniyeler içinde teşhis etmesine, organik koruma reçetelerine ulaşmasına ve yapay zeka destekli ziraat asistanıyla sohbet etmesine olanak tanır.

---

## 📱 Öne Çıkan Özellikler

*   **Yapay Zeka Destekli Kamera Tarayıcı (AI Diagnosis):** Cihazın kamerasını kullanarak yaprak fotoğraflarını yakalar, bunları Django API'sine gönderir ve anlık hastalık teşhisi sunar.
*   **Açıklanabilir Yapay Zeka (XAI) Entegrasyonu:** Teşhis sonuçlarında, yapay zekanın yaprağın hangi lezyonlu noktasına odaklandığını gösteren Grad-CAM ısı haritası görselleştirmelerini sunar.
*   **Ziraat Asistanı (AI Chat):** Bitki sağlığı, sulama, gübreleme ve tarımsal problemler hakkında çiftçilerin sorularını yanıtlayan akıllı sohbet ekranı.
*   **Bitki & Hastalık Ansiklopedisi:** Bölgedeki yaygın bitkiler, ekim ipuçları ve hastalık önleme yöntemlerini listeleyen zengin bir kütüphane.
*   **Misafir Girişi ve Hızlı Yetkilendirme:** Kullanıcıların üye olmadan da uygulamayı anında deneyimlemesini sağlayan pratik giriş mekanizması.

---

## 🛠️ Kurulum ve Çalıştırma

1.  **Flutter SDK Yükleyin:** Bilgisayarınızda Flutter'ın kurulu olduğundan emin olun (`flutter doctor`).
2.  **Bağımlılıkları Çekin:**
    ```bash
    flutter pub get
    ```
3.  **Uygulamayı Çalıştırın (Android/iOS Simülatör veya Cihazda):**
    ```bash
    flutter run
    ```
4.  **Backend Bağlantı Ayarı:**
    Mobil uygulamanın API isteklerini yerel Django sunucunuza yönlendirmek için `lib/config/` altındaki API URL tanımlamalarını yerel IP adresinizle (veya emülatörler için `10.0.2.2:8000`) güncellediğinizden emin olun.
