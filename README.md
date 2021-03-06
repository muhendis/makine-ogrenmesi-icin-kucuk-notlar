# Makine ogrenmesi icin küçük notlar
Bu depo makine öğrenmesi ve veri bilimine başlamış kişilere kısa notlar şeklinde bilgiler sunmak için oluşturuldu. Eğer sizinde eklemek istedikleriniz varsa bir pull request kadar uzaktasınız.
###### ***Lisans :GNU General Public License v3.0***

Notlar
  - [Not 1 : Güven aralığı nasıl yorumlanır?](https://github.com/muhendis/makine-ogrenmesi-icin-kucuk-notlar#not-1--g%C3%BCven-aral%C4%B1%C4%9F%C4%B1-nas%C4%B1l-yorumlan%C4%B1r)
  - [Not 2 : Merkezi Limit Teoremi ?](https://github.com/muhendis/makine-ogrenmesi-icin-kucuk-notlar#not-2--merkezi-limit-teoremi-)
  
## Not 0 : Veri bilimi için nasıl bir yol izlenmeli ?  

  0. Betimsel istatik  ve genel resim görselleştirmesi
  1. Eksik veri incelenmesi
  2. Aykırı değerlei inceleme
  3. Tekrardan görselleştirme
  4. Nitelik seçimi ve azaltımı
  5. Tekrardan görselleştirme
  6. Model kurulumu
  7. Tekrardan görselleştirme


## Not 1 : Güven aralığı nasıl yorumlanır?
Güven aralığının değeri %95 olmasının özel bir sebebi yoktur. %0 ile %100 arasında istenilen değer olabilir ancak %5 hatalı olma durumu bir şekilde öteden beri yeterli görüldüğü için tıbbı araştırmalarda %95 güven aralığı kullanılır.
%95 güven aralığı bize en kitabi haliyle, şunu söylemektedir; çalışmayı aynı popülasyondan farklı örneklemler seçerek birçok kere tekrarlasak örneğin 1000 kere, bunların %95’inde yani 950’sinde hesaplayacağımız güven aralığı popülasyondaki gerçek sonucu içerecektir.

Bu şekildeki bir ifade yorum yapmak biraz zor olduğu için, belki biraz kitabi bilgiyi zorlayarak, günlük pratikte % 95 güven aralığını söyle yorumlayabiliriz;

Örneğin yukarıdaki çalışmanın sonunda 6 aylık tedavi sonrasın A ve B ilaçları arasında sistolik kan basıncını azaltma açısından ortalama 6 mmHg’lik bir fark bulduğumuzu ve bu 6 mmHg’lik ortalama için %95 güven aralığının alt sınırı 3 mmHg, üst sınırını 9 mmHg hesapladığımızı varsayalım.

Bu sonuçları yapmak istediğimiz çıkarıma göre günlük pratiğimizde 2 şekilde ifade edebiliriz (3);

   - Aynı çalışmayı aynı popülasyondan seçiliş 100 farklı örneklem ile tekrarlasam 95’inde A ve B ilaçları arasındaki ortalama farkı 3 ile 9 mmHg arasında bulabilirim veya

   - %95 eminlikte söyleyebilirim ki tüm popülasyonda A ve B ilaçları arasındaki ortalama fark 3 ile 9 mmHg arasında bir değer olacaktır.
   
   ***Ek : Güven aralığının alt ve üst sınırı birbirine ne kadar yakın ise yani güven aralığı ne kadar darsa tüm popülasyonu tahmin etmede o kadar başarılıyız denilebilir yani
yukarıdaki çalışmada %95 güven aralığının sınırlarını 5 ve 7 olarak hesaplamış olsaydık, 3 ve 9 olarak hesaplanan durumdan daha iyi bir tahmin yapmış olurduk***
[Kaynak](https://medium.com/@mehmetberktasmdmsc/guvenaraligi-d3dcca18779d)

## Not 2 : Merkezi Limit Teoremi ?

İstatistiksel problem kontrol sürecinde süreç davranışını analiz edebilmemiz için öncelikle sürecin nasıl bir dağılım gösterdiğinin anlaşılması gerekir ve genelde bir çok problem normal dağılım özellikleri baz alınarak çözümlenir.

Ancak, değişkenliklerin her zaman kontrol edilememesi ya da çıktıların her zaman çan eğrisine benzemediği durumlarda, süreçlerin modellenebilmesi kolay değildir.

İşte bu aşamama Merkezi Limit teoremi bize yardımcı olmaktadır.

İstatistik biliminde Merkezi Limit teoreminin çok anlamlı bir yeri vardır. Merkezi limit teoremine göre, süreç üzerinden alınan örnek sayısı artıkça ve dışarıdan bir etki olmadığı müddetçe, farklı dağılım özelliği taşıyan süreç çıktıları histogram üzerinde ortalama değer etrafında normal dağılıma yakınsar bir dağılım gösterirler.

Merkezi limit teoremi doğrultusunda, alınan örnek sayısının 30 ve üzeri olması durumlarında süreç dağılımı normal dağılıma yakınsama göstermedir. [Kaynak](https://www.leanofis.com/6-sigma/merkezi-limit-teoremi-ve-normal-dagilim.html)

## Not 3 : Standart sapma, varyans, kovaryans ve korelasyon ?

## Not 4 : ROC ?

## Not 5 : Hata Matrisi(Confusion Matrix) nasıl yorumlanır?
[kaynak](http://www.datascience.istanbul/2017/07/02/hata-matrisini-confusion-matrix-yorumlama/)

## Not 6 : İstatistiksel dağılımlar ?

## Not 7 : İstatistiksel testler ?

## Not 8 : Bias-Variance arasındaki tradeoff , Underfitting ve Overfitting?

## Not 9 : Bias-Variance dan etkileri sonucu train ve test hata sonuçları ? 

## Not 10 : RMSE,MSE,MAE ?

## Not 11 : Tamam modelleri rmse,mse gibi değerler ile karşılaştıra bilirim , peki müşteriye  şu rmse ile hatalı sonuç alabilirsiniz demek ne kadar doğru? (✮)

Çok güzel noktaya değinmişsiniz . Bu durumda  test verisinden her bir elamanı için oluşan hataların dağılımın çizdirip şu değerler için şu hatayı aldım örneğin test verisinin %85 inde 0.2 gibi bir hata verirken %5 ise 0.8 gibi hata alındı biz bu %5 lik veriyi inceleyeceğiz yapısal bir sorun mu yoksa başka bir neden oldu onu üzerine gideceğiz gibi bir yorum yapılabilir.

## Not 11 : Holdout ve K-fold Cross Validation ?

## Not 12 : Basit doğrusal regresyonda Gradient Descent Vs Closed Form ?

Çoğunlukla tercih edilen yöntem Gradient Descent’tir fakat adım boyu, eşik değeri gibi durumları belirlemek zordur. Closed form da bu tarz belirlemeler olmadığı için daha kolaydır ama değişkenler arttıkça Gradient Descent’ti kullanmak daha verimli olur.[Kaynak](http://devveri.com/yapay-ogrenme/basit-lineer-regresyon)

## Not 13 : Doğrusal regresyonda e(hata) ?

Formül olarak e=y-ý ile bulunur. Amaç gerçek veri ile tahmin arasındaki farkı tolere etmekdir.

## Not 14 : Korelasyonun regresyondaki önemi ? (✮)

Örneğin tahmin edilecek olan y değişkeni ile x1 arasında 0.75 olan korelasyon x2 ile de 0.65 ise ve x1 ile x2 arasındaki korelasyon 0.05 gibi düşük ise x1 'in açıklayamadığı kısımı x2 değikenini açıklar ve modelde büyük etkiye sahip olurlar diğer değişkenlere göre(diğer değişkenlerin y ile düşük kolerasyon yaptığını göz önüne alırsak)

## Not 15 : Regresyonda hangi parametrelere dikkat edilmeli?
R-squared,adj-R-squared,p-value,coef ve bu coeff in güven aralığı 

## Not 16 : Lineer regresyon yapıldığında elde edilen değerleri nasıl formül haline  getirebiliriz ?
örneğin => satış = intercept_value + x1_value*Reklam

## Not 18 : Multiple Lineer regresyon ile temel 2 amaç nedir ? (✮)

1- Bağımlı değişkenler ile bağımsız değişkeni tahmin etme(ana amaç)

2- Bağımlı değişkeni tahmin etmye yarayan bağımsız değişkenlerin şiddeti ve yönüdür.(örneğin ev fiyatı tahmin ederken kaç yıllık olduğu negatif bir etki bırakırken oda sayısı ise pozitif yönde şiddetli bir etki verir )

## Not 19 : Regresyon problemlerinde her zaman ilk önce Multiple Lineer regresyon uygulanmalı neden mi  ? (✮)

MLR uygulanarak bağımlı değişken ile bağımsız değişkenler arasında yapılan test sonucu p-value değerlerine bak çünkü anlamı bir durum olması lazımdır.Ona göre bağımsız değikenler seçip başka algoritmalarda da kullanlır.

## Not 20 : Cross validation hatası veya R2 ?

Bize daha doğru net bilgi verir çünkü verinin tamamını görür.

-

## Not 21 : Aykırı değerleri neden veriden atmalıyız ?

Öncelikle şunu söyleyebiliriz ki aykırı değerler o kadar kötü bir durumu temsil etmez kimi zaman yeni trendi kimi zaman ise anormallikleri belirlemede yardımcı olur fakat atma sebebimiz bu değil biz bunu algoritmaya gösterdiğimiz zaman algoritma bunu genel bir davranış olarak anlar ve tahmin etmede bu değeri kullanır , 10.000 de 1 olacak bir olay sistemni etkiler yani yanlılık artışı tahmin yeteneğini öldürür.


## Not 22 : Aykırı değerler var ne yapmalıyım?

- Eğer bunlar % 1 ise bunları direkt olarak at
- Eğer biraz varsa onları ortalama ile yer değiştir(Genellikle)
- Eğer hatrı sayılır düzeyde ise baskılama yöntemi ile alt ve üst sınırlara çek çeyrekler arasındaki Q1 ve Q3 e göre
