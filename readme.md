# Robot AI Project

## Proje Hakkında
Robot AI Project, FreeRTOS tabanlı, ESP32 ve Raspberry Pi Pico kullanan otonom bir robot sistemidir.
Bu proje, sensörler ve yapay zeka modelleri ile çevresini algılayıp, karar verebilen bir robot geliştirmeyi amaçlamaktadır.

## Kullanılan Teknolojiler
- **ESP32-CAM**: Ana kontrol birimi
- **Raspberry Pi Pico**: Sensör okuma ve motor sürme işlemleri
- **FreeRTOS**: Gerçek zamanlı işletim sistemi
- **UART & MQTT**: Haberleşme protokolleri
- **Jekyll & GitHub Pages**: Proje dökümantasyonu ve web arayüzü

## Proje Dizini
```
robot_ai_project/
│── core/                         # Temel AI yöneticileri
│── ai_models/                     # AI Modelleri
│── personality/                   # Kişilik Motoru
│── sensors/                       # Sensör Girişleri
│── output/                        # Çıktılar (Ses, hareket vs.)
│── communication/                 # Donanım Haberleşmesi
│── utils/                         # Yardımcı fonksiyonlar
│── config/                        # Yapılandırma Dosyaları
│── logs/                          # Log & Kayıt Sistemi
│── docs/                          # GitHub Pages içeriği
│── main.py                        # Ana çalıştırılabilir dosya
│── README.md                      # Proje açıklaması
```

## GitHub Pages & Cayman Teması
Bu proje, dökümantasyon için GitHub Pages ve Cayman temasını kullanmaktadır.
Dökümantasyonu yerel olarak çalıştırmak için:

```bash
bundle exec jekyll serve
```

Ardından tarayıcınızda `http://localhost:4000` adresini ziyaret edebilirsiniz.

## Katkıda Bulunma
Projeye katkıda bulunmak isterseniz:
1. Depoyu forklayın.
2. Yeni bir dal (branch) oluşturun: `git checkout -b yeni-ozellik`
3. Değişiklikleri yapıp commit edin: `git commit -m 'Yeni özellik eklendi'`
4. Deponuza push edin: `git push origin yeni-ozellik`
5. Bir Pull Request açın.

## Lisans
Bu proje MIT Lisansı altında lisanslanmıştır.

