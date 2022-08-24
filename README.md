<h1 align = 'Center'>Nane&Limon 🐍 Teknofest 2022 TDDİ Repository</h1>

<div>Bu depo Teknofest 2022 Kapsamında Türkçe Doğal Dil İşleme Yarışması katılımcısı Nane&Limon ekibinin dökümanlarını içermektedir.</div>


* **Nane&Limon-Tanıtım.pdf** dökümanı yarışmaya katılmak için oluşturulan ilk dökümandır.

* **Nane&Limon-Sunumu.pdf** dökümanı yarışma sonunda yapılacak olan sunum pdf idir.
  > Not: Cihaz farkı nedeniyle bozulma olması ihtimalinden dolayı eklenmiştir.

* **Nane&Limon-Sunumu.pptx** dökümanı yarışma sonunda yapılacak olan sunum interaktif dökümanıdır.
### Problem?
Siber zorbalık,
Bir kişiyi veya kişinin içinde bulunduğu belli bir topluluğu  hedef alan her türlü aşağılayıcı, küçük düşürücü ve zedeleyici  paylaşımların tümüdür.
UNESCO’nun siber zorbalığın yüksek gelir düzeyindeki  ülkelerde yaygınlığı ile ilgili verilerine göre siber zorbalıktan  etkilenen çocukların ve ergenlerin oranı yüzde 5 ile yüzde 21  arasında değişmektedir. Bu arada kızların bu tür zorbalığa  maruz kalma olasılığı erkeklere göre daha yüksektir.
- Yarışmada, Türkçe metinlerden siber zorbalık yapılması ve yapılan zorbalığın alt kategorisinin yüzdelik oranla ne olduğunu tespit eden bir model geliştirilmesi hedeflenmiştir. 

## Katkılarımız
  Proje kapsamında ;
  * 3388 adet 4 kategorili etiketli güncel [veri seti](https://huggingface.co/datasets/nanelimon/turkish-social-media-bullying-dataset) üretilmiştir.
  * Aşağıda görüldüğü gibi [yüksek başarı oranlarına sahip alt kategorileri bulunan Türkçe Siber Zorbalık modeli]( https://huggingface.co/nanelimon/bert-base-turkish-bullying) kazandırılmıştır. 
  
    |        | Cinsiyetçilik | Irkçılık | Kızdırma | Nötr | 
    | ------ | ------  | ------ | ------  | ------ |
    | Precision | 0.925 | 0.878 | 0.824 | 0.915 |
    | Recall  | 0.831 | 0.896 | 0.843 | 0.935 |
    | F1 Score | 0.875 | 0.887 | 0.833 | 0.925 |

    Accuracy : 0.886
  
  * Oluşturulan yeni veri seti için bir çok yöntem denenerek literatüre henüz yeni katılmış olan bu veri seti için ilk hyper parametre araştırmaları yapılmıştır.([TFIDF & ML modelleri](https://github.com/Teknofest-Nane-Limon/tfidf-model-turkish-bullying) ve [Transformers(BERT)]((https://github.com/Teknofest-Nane-Limon/bert-base-turkish-bullying)) yöntemler denenmiştir.) 
  * Türkçe Doğal Dil İşleme yapılırken diğer araştırmacıların ön işleme adımlarını hızlıca geçebilmeleri için [veri temizleme aracı](https://text-data-cleaner.herokuapp.com/) geliştirilip yayınlanmıştır.
  * Türkçe Doğal Dil İşleme yapacak diğer araştırmacıların ihtiyaç duydukları twitter verileri için hiçbir kütüphaneden hazır bir araç kullanılmayarak **özgün algoritmalar** ile [veri çeken bir bot](https://github.com/Teknofest-Nane-Limon/twitter-scraper) yazılmıştır.
  * Veri etiketleme adımında kendi özgün veri etiketleme aracımızı yazarak bundan sonra yapacağımız çalışmalar için ve diğer bütün veri etiketleme üzerine çalışan araştırmacılar için daha hızlı, kolay ve erişilebilir etiketleyebilmek, çapraz kontrollerini yapabilmek ve istatistiklerine heran ulaşabilmek için [kendi veri etiketleme aracımızı yazdık](https://easy-data-labeling-engine.herokuapp.com/)
  * Oluşturulan başarılı model [ürünleştirilmiştir](https://github.com/Teknofest-Nane-Limon/turkish-bullying-api).
  
  ### Oluşturulan servisin uygulama halini [buradan deneyebilirsiniz.](https://duvar-app.herokuapp.com/)

* ÖNEMLİ NOT:
  > * Çalışma boyunca hiçbir hazır api, kütüphane, veri seti, araç veya model kullanılmamıştır.
  > * Çalışma boyunca hiçbir ücretli uygulama, sunucu veya domain hizmeti kullanılmamıştır.
  


### Yapılan proje adımları aşağıda yer almaktadır.

  ![plot](/img/akış.drawio.png)
  
  Veri Kazıma Demo Videosuna [buradan ulaşabilirsiniz.](https://youtu.be/yn03mcsl42M)
  Araçların tanımın videosuna [buradan ulaşabilirsiniz.](https://www.youtube.com/watch?v=osjWOwDcqvQ&t=4&ab_channel=AlaaddinErdin%C3%A7DAL)
  
  - Adım adım 1: Veri Kazıma Aracı: https://github.com/Teknofest-Nane-Limon/twitter-scraper
  
  - Adım adım 2: Veri Etiketleme Aracı: https://github.com/Teknofest-Nane-Limon/easy-data-labeling-engine
    - Etiketli verinin ürünleştirilmesi: https://huggingface.co/datasets/nanelimon/turkish-social-media-bullying-dataset
  
  - Adım adım 3: Veri Temizleme Aracı: https://github.com/Teknofest-Nane-Limon/text-data-cleaner
  
  - Adım adım 4: Veri Modelleme:
    - 4.1. TFID ile için analiz ve denemeler notebooku: https://github.com/Teknofest-Nane-Limon/tfidf-model-turkish-bullying
    - 4.2 Bert Mobel için analizler ve denemeler notebooku: https://github.com/Teknofest-Nane-Limon/bert-base-turkish-bullying/blob/main/bert-cv.ipynb%20-%20Colaboratory.pdf & bert-cv.ipynb
    - 4.3 Bert Modelden çıkan hyper parametreler ile çıkan moddelleme notebook u: https://github.com/Teknofest-Nane-Limon/bert-base-turkish-bullying/blob/main/bert-base-turkish-bullying-best-parameter.ipynb 
  
  - Adım adım 5: Modelin Ürünleştirilmesi:
    - 5.1 Python FastAPI: https://github.com/Teknofest-Nane-Limon/turkish-bullying-api
    - 5.2 Hugging Face : https://huggingface.co/nanelimon/bert-base-turkish-bullying
    
    
  ## Örnekler
  > Cinsiyetçilik Örneği:
    ![plot](/img/Cinsiyetçilik.jpeg)
  > Irkçılık Örneği:
    ![plot](/img/Irkçılık.jpeg)
  > Kızdırma Örneği:
    ![plot](/img/Kızdırma.jpeg)
  > Nötr Örneği
    ![plot](/img/Nötr.jpeg)
