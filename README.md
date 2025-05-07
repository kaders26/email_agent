# 🤖 Email Agent

**Email Agent**, gelen e-postaları yönetmek ve yanıtlamak için tasarlanmış akıllı bir asistandır. OpenAI'nin GPT-4o modeli kullanılarak geliştirilen bu ajan, profesyonel HTML formatında e-postalar oluşturur ve imza olarak her mesajın sonuna “Nate” ismini ekler.

## 📌 Özellikler

- Gelen e-postaları analiz eder ve otomatik olarak yanıt oluşturur.
- E-posta gönderme, taslak oluşturma, yanıtlama, etiketleme ve okunmamış olarak işaretleme işlemlerini destekler.
- Gmail API ile entegredir.
- n8n platformu üzerinden sürükle-bırak ile görsel akış desteği.

## ⚙️ Kullanılan Teknolojiler

- [n8n](https://n8n.io/) (otomasyon platformu)
- OpenAI GPT-4o
- Gmail OAuth2 entegrasyonu
- Langchain agent + tool sistemi

## 🧠 Agent Yapılandırması

- **Model:** GPT-4o
- **Rol Tanımı:** E-posta yönetim asistanı
- **Prompt (Sistem Mesajı):**
  - Gelen tüm e-postalar profesyonel HTML formatında yanıtlanmalıdır.
  - Mesajlar “Nate” adıyla imzalanmalıdır.
  - Ajan; gönderme, yanıt, taslak oluşturma, etiketleme ve okunmamış yapma gibi işlemler için uygun araçları kullanmalıdır.
  
## 🛠️ Kullanılabilir Araçlar

| Araç | Açıklama |
|------|----------|
| `Send Email` | Yeni e-posta gönderir |
| `Create Draft` | Taslak oluşturur |
| `Get Emails` | Gelen kutusundaki e-postaları getirir |
| `Get Labels` | Gmail etiketlerini listeler |
| `Label Email` | Belirli bir e-postaya etiket uygular |
| `Mark Unread` | E-postayı okunmamış olarak işaretler |
| `Email Reply` | Gelen bir e-postaya yanıt verir |

