# Yiğit Simülasyonu – GitHub / Render

Bu paket, mevcut simülasyonun ayrı bir çalışma kopyasıdır. Orijinal dosyalar değiştirilmemiştir.

## Dosyalar
- `index.html`: Simülasyon.
- `bugatti.modelbin`, `range.modelbin`, `porsche.modelbin`, `bmw.modelbin`, `lambo.modelbin`: Simülasyonda önceden gömülü olan aynı GLB araç modellerinin gzip sıkıştırılmış verileri.

Dosya adlarında `.modelbin` kullanılması bilinçlidir: dosyalar normal ikili veri olarak sunulur ve tarayıcı içinde gzip açılır.

## GitHub'a yükleme (ZIP'i tek dosya olarak yüklemeyin)
1. Bu ZIP dosyasını telefonda çıkartın.
2. GitHub'da yeni ve boş bir repository oluşturun.
3. Repository içinde **Add file → Upload files** seçin.
4. `index.html` ile beş `.modelbin` dosyasını birlikte seçip yükleyin. Hepsi repository'nin ana dizininde (root) olmalı.
5. Commit changes ile kaydedin.

## Render
1. Render Dashboard → New → Static Site.
2. GitHub repository'nizi bağlayın.
3. Build Command boş bırakın.
4. Publish Directory alanına `.` yazın.
5. Deploy edin.

## Önemli
- Modeller ayrı dosyalardan yüklenir; seçilen aracın gerçek GLB modeli doğrudan açılır, basit bir geçici araç gösterilmez.
- Araç modellerinin GLB içeriği değiştirilmedi; yalnızca depolama/indirme biçimi değiştirildi.
- Bu paket hesap sistemi veya yeni çevrimiçi sunucu eklemez.
- Modelleri indirmek için internet bağlantısı gerekir. Three.js ve GLTFLoader da mevcut sürümde olduğu gibi CDN'den yüklenir.
- Yayına almadan önce Render adresinde BMW, Porsche, Lamborghini, Bugatti ve Range Rover'ı tek tek deneyin. Orijinal simülasyon ZIP'ini yedek olarak saklayın.
