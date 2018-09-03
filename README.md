# Forecast-algoritms
Machine learning, Deep Learning and Statistical Models
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
