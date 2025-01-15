Özellikler
Öğretim Görevlisi Tanımlama

Yeni bir öğretim görevlisi adı, soyadı ve bölümü girilerek sisteme eklenebilir.
Veriler ogretmenler.json dosyasına kaydedilir.
Ders Tanımlama

Daha önce tanımlanmış bir öğretim görevlisi seçilerek ders adı ve kredi bilgileri ile yeni bir ders oluşturulur.
Veriler dersler.json dosyasına kaydedilir.
Öğrenci Tanımlama

Öğrencilerin adı, soyadı ve 11 haneli öğrenci numarası girilerek sisteme kayıt edilir.
Veriler ogrenciler.json dosyasına kaydedilir.
Öğrenciyi Derse Kaydetme

Sisteme kayıtlı öğrenciler ve dersler arasında ilişki kurulabilir.
Ders bilgileri içinde kayıtlı öğrenciler listelenir.
Ders Bilgilerini Görüntüleme

Her bir ders için öğretim görevlisi bilgileri, ders kredisi ve kayıtlı öğrenciler listelenir.
Veri Kaydetme ve Çıkış

Tanımlanan tüm öğretim görevlileri, dersler ve öğrenciler JSON formatında dosyaya kaydedilir. Program güvenli bir şekilde sonlandırılır.
Kullanılan Yapılar
Polimorfizm:
BilgiGoster() metodu, hem öğrenci hem de öğretim görevlisi sınıflarında farklı şekillerde özelleştirilmiştir.

Soyutlama:
Person sınıfı, hem Ogrenci hem de OgretimGorevlisi için temel bir yapı sağlar.

Arayüz:
IPerson arayüzü, BilgiGoster metodunun sınıflar tarafından uygulanmasını zorunlu kılar.

JSON Entegrasyonu:
Veriler System.Text.Json kütüphanesi ile JSON formatında dosyaya kaydedilir ve yüklenir.

JSON Dosya Yapısı
ogretmenler.json
Öğretim görevlilerinin ad, soyad ve bölüm bilgilerini saklar.

dersler.json
Ders adı, kredi bilgisi, öğretim görevlisi ve kayıtlı öğrencilerin listesini içerir.

ogrenciler.json
Öğrencilerin ad, soyad ve numaralarını barındırır.

Kullanım Talimatları
Uygulamayı çalıştırın. Konsolda bir menü görüntülenecektir.
Seçiminizi yapmak için 1 ile 6 arasında bir seçenek girin.
Gerekli bilgileri doldurduktan sonra işlemleri tamamlayın.
Çıkış yapmak için "6"yı seçin ve verilerin kaydedildiğinden emin olun.
Örnek Çalışma Akışı
Adım 1: Öğretim görevlisi tanımlayın.
Örnek: "Ahmet Yılmaz, Bilgisayar Mühendisliği".
Adım 2: Ders tanımlayın.
Örnek: "Veri Yapıları, 3 kredi, Ahmet Yılmaz".
Adım 3: Öğrenci tanımlayın.
Örnek: "Ali Demir, 12345678901".
Adım 4: Öğrenciyi derse kaydedin.
Örnek: "Ali Demir -> Veri Yapıları".
Adım 5: Ders bilgilerini görüntüleyerek kayıtları kontrol edin.
