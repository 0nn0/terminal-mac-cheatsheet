# Terminal Hile Sayfası Mac (Temel)
Original translation by [durul](https://github.com/durul)

------------

## KISAYOL

| Anahtar | Komut |
| ------ | ----------|
| Ctrl + A | Şu anda üzerinde yazdığını satırın başına git |
| Ctrl + E | Şu anda üzerinde yazdığını satırın sonuna git |
| Ctrl + L | Ekranı temizler |
| Command + K | Ekranı temizler |
| Ctrl + U | İmleç konumunda önce çizgiyi temizleyin. Satırın sonundaki ise, tüm çizgi temizler. |
| Ctrl + H | Gerituşu ile aynı |
| Ctrl + C | Her ne çalıştırıyorsanız ise sonlandırır.|
| Ctrl + D | Bir süreç çalışırken EOF gönderir veya süreç çalışmadığı zaman da anlık shell'den çıkar. |
| Ctrl + Z | Eğer bir bekleyen varsa ya da arka planda çalışan ne olursa olsun geçirir. fg yükler. |
| Ctrl + W | İmleçten önceki kelimeyi temizle.  |
| Ctrl + K | Şu anda üzerinde olduğun satırın imleçten sonrasını temizleyin. |
| Ctrl + T | İmleçten önce son iki karakteri değiştirir. |
| Ctrl + F | İmleçi bir karakter ileri taşır. |
| Ctrl + B | İmleçi bir karakter geriye taşır. |
| Esc + F | İmleçi bir kelime ileri taşır. |
| Esc + B | İmleçi bir kelime geriye taşır. |
| Esc + T | İmleçten önceki son iki kelimeyi değiştirir. |
| Tab | Dosya ve klasör adları otomatik tamamlama |


## ANAHTAR KOMUTLAR

| Anahtar | Komut |
| ------ | ----------|
| cd | Ev dizini |
| cd [dosya] | Dizini değiştir. |
| cd - | Önceki dizin. |
| cd / | Kök dizin. |
| ls | Kısa liste. |
| ls -l | Uzun liste. |
| ls -a | Gizli dosyaları listele. |
| ls -lh | İnsanların okuyabileceği dosya boyutları ile uzun listeleme. |
| ls -R | Ardışık klasörün tüm içeriği |
| sudo [Komut] | (DO Süper Kullanıcı) Süper kullanıcının güvenlik ayrıcalıkları ile komutunu çalıştırın. |
| open [dosya] | (Çift tıklamışsınız gibi) Bir dosya açar |
| top | etkin işlemleri gösterir. Çıkmak için Q basın. |
| nano [dosya] | Nano düzenleyicisi kullanarak dosyayı açar |
| vim	[dosya] | Vim düzenleyicisi kullanarak dosyayı açar |
| exit | Çıkış |
| clear | Temizle |


## KOMUT GEÇMİŞİ

| Anahtar | Komut |
| ------ | ----------|
| history n | Kullandığınız son "n" tane komutu gösterir. |
| ctrl-r | Önceden yazdığınız komutlar arasında arama yapma. |
| ![value] | 'Value' ile başlayarak yazdığınız son komutu çalıştırır. |
| !! | Yazdığınız son komutu çalıştırmak. |


## DOSYA YÖNETİMİ

| Anahtar | Komut |
| ------ | ----------|
| touch [dosya] | Yeni dosya yaratır. |
| pwd | Bulunulan dizinin tam yolu.  |
| ls -l | Üst dizini uzun listeler. |
| cd ../../ | İki üst dizine gider |
| cat | Dosyanın çıktısını ekranda gösterir |
| rm [dosya] | Bir dosyayı sil, ex.: rm [dosya] [dosya] |
| rm -i [dosya] | Onay ile dosya sil. |
| rm -r [dizin] | Dizin ve içeriğini sil. |
| rm -f [dosya] | Onay olmadan dosya sil |
| cp [dosya] [yeni dosya] | "dosya"nın içeriğini "yeni dosya'ya kopyalayın|
| cp [dosya] [dir] | Dizinine dosyayı kopyalayın |
| mv [dosya] [yeni dosya] | Taşı / yeniden adlandır |


## DİZİN YÖNETİMİ

| Anahtar | Komut |
| ------ | ----------|
| mkdir [dir] | Yeni bir dizin oluşturun |
| mkdir -p [dir]/[dir] | İç içe dizinleri oluşturun |
| rmdir [dir] | Dizini kaldır |
| rm -R [dir] | Dizin ve içeriğini kaldır |
| [command] | [command] |	Çıktı üreten birden çok komutu birleştirmeyi sağlar. |
| less | Az |
| [command] > [file] | Dosyaya çıktı alır, üzerine yazılır alacak akılda tutmaz |
| [command] >> [file] |	Mevcut dosyaya çıktıları ekler. |
| [command] < [file] | Bir dosyanın içeriğini okumak için komutu girin. |


## YARDIM

| Anahtar | Komut |
| ------ | ----------|
| [command] -h | Yardım |
| [command] --help | Yardım |
| info [command] | Yardım |
| reset | Sıfırla |
| man [command] | Yardım menüsünü göser. |
| whatis [command] | Komutu tek bir satırla açıklar. |
