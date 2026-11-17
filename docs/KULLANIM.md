# Kurulum ve kullanım

1. GitHub Releases üzerinden Universal ZIP’i indir ve aç.
2. `Termusta.app` dosyasını Uygulamalar klasörüne taşı.
3. Termusta’yı aç, **Sunucu ekle** düğmesine bas, bağlantı bilgilerini gir ve kaydet.
4. Sunucuyu seçip **Bağlan** düğmesine bas. Her oturum pencerenin üst çubuğunda ayrı bir sekme açar.
5. Sunucu listesine dönmek için **Sunucular** düğmesine tıkla. Sekmenin kapatma düğmesi ilgili SSH oturumunu sonlandırır.

## SSH parolası

Sunucu formunda **Kayıtlı parolayı değiştir** seçeneğini açıp parolayı gir. Parola `~/Library/Application Support/Termusta` altında, kullanıcı hesabına özel izinlerle şifresiz saklanır. Sonraki bağlantılarda Termusta, OpenSSH’nin parola istemine kayıtlı parolayı bir kez otomatik girer. Parola reddedilirse terminalde yeniden girebilirsin. Parolayı kaldırmak için formdaki parola alanını boş kaydet. Kimlik doğrulamayı ve sunucu anahtarı denetimini macOS OpenSSH yürütür.

## Güncellemeler

Termusta açıldığında ve açık kaldığı sürece saatte bir GitHub Releases’ı denetler. Elle denetlemek için **Termusta → Güncellemeleri Denetle…** menüsünü kullan. Yeni sürüm varsa Termusta paketi indirir, SHA-256 değerini doğrular, kurar ve yeni sürümle yeniden açılır. Yeniden başlatıldığında açık SSH oturumları sonlanır.

Paket yerel olarak imzalanır ve Apple noter onayı içermez.
