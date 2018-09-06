# Linux_Notes
#### Dosya Listeleme
* ls: Bulunduğun dizinin içeriğini göster
* ls -a: Gizli dosyaları da göster
* ls -l: Uzun listele (sahip, izinler, boyut ve tarih dahil)
#### Bulunduğun Dizini Gösterme:
* pwd : Çalışılan dizinin ismini verir
#### Başka Dizine Geçme:
* cd yol: yol dizinine geçer
* cd ~: Sizin home dizininize geçer
* cd -: Bir önceki dizine döner
* cd ..: Bir üst dizine geçer
#### Yeni Dizin Dosya Yaratma, Taşıma, Kopayalama ve Silme:
* mkdir dizin: Yeni dizin yaratır
* touch dosya: Dosya varsa tarihini değiştirir, yoksa yaratır
* rmdir dizin: Boş dizini kaldırır
* rmdir -r dizin: dizini ve altdizinleri kaldırır
* rm dosya: Dosyayı kaldırır
* mv kaynak hedef: Dosyaları taşımak veya adlarını değiştirmek için
* cp kaynak hedef: Dosya kopyalama

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
