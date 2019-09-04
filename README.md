# makine-ogrenmesi-icin-kucuk-notlar
Makine öğrenmeside kullanılan teknik bilgiler için küçük ama değerli notlar

Notlar
  - [Note 1 : Güven aralığı nasıl yorumlanır?](https://github.com/muhendis/makine-ogrenmesi-icin-kucuk-notlar#note-1--g%C3%BCven-aral%C4%B1%C4%9F%C4%B1-nas%C4%B1l-yorumlan%C4%B1r)
  - [Note 2 : Merkezi Limit Teoremi ?](https://github.com/muhendis/makine-ogrenmesi-icin-kucuk-notlar#note-2--merkezi-limit-teoremi-)
  
  

## Note 1 : Güven aralığı nasıl yorumlanır?
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

## Note 2 : Merkezi Limit Teoremi ?

İstatistiksel problem kontrol sürecinde süreç davranışını analiz edebilmemiz için öncelikle sürecin nasıl bir dağılım gösterdiğinin anlaşılması gerekir ve genelde bir çok problem normal dağılım özellikleri baz alınarak çözümlenir.

Ancak, değişkenliklerin her zaman kontrol edilememesi ya da çıktıların her zaman çan eğrisine benzemediği durumlarda, süreçlerin modellenebilmesi kolay değildir.

İşte bu aşamama Merkezi Limit teoremi bize yardımcı olmaktadır.

İstatistik biliminde Merkezi Limit teoreminin çok anlamlı bir yeri vardır. Merkezi limit teoremine göre, süreç üzerinden alınan örnek sayısı artıkça ve dışarıdan bir etki olmadığı müddetçe, farklı dağılım özelliği taşıyan süreç çıktıları histogram üzerinde ortalama değer etrafında normal dağılıma yakınsar bir dağılım gösterirler.

Merkezi limit teoremi doğrultusunda, alınan örnek sayısının 30 ve üzeri olması durumlarında süreç dağılımı normal dağılıma yakınsama göstermedir. [Kaynak](https://www.leanofis.com/6-sigma/merkezi-limit-teoremi-ve-normal-dagilim.html)

