<div align="center">

# 🧪 LangChain Lab

**Gelişmiş Yapay Zeka Ajanları ve LLM Orkestrasyonu için Deneysel Çalışma Alanı**

[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![LangChain](https://img.shields.io/badge/LangChain-Integration-green.svg?style=for-the-badge&logo=chainlink&logoColor=white)](https://langchain.com/)
[![License](https://img.shields.io/badge/License-MIT-purple.svg?style=for-the-badge)](LICENSE)

*Profesyonel düzeyde yapay zeka entegrasyonları, bağlam yönetimi ve yapılandırılmış çıktı mimarilerinin test edildiği araştırma ve geliştirme laboratuvarı.*

</div>

---

## 📖 Proje Hakkında

**LangChain Lab**, büyük dil modelleri (LLM'ler) ile çalışırken karşılaşılan karmaşık problemleri çözmek, model performansını optimize etmek ve güvenli, yapılandırılabilir ajanlar (AI Agents) geliştirmek amacıyla oluşturulmuş bir deney ortamıdır. 

Bu laboratuvar, özellikle **Middleware (Ara Katman)**, **Structured Output (Yapılandırılmış Çıktı)** ve **Context Management (Bağlam Yönetimi)** gibi ileri düzey LangChain konseptlerinin derinlemesine incelendiği Jupyter Notebook'larından oluşmaktadır.

---

## 🏗️ Temel Mimari ve Özellikler

Proje, her biri belirli bir LLM entegrasyonu ve orkestrasyonu konseptine odaklanan modüler notebook'lara ayrılmıştır:

### 🛡️ Middleware & Hooks (`middleware.ipynb`)
Yapay zeka modelleri ile kullanıcı arasındaki iletişimi denetleyen "yazılım köprüsü" yapıları.
- **Summarization Middleware:** Token sınırlarını aşmamak ve maliyetleri düşürmek için konuşma geçmişini (Context Window) özyinelemeli (Recursive Summarization) olarak özetleyen ara katman.
- **Lifecycle Hooks:** İşlem akışına müdahale eden kancalar (`Pre-processing`, `On-processing`, `Post-processing`).
- **Model Call limits:** Aşırı API maliyetini önlemek için model çağrı sayılarını sınırlandıran güvenlik kalkanları (Guardrails).

### 📐 Yapılandırılmış Çıktılar (`structured_outpuy.ipynb`)
LLM'lerin tutarlı ve programatik olarak işlenebilir veri dönmesini sağlayan mimariler.
- **Nested Structures:** Gerçek dünya verilerini modellemek için iç içe geçmiş Pydantic BaseModels (örn. Film -> Oyuncu listesi).
- **TypeDict & DataClass:** Çalışma zamanı doğrulamasına (runtime validation) ihtiyaç duyulmayan hafif yapılar ve tekrarlayan kodlardan (`__init__`) kurtaran Data Class kullanımları.

### 🔌 Model Entegrasyonu (`model_integration.ipynb`)
Farklı LLM sağlayıcılarının sisteme entegrasyonu, model parametrelerinin optimizasyonu ve kesirli (fraction) hesaplamalar gibi özel kullanımlar.

### 🛠️ Araç Kullanımı ve Mesajlaşma (`tools.ipynb`, `messages.ipynb`)
- Ajanların dış dünyayla etkileşime girmesini sağlayan özel fonksiyon donanımları (Custom Tools).
- LangChain mesaj tipleri (SystemMessage, HumanMessage, AIMessage) üzerinden karmaşık diyalog ağaçlarının inşası.

---

## 🚀 Başlangıç Rehberi

### Gereksinimler
- Python 3.11 veya üzeri

### Kurulum

1. Repoyu bilgisayarınıza klonlayın:
```bash
git clone https://github.com/MustafaKocamann/Langchain-Lab.git
cd Langchain-Lab
```

2. Sanal bir ortam (Virtual Environment) oluşturun ve aktif edin:
```bash
python -m venv venv
# Windows için:
.\venv\Scripts\activate
# Linux/macOS için:
source venv/bin/activate
```

3. Gerekli bağımlılıkları yükleyin:
```bash
pip install -r requirements.txt
```

4. Çevre değişkenlerini ayarlayın:
`.env` adında bir dosya oluşturun ve gerekli API anahtarlarınızı ekleyin (örn. `OPENAI_API_KEY`, `GROQ_API_KEY` vb.).

---

> [!TIP]
> **Daha İyi Bir Performans İçin:**
> Token maliyetlerini optimize etmek için özellikle uzun metin analizlerinde `Summarization Middleware` yapısını sisteminizde aktif olarak kullanmayı unutmayın.

---

## 👨‍💻 Yazar ve İletişim

Bu proje, yapay zeka sistem mimarileri ve ileri düzey LLM orkestrasyonu konularında araştırmalar yapan **Mustafa Kocaman** tarafından geliştirilmektedir.

📧 **Email:** [mustafakocaman789@gmail.com](mailto:mustafakocaman789@gmail.com)  
🔗 **GitHub:** [@MustafaKocamann](https://github.com/MustafaKocamann)

<div align="center">
  <sub>World-Class Technical Documentation by Design.</sub>
</div>
