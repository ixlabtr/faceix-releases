# YüzKoru Lisans Denetim Raporu ve Üçüncü Taraf Lisansları (LICENSES.md)

Bu belge, **YüzKoru** uygulamasında kullanılan tüm bağımlılıkların, modellerin ve kütüphanelerin lisans türlerini ve uyumluluk durumlarını belgeler.

YüzKoru, **kamu kurumları, okullar ve ticari kullanım için tamamen güvenli, kısıtlayıcı olmayan (permissive) ve açık kaynak lisanslı** bileşenlerle geliştirilmiştir.

---

## 1. Dahil Edilen Modeller ve Lisansları

| Bileşen | Dosya Adı | Kaynak / Sağlayıcı | Lisans Türü | Ticari Kullanım İzni |
|---|---|---|---|---|
| **YuNet Yüz Tespit Modeli** | `face_detection_yunet_2023mar.onnx` | OpenCV Model Zoo (Shiqi Yu / OpenCV) | **MIT Lisansı** | **Evet** |
| **SFace Yüz Tanıma/Eşleme Modeli** | `face_recognition_sface_2021dec.onnx` | OpenCV Model Zoo (Zhong et al. / OpenCV) | **Apache-2.0 Lisansı** | **Evet** |
| **Haar Profil Yüz Kaskadı** | `haarcascade_profileface.xml` | OpenCV Projesi | **BSD 3-Clause Lisansı** | **Evet** |
| **PP-HumanSeg Portre Segmentasyon** | `human_segmentation_pphumanseg_2023mar.onnx` | OpenCV Model Zoo (PaddlePaddle / OpenCV) | **Apache-2.0 Lisansı** | **Evet** |

> **Önemli Not:**
> - Ticari kullanımı yasaklayan kütüphaneler/ağırlıklar (ör. ticari olmayan lisanslı InsightFace modelleri) **kullanılmamıştır**.
> - Katı copyleft veya ticari dağıtımı engelleyen yapay zeka modelleri (ör. Ultralytics YOLO AGPL-3.0) **kullanılmamıştır**.

---

## 2. Yazılım Bağımlılıkları ve Kütüphaneler

| Kütüphane | Sürüm | Amacı | Lisans |
|---|---|---|---|
| **PySide6 / shiboken6** | 6.7.2 | Masaüstü Kullanıcı Arayüzü (Qt6) | **LGPL-3.0** (Dinamik bağlantı ile ticari/kapalı koda uygundur) |
| **opencv-python-headless** | 4.10.0.84 | Bilgisayarlı görü, DNN çıkarım, karo/NMS | **Apache-2.0** |
| **numpy** | >=1.26.0,<2.0.0 | Hızlı matris ve piksel dizi hesaplamaları | **BSD 3-Clause** |
| **Pillow** | >=10.4.0 | Görüntü I/O, renk profilleri ve metadata temizliği | **HPND / MIT-eşdeğeri** |
| **pillow-heif** | >=0.18.0 | Apple HEIC format desteği (libheif) | **LGPL-3.0** |
| **platformdirs** | >=4.2.2 | Platforma özgü güvenli ayar/veri dizinleri | **MIT** |
| **reportlab** | >=4.2.2 | Hesap verebilirlik PDF raporu üretimi | **BSD 3-Clause** |
| **pytest / pytest-qt** | >=8.3.2 | Birim, çevrimdışı ve GUI testleri | **MIT** |
| **ruff** | >=0.5.5 | Kod kalitesi ve statik analiz | **MIT** |

---

## 3. Lisans Metinleri Özeti

### MIT License (YuNet, platformdirs, pytest, pytest-qt, ruff)
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

### Apache License 2.0 (OpenCV, SFace)
Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0

### BSD 3-Clause License (NumPy, Haar Cascade, ReportLab)
Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

### GNU Lesser General Public License v3.0 (PySide6, pillow-heif)
YüzKoru, PySide6 kütüphanesini dinamik olarak içe aktarır (bağlar). Uygulama LGPL v3.0 şartlarına uygun olup, PySide6 kütüphanesinin kaynak kodunu değiştirmeden bağımsız bir modül olarak kullanır.

