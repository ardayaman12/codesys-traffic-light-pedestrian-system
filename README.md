# codesys-traffic-light-pedestrian-system
CODESYS V3 Ladder Logic ile Yaya Butonlu Trafik Lambası ve Interrupt Mantığı Otomasyonu
CODESYS V3 - Yaya Butonlu ve Interrupt Mantıklı Trafik Lambası Otomasyonu

Bu proje, CODESYS V3 ortamında Ladder Logic (LD) dili kullanılarak geliştirilmiş, sanal HMI (Visualization) ile simüle edilmiş bir trafik ve yaya lambası otomasyon sistemidir.

 🎯 Projenin Öne Çıkan Özellikleri
- Akıllı Yaya Önceliği (Interrupt / Override):Yaya butonuna basıldığında, sistem 3 saniye içerisinde ana zamanlayıcıyı (`TON`) sıfırlayarak trafiği derhal kırmızıya keser ve yaya geçişini sağlar.
- Güvenli Mühürleme & Otomatik Sıfırlama: Yaya isteği sanal bir röle (`yaya_istek`) ile hafızaya alınır, kilitlenme tamamlandığında PLC'nin *Scan Cycle* avantajı kullanılarak milisaniyeler içinde mühür otomatik bozulur.
- Çift Bobin (Double Coiling) Koruması: PLC mantığına aykırı olan çift bobin kullanımını engellemek amacıyla şartlar sanal rölelerle (flag) ayrıştırılmış ve tek çıkış üzerinden sürülmüştür.
- HMI Visualisation: Sistem, kullanıcı arayüzü üzerinden anlık olarak izlenebilir ve butonlar vasıtasıyla kontrol edilebilir.

---

 🛠 Kullanılan Teknolojiler
- Yazılım: CODESYS V3.5
- Programlama Dili:Ladder Diagram (LD) / PLCopen XML
- Bileşenler:TON (Timer On-Delay), RS Flip-Flop / Mühürleme Mantığı, Normalde Kapalı Kontak (NC) Interrupts, HMI Visualization



👨‍💻 Yazar
Hasan Arda Yaman
Elektrik-Elektronik Mühendisliği Öğrencisi
