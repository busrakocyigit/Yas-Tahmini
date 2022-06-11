# Yas-Tahmini
Bu çalışma İstanbul Medeniyet Üniversitesi, Mühendislik ve Doğa Bilimleri Fakültesi, Matematik Bölümü, Mezuniyet Projesi için yapılmış bir çalışmadır.
Bu çalışmada denetimli yaş aralığı tahmini yapılarak bireylerin yaşlarını tahmin etmek hedeflenmiştir. Hali hazırda var olan, önceden eğitilmiş modeller yorumlanarak ve geliştirilerek model test edildikten sonra bir grup bireyin fotoğraflarından oluşan veri setinden yardım alınarak yaş tahmini yapılmıştır.
Bu veri seti https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/ çalışmasında da kullanılan WIKI veri setidir.
Ayrıca henüz tazeliğini koruyan DeepFace hazır paketinin 'yüz öznitelik analizi' kullanılarak yaş tahmini yapılmıştır.


Bir kişinin kimliği, yaşı, cinsiyeti, duyguları ve etnik kökeni, yüzlerindeki özellikler tarafından belirlenir. Güvenlik ve video gözetimi, elektronik müşteri ilişkileri yönetimi, biyometri, elektronik satış makineleri, insan-bilgisayar arayüzü, eğlence, kozmetoloji ve adli tıp, yaş ve cinsiyet sınıflandırmasının kullanışlı olabileceği gerçek dünya uygulamalarından sadece birkaçıdır.

Görüntülerden yaş tahmini ile ilgili mevcut araştırmalar, tahminlerin nasıl yapıldığına bağlı olarak iki yöntemle yapılabildiğini göstermektedir. Problem yaşların yaş kutularına dönüştürüldüğü çok sınıflı bir sınıflandırma problemi olarak ya da kesin yaşın tahmin edildiği bir regresyon problemi olarak ele alınabildiğini göstermektedir. Bu çalışmada regresyon problemi yöntemi ile çalışılmıştır. İncelemeler sonucunda daha önceden bu konuda yapılan çalışmalarda CNN modelindeve VGG-16 modelinin ince detaylandırmaları ile sonuca ulaşıldığı gözlemlenmiştir. Bu çalışma modeli CNN modeli ile sonuçlandırmıştır. Bu çalışmada kaynak olarak https://github.com/ShreyanshJoshi/Facial-Demographics-using-CNN/blob/master/Report\%20-\%20Detailed\%20Analysis\%20of\%20work.pdf çalışması kullanılmıştır.

Fotoğraftan yaş tahmini yapılırken ikinci bir yöntem olarak yeni bir kütüphane olan DeepFace kütüphanesi özellikleri kullanıldı. 7 yıllık bir kütüphane olan DeepFace yeni bir kütüphane olmasına rağmen gayet olumlu sonuçlar verebilmekte. DeepFace kütüphanesine ait olan yüz öznitelik analizinin analyze() fonksiyonu ile yaş tahmini yapıldı. (analyze() fonksiyonu ile yaş, cinsiyet, duygu ve etnik köken tahmini yapılmaktadır. Fakat biz yaş tahminini göz önünde tutup diğer girdileri ihmal ettik.)  Cihazda bulunan herhangi bir fotoğraf sisteme tanıtıldı ve çalıştırıldı.

# Kullanılan-Kütüphaneler
pip install numpy

pip install pandas

pip install keras\\
pip install deepface

