# Forecast-algoritms
Machine learning, Deep Learning and Statistical Models

## DISCLAIMER
Time series verilerinde, seriyi olabildiğince ergodik hale getirebilmemiz gerekiyor. Neural Network'te vs 18-30% bandında RMSE almamızın sebebi, network, t+1 anına, t verisinin değerini basıyor. Çünkü x(t+1) ile x(t) arasındaki korelasyon çok yüksek. Hangi forecast algoritmasını kullanırsak kullanalım, seriye önce bir preprocessing uygulamamız lazım. Bunlar:
 - Seriden mevsimsel etkilerin kaldırılması,
 - Autocorrelation'ı düzeltmek için serinin ( x(t) ) logunun alınması ( 1 + log x(t) )
 - Seriyi n tane periyodik ergodik komponente ayırmak
 
gibi şeyler olabilir. Time-series verileri sıkıntılı veriler. Üzerinde biraz düşünmemiz gerekiyor. Şeyda hoca bize bu konuda yardımcı olabilir. (Egemen)

## Statistical Models
* ARIMA, ARMAX
  * Bulutun olmadığı günlerde günlerde sorunsuz çalışıyor. Time-serieslerde oldukça yaygın kullanılan bir model. Bir iki döküman ekliyorum. Benim (Nail), en zayıf olduğum konu bu. Mendeleye de yayın ekleyeceğim.
  
 ## Neural Networks
 * Weather datalarını ve saati feature olarak ekledim. Hata RMSE %18-30 bandında. Fakat dandik olması literaturede de belirtilmiş. Sonuçta time-series ve önceki değerlere oldukça bağlı. Sonuçları ve modeli yine bu klasöre ekleyeceğim
 
  ## Deep Belief Network
  * Literature de gördüm hiçbir fikrim yok. Araştırılabilir.
  
  ## LSTM
  * Univariate olanı denedim(Sadece geçmiş power verileri var yani 1-d array ). Daha önce egemenle bir model geliştirmiştik günlük veriler üzerine ve %10 a yakın bir RMSE elde etmiştik.
    * Univariate LSTM (5-min resolution) %4.5 RMSE optimizer (rmsprop) ki fazla iyi. Bu kadar iyi olmamalı (possible overfit). Loss grafiklerini ekleyeceğim tartışılabilir. Fazla iyi olmasına rağmen bir yayında da aynı RMSE yi bulmuş. Adamlar kendi datasetlerini paylaşıyorlar onlarınkini alıp bizim modelde test edebiliriz. [Yayın](buraya link gelecek.)
    
   ## Seq2Seq, causal network, attention
  * Bence en çok fayda göreceğimiz bu. Derinine kadar bilmiyorum fakat [LSTM'e karşı olarak çıkmış bir algoritma](https://towardsdatascience.com/the-fall-of-rnn-lstm-2d1594c74ce0)
