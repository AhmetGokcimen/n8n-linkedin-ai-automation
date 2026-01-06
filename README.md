# LinkedIn AI Post Automation (n8n)

Bu n8n workflow'u; belirlenen konularda yapay zeka (Google Gemini) kullanarak içerik üretir, buna uygun görsel oluşturur (Replicate) ve LinkedIn hesabınızda otomatik paylaşır.

![Workflow Şeması](preview.png)
## Özellikler
- 🧠 **İçerik Üretimi:** Google Gemini ile trendlere uygun metin yazar.
- 🎨 **Görsel Üretimi:** Metne uygun prompt oluşturup Replicate (Imagen) ile görsel çizer.
- 🚀 **Otomatik Paylaşım:** LinkedIn API üzerinden paylaşır.
- 💾 **Veritabanı:** Eski paylaşımları Supabase'de tutar (tekrara düşmemek için).

## Kurulum
1. `n8n-linkedin-automation.json` dosyasını indirin.
2. n8n panelinizde "Import from File" diyerek içeri aktarın.
3. Credentials bölümünden kendi API anahtarlarınızı (Supabase, Replicate, Google PaLM, LinkedIn) girin.

## Gereksinimler
- n8n (Self-hosted veya Cloud)
- Replicate Hesabı
- Google AI Studio (Gemini) API Anahtarı
- Supabase Veritabanı
