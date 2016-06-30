# Terminal Hile Sayfası Mac (Temel)
Original translation by [zeluizr](https://github.com/zeluizr)

------------

## KISAYOL

| Anahtar | Komut |
| ------ | ----------|
| Ctrl + A | Şu anda üzerinde yazdığını satırın başına git |
| Ctrl + E | Şu anda üzerinde yazdığını satırın sonuna git |
| Ctrl + L | Ekranı temizle |
| Command + K | Ekranı temizler |
| Ctrl + U | İmleç konumunda önce çizgiyi temizleyin. Satırın sonundaki ise, tüm çizgi temizler. |
| Ctrl + H | Gerituşu aynı |
| Ctrl + R | Bu daha önce kullanılan komutları ile arama yapmanızı sağlar |
| Ctrl + C | Her ne çalıştırıyorsanız ise sonlandırır.|
| Ctrl + D | Bir süreç çalışırken EOF gönderir veya süreç çalışmadığı zaman da anlık shell'den çıkar. |
| Ctrl + Z | Eğer bir bekleyen varsa ya da arka planda çalışan ne olursa olsun geçirir. fg yükler. |
| Ctrl + W | İmleçten önceki kelimeyi temizle.  |
| Ctrl + K | İmleçten sonraki çizgiyi temizleyin. |
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

| Kısayol | Açıklama |
| ------ | ----------|
| history n | Yazılan şeyler gösterir - son n öğeleri sınırlamak için bir numara ekler. |
| ctrl-r | Etkileşimli önceden yazdığınız komutları ile arama. |
| ![value] | 'Value' ile başlayarak yazdığınız son komutu çalıştırır. |
| !! | Yazdığınız son komutu çalıştırmak. |


## DOSYA YÖNETİMİ

| Kısayol | Açıklama |
| ------ | ----------|
| touch [dosya] | Yeni dosya yaratır. |
| pwd | Bulunulan dizinin tam yolu.  |
| ls -l | Üst dizini uzun listeler. |
| cd ../../ | Move dois niveis acima |
| cat | Concatenar as telas |
| rm [dosya] | Apaga dosyas, ex.: rm [dosya] [dosya] |
| rm -i [dosya] | Deletar com comfirmação |
| rm -r [dizin] | Apaga um diretório e seu conteúdo |
| rm -f [dosya] | Força o apagar sem confirmação |
| cp [dosya] [novo dosya copiado] | Copiar dosya |
| cp [dosya] [dizin] | Copiar um dosya para outro diretorio |
| mv [dosya] [novo nome] | Move/Renomeia, ex.: mv -v [dosya] [diretorio] |


## MANIPULANDO DIRETÓRIOS

| Kısayol | Açıklama |
| ------ | ----------|
| mkdir [diretorio] | Cria uma nova pasta |
| mkdir -p [diretorio]/[diretorio] | Cria uma pasta com uma sub-pasta |
| rmdir [diretorio] | Remove pasta ( esse komut só funciona se a pasta estiver vazia ) |
| rm -R [diretorio] | Remove a pasta com todos os dosyas dentro |


## PIPES - permite combinar vários komuts que geram saída

| Kısayol | Açıklama |
| ------ | ----------|
| > [dosya] | Gera um novo dosyas, lembrando que ela pode ser sobrescrita |
| >> [dosya] | Adiciona a saida ao dosyas |


## YARDIM

| Kısayol | Açıklama |
| ------ | ----------|
| [komut] -h | Exibe ajuda do komut |
| [komut] --help | Exibe ajuda do komut |
| [komut] help | Exibe ajuda do komut |
| reset | Reseta sua tela atual no terminal |
| man [komut] | Exibe ajuda para o seu 'komut' |
| whatis [komut] | Dá uma descrição de uma linha de 'komut' |

## komutS PARA GIT

| Kısayol | Açıklama |
| ------ | ----------|
| [komut] git init | Inicia um projeto git na pasta atual. |
