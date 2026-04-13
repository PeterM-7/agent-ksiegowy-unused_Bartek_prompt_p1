# Backend Installation (Quick Start)

Minimalna ścieżka uruchomienia środowiska backend + frontend MVP.

## 1) Wymagania

- Python 3.10+
- (Opcjonalnie dla OCR obrazów) Tesseract
  - macOS: `brew install tesseract tesseract-lang`
  - Ubuntu/Debian: `sudo apt-get install tesseract-ocr tesseract-ocr-pol`

## 2) Uruchom backend

```bash
cd backend
python3 -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

Backend będzie dostępny na `http://127.0.0.1:8000`.

## 3) Uruchom frontend MVP

W drugim terminalu:

```bash
cd frontend
python3 -m http.server 5500
```

Frontend będzie dostępny na `http://127.0.0.1:5500`.

## 4) Szybka weryfikacja

- Otwórz frontend, wybierz plik faktury i kliknij `Przetwórz dokument`.
- Frontend woła endpoint `POST /api/v1/invoices/upload-and-process`.
- Na ekranie głównym zobaczysz tabelę kluczowych pól faktury.
- Dane techniczne i pełny JSON są dostępne po rozwinięciu panelu administratora.
