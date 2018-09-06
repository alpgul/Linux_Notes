# Linux_Notes_Basic
#### Dosya Listeleme
* ls: Bulunduğun dizinin içeriğini göster
* ls -a: Gizli dosyaları da göster
* ls -l: Uzun listele (sahip, izinler, boyut ve tarih dahil)
* ls -lh: Uzun listele ve dosya boyutlarını gosterir
* ls -lt: Uzun listele ve oluşma tarihine göre sırala yeni>eski
* ls -r: Sıralamayı ters çevirir.
#### Bulunduğun Dizini Gösterme:
* pwd : Çalışılan dizinin ismini verir
#### Başka Dizine Geçme:
* cd yol: yol dizinine geçer
* cd ~: Sizin home dizininize geçer
* cd -: Bir önceki dizine döner
* cd ..: Bir üst dizine geçer
#### Yeni Dizin Dosya Yaratma, Taşıma, Kopayalama ve Silme:
* mkdir dizin: Yeni dizin yaratır
* mkdir -p asa/asa1/asa2: bununulan dizinde belirtilinen klasörleri olşturur
* mkdir -p aa1/{bb1/cc1/{dd1,dd2,dd3},bb2,bb3,bb4}:Verilen komutla en üst dizin aa1 olur. Bir alt dizinde bb1,bb2,bb3,bb4 yer almaktadır. bb1 dizininin altında ise cc1 dizini vardır. cc1 dizinin altında ise dd1,dd2,dd3 dizinleri oluşturulmuştur.	
* mkdir -m 754 aaa veya mkdir -m o=+r,g=+rx aaa :kullanma yetkileri düzenler u:user o:other g:group r:read w:wried x:erişim 754 her basamak binary şekilde u g o ifade eder
* touch dosya: Dosya varsa tarihini değiştirir, yoksa yaratır
* rmdir dizin: Boş dizini kaldırır
* rmdir -r dizin: dizini ve altdizinleri kaldırır
* rm dosya: Dosyayı kaldırır
* rm -f dosya: Dosya silmek isteyip istemediği sormaz.
* rm -v dosya: Dosya silme işlemi sonucunda silinen dosyaların özetini verir.
* mv kaynak hedef: Dosyaları taşımak veya adlarını değiştirmek için
* cp kaynak hedef: Dosya kopyalama
* cp -r kaynak hedef: Dizin kopyalama

#### Dosya Görüntüleme
* cat:dosyanın içini gösterir
* less : Dosyalari goruntulerken filtre koymak icin

#### Pipe(|)
* ifconfig | cat : Pipe öncesinde kullanıdığınız komutun veya işlemin sonucunu sonrasındaki komuta aktarır.
#### Redirect(>)
* ls -al > list.txt : Bu işaret öncesindeki komutun sonucunu yeni oluşturulacak bir dosyaya yazar.
#### Softlink
* ln -s kaynak hedef:Dosyanın veya klasörün şu anda bulunduğu dizinin yerine bağlantı yaparlar. kaynak silinse veya yeri değişirse çalışmazlar
#### Hardlink
* ln dosya hedef: Hard link'ler dosyanın şu anda bulunduğu fiziksel lokasyonuna bağlantı yaparlar.Kaynağa ne olursa olsun çalışmaya devam eder.
