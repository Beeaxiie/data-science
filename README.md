## Veri bilimi
****
- Veri bilimi, yapılandırılmış ve yapılandırılmamış verilerden bilgi ve öngörü elde etmek için bilimsel yöntemleri, süreçleri, algoritmaları ve sistemleri kullanan çok disiplinli bir alandır. (*Wikipedia*)
- Daha basitçe, veri bilimi geleceğe yönelik analizler yapmak için algoritmalar kullanan bir alandır.
- Veri biliminin asıl amacı, gerçek olayları verilerle anladıktan sonra analizler yapmaktır. Örnek vererek anlatmak istiyorum, 2020 yılındaki ev fiyatlarını anlayıp, 2023'deki ev fiyatlarını analiz eden bir model (yapay zeka) yapmak doğrudan veri bilimi ile alakalıdır.
- Bu yazımda size veri biliminin bir alt alanı olan, makine öğrenmesi alanını anlatacağım. Bu alanın dünyaya ne kattığını, aynı zamanda neleri sildiğini, avantajları ve dezavantajlarıyla ele alacağım.

## Makine öğrenmesi
****
- Makine öğrenimi veya makine öğrenmesi, bilgisayarların algılayıcı verisi ya da veritabanları gibi veri türlerine dayalı öğrenimini olanaklı kılan algoritmaların tasarım ve geliştirme süreçlerini konu edinen bir bilim dalıdır. (*Wikipedia*)
- Wikipedia tanımı size karışık gelmiş olabilir basitçe, insan ve bilgisayarın iletişimini kurmayı sağlayan, bunu yaparak insanın problemlerini çözen (çözmeye çalışan) alan diyebiliriz.

### Makine ile insan nasıl iletişim kuruyor?
- Bu alanı araştırdığımda direkt olarak merak ettiğim konu bu oldu, o yüzden ilk olarak teorik bilgilere geçmeden önce konuyu anlamamız için ön bilgiler vereceğim.
- Makine ile insan veriler sayesinde iletişim kurabiliyor. Nasıl yani diye soruyorsanız şöyle, elimizdeki veri kümesini makineye tanıtıyoruz (belli algoritmalar kullanarak bu işlemi gerçekleştiriyoruz) makineye bu verilerle birşeyler öğretmeye çalışıyoruz (örnek vermek gerekirse kedi köpek ayırımı gibi) makineyle bu sayede iletişim kurup, sorunlarımıza çözümler yapabiliyoruz.

### Veri nedir?
- Veri günlük hayattaki her türlü bilgiye denen kapsayıcı bir kavramdır. Bir sürü veri türü var fakat bu yazımda kafanızı bunlarla doldurmak istemiyorum :).
- Örnek verecek olursak, "Caddede 3 araba var." bu bir veridir hatta, "1. araba kırmızı, 2. araba beyaz, 3. araba siyah renginde." bu da bir veridir. "Caddenin genişliği 10 metre.", "Caddenin ortasında yaya geçidi var." bunların hepsi bir veri. Fakat işe yaramaz veriler. Tabii ki yapacağımız uygulamanın amacına göre bu işe yaramaz veriler belki altın madeni gibi değerli olabilir.

### Doğruluk
- Doğruluk, programa verdiğimiz inputun ne kadar doğru olduğunu gösteren sayısal ifade. (Mesela 10 adet kedi fotoğrafı verdik ve tahmin et dedik, 7sine kedi 3üne de vaşak dedi diyelim bu halde doğruluk oranımız: 70% oluyor.)

### Denetimli & denetimsiz öğrenme
- Denetimli öğrenme, veriyi etiketleyerek veriyoruz ve makineye öğretiyoruz.
- Denetimsiz öğrenme, veriyi etiketlemeyerek vererek kendi kendine sınıflandırmasını istiyoruz. Aslıdna isminde her ne kadar denetimsiz öğrenme yazsa bile en son işlemde bir insan tarafından denetimleniyor.

### Modelin eğitilmesi
- Makinelerin öğrenmesi ve gerçek hayata geçirildiğinde düzgün sonuçlar vermesi için yapılan öğretilmedir.
- Şöyle eğitiyoruz, elimizde bir miktar verimiz var ve bu verileri programa verdiğimizde programda bunları doğru bir şekilde tahmin etmeye çalışıyor, eğer yanlış tahmin ederse bazı değişiklikler yaparak doğruluğunu arttırmaya çalışıyoruz.

### Modelin test edilmesi
- Modeli eğittikten sonra gerçek bir kullanıcı gibi test etmeye başlıyoruz ve cevapların nasıl olduğunu bakıyoruz.
- Burada yanlış bir adım yaptık aslında modeli eğittikten hemen sonra test ettik. Bu modelimizi ezberlemeye iter ve, hiç görmediği verilerde doğruluğu çok düşer.

### Modelin ön test edilmesi
- Modeli eğittikten sonra modeli hiç görmediği verilerle ön test. Modelimizde istediğimiz doğruluk oranını elde ettikten sonra gerçek bir kullanıcı gibi test ediyoruz.

### Makine öğrenmesi alanında kullanılan programlama dilleri
- Makine bilimi alanı her gün çok hızlı bir şekilde gelişiyor. Bunun yanı sıra programlama dilerinde makine öğrenimi, derin öğrenme (makine öğrenmesinin alt dalı) kütüphaneleri hızlı bir şekilde genişliyor. Makine öğrenmesi için bir çok dil kullanılabilir fakat önerilenler, Python, Julia, R(daha çok veri analizi için kullanılır).
**Pythonun avantajları ve dezavantajları**
- Pythonun avantajları, çok geniş bir topluluğa sahip olması, geniş bir kütüphane desteği, genel programlama dili olması (yani tek bir amaca hizmet etmiyor, genel programlama için kullanılabilir), kolay öğrenilebilirlik, kolay okunabilirlik.
- Pythonun dezavantajları, -bana göre- en büyük dezavantajı yavaş çalışmasıdır, bazı durumlarda R'dan daha az istatiksel özelliğe sahiptir.
**Julialang avantajları ve dezavantajları**
- Julialangin avantajları, yeni ve hızla gelişen bir programalam dilidir, -en beğendiğim özelliği- R'ın istatiksel, pythonun kolaylığını, C'nin ise performanslı olan özelliklerini tek bir dilde birleştirir.
- Julialangin dezavantajları, topluluğu pythona göre azdır, bazı önemli kütüphaneler julialang'de bulunmayabilir.
**R'ın avantajları ve dezavantajları**
*Ön bilgi: R en fazla veri analizi için kullanılır. Makine öğrenimi için de kullanılabilir.*
- R'ın avantajları, istatiksel özellikleri gelişmiştir, veri analizi için idealdir, topluluğu geniştir, kütüphane desteği iyidir.
- R'ın dezavantajları, okunması ve öğrenilmesi zor olabilir, genellikle sadece veri bilimi alanı için kullanılır, bazı durumlarda performansı düşük olabilir.

### Makine öğrenimi için kullanılan kütüphaneler
- Elbette önerdiğim 3 dilde bir sürü kütüphane var fakat ben sadece python dili için göstereceğim.
1. *scikit-learn*: Makine öğrenimi için kullanılan güçlü bir kütüphane.
2. *PyTorch*: Facebook tarafından geliştirilen, güzel bir kütüphane.
3. *TensorFlow*: Google tarafından geliştirilen, makine ve derin öğrenme algoritmaları için kullanılan ve en popüler kütüphane.
4. *Keras*: TensorFlow'un üstüne inşa edilmiştir ve daha gelişmiş özelliklere sahiptir.
- Tabii ki bir sürü kütüphane var fakat ben size 4 tanesini göstermek istedim. Araştırarak diğerlerine de bakabilirsiniz.

 Bu yazımda size makine öğrenimi alanını az da olsa anlatmak istedim, umarım faydalı olmuştur sağlıcakla kalın!
