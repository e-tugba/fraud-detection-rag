# 💳 Gelişmiş Kredi Kartı Dolandırıcılık Analizi Chatbotu

Bu proje, kredi kartı dolandırıcılığı konusuna odaklanan, Türkçe soruları anlayabilen ve bilgi tabanına göre akıllı cevaplar üretebilen bir **Yapay Zekâ Chatbot** uygulamasıdır.  
Amaç, dolandırıcılık tespitine yönelik veri yapısını, kavramları ve süreçleri açıklayabilen etkileşimli bir sistem geliştirmektir.

---

## 🎯 Proje Amacı

Projenin temel amacı, kredi kartı işlemlerinde dolandırıcılığı anlamaya ve tespit etmeye yardımcı olacak bir **RAG (Retrieval-Augmented Generation)** tabanlı chatbot oluşturmaktır.  
Bu sistem, kullanıcıdan gelen Türkçe veya İngilizce soruları alır, bilgi tabanında arama yapar ve en uygun cevabı üretir.  
Yani hem veri bilimi hem de doğal dil işleme birleşerek sade ama işlevsel bir deneyim sunar.

---

## ⚙️ Teknik Özellikler

- **Model:** `google/flan-t5-small`  
- **Embedding:** `sentence-transformers/paraphrase-MiniLM-L6-v2`  
- **Teknolojiler:** Python, Gradio, Hugging Face Spaces  
- **Çalışma Yapısı:**  
  - Kullanıcının sorusu alınır  
  - Soru, bilgi tabanıyla benzerlik açısından değerlendirilir  
  - En uygun içerik seçilir ve kısa, açık Türkçe cevap üretilir  

---

## 🧠 Bilgi Tabanı (Knowledge Base)

Chatbot, kredi kartı dolandırıcılığı veri setine ait temel kavramlarla eğitilmiştir.  
Örneğin:
- Veri setinde toplam 284807 işlem vardır.  
- Sütunlar: `Time`, `V1–V28`, `Amount` ve `Class`.  
- `Class` sütunu 1 ise işlem dolandırıcılıktır, 0 ise normaldir.  
- `V1–V28` sütunları PCA ile anonimleştirilmiştir.  
- `Amount` sütunu işlem tutarını gösterir.  

---

## 💬 Kullanım

1. Chatbot arayüzü açılır.  
2. Türkçe veya İngilizce bir soru yazılır (örneğin: *“Class sütunu neyi gösterir?”*).  
3. Chatbot bilgi tabanını tarar ve en uygun yanıtı verir.  
4. Gerektiğinde “Context göster” seçeneği ile hangi bilgilere dayandığını da görebilirsiniz.

---

## 🖼️ Örnek Çalışma Görseli

Aşağıda chatbot arayüzünden alınmış bir örnek etkileşim ekranı yer almaktadır:

![Fraud Detection Chatbot Ekran Görüntüsü](Screenshot%202025-10-20%20at%2014.34.29.jpg)




Bu örnekte kullanıcı farklı sorular sormuş ve chatbot doğru şekilde bilgi tabanına dayanarak kısa Türkçe yanıtlar üretmiştir.

---

## 🌐 Canlı Demo

Projeyi canlı olarak aşağıdaki bağlantıdan deneyebilirsiniz:  
👉 **[Hugging Face Space Linki](https://huggingface.co/spaces/bayar1/fraud-detection-rag)**  

---

## ✨ Katkı ve Geliştirme

Proje tamamen açık kaynaklıdır.  
Yeni bilgi tabanları, farklı modeller veya Türkçe dil desteğini geliştirecek katkılar memnuniyetle kabul edilir.  

---

## 👩‍💻 Geliştirici

**Tuğba Bayar**  
Bu proje Yapay Zekâ Proje Dersi kapsamında geliştirilmiştir.  
Amaç, RAG tabanlı chatbotların veri bilimi alanında nasıl açıklayıcı ve yardımcı araçlara dönüşebileceğini göstermektir.

---
