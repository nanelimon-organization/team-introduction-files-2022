<h1 align = 'Center'>Nane&Limon 🐍 Teknofest 2022 TDDİ Repository</h1>

<div>Bu depo Teknofest 2022 Kapsamında Türkçe Doğal Dil İşleme Yarışması katılımcısı Nane&Limon ekibinin dökümanlarını içermektedir.</div>


* **Nane&Limon-Tanıtım.pdf** dökümanı yarışmaya katılmak için oluşturulan ilk dökümandır.

* **Nane&Limon-Sunumu.pdf** dökümanı yarışma sonunda yapılacak olan sunum pdf idir.
  > Not: Cihaz farkı nedeniyle bozulma olması ihtimalinden dolayı eklenmiştir.

* **Nane&Limon-Sunumu.pptx** dökümanı yarışma sonunda yapılacak olan sunum interaktif dökümanıdır.

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
