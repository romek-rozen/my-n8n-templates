# My n8n Templates

Kolekcja workflow'ów n8n do automatyzacji różnych procesów biznesowych i technicznych.

## 📋 Lista Workflow'ów

### RSS Reader to Google Sheets
**Lokalizacja:** `RSS READER TO GOOGLE SHEETS/`

Zaawansowany workflow do automatycznego:
- Czytania feedów RSS z listy w Google Sheets
- Filtrowania duplikatów (sprawdza już przetworzone artykuły)
- Pobierania pełnej treści artykułów
- Generowania podsumowań AI za pomocą modelu Gemini
- Zapisywania wyników do Google Sheets

**Funkcje:**
- ⏰ Automatyczne uruchomienie co godzinę
- 🔄 Filtrowanie artykułów z ostatnich X dni (konfigurowalny)
- 🤖 Inteligentne podsumowania AI w strukturyzowanym formacie
- 📊 Integracja z Google Sheets
- 🚫 Automatyczne pomijanie duplikatów

### Export Markdown Content to Google Docs
**Lokalizacja:** `Export_Markdown_Content_do_Google_Docs_Document/`

Workflow do eksportowania treści Markdown do dokumentów Google Docs.

## 🛠️ Konfiguracja

### Wymagania
- Konto n8n (cloud lub self-hosted)
- Konta Google (Sheets, Docs)
- Klucze API dla usług AI (OpenRouter)

### Instalacja
1. Importuj plik JSON workflow'u do n8n
2. Skonfiguruj credentiale dla:
   - Google Sheets API
   - Google Docs API
   - OpenRouter API (dla AI)
3. Dostosuj ustawienia w node'zie "Settings"

## 📖 Dokumentacja

Każdy workflow zawiera:
- Plik JSON z definicją workflow'u
- Instrukcje setup'u
- Opis funkcjonalności
- Przykłady konfiguracji

## 🤝 Współpraca

Jeśli masz pomysły na ulepszenia lub nowe workflow'y, otwórz issue lub wyślij pull request.

## 📄 Licencja

MIT License - możesz swobodnie używać, modyfikować i dystrybuować te workflow'y.

---

**Autor:** Roman Rozenberger  
**Email:** roman@ibb.media
