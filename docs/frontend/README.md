# Frontend

Katalog frontendu będzie zawierał interfejs użytkownika aplikacji.

## Odpowiedzialność frontendu
- przesyłanie faktur,
- prezentacja wyników analizy,
- umożliwienie edycji i zatwierdzania danych,
- wyświetlanie listy przetworzonych dokumentów,
- uruchamianie eksportu danych.

## Planowane widoki
- ekran uploadu dokumentu,
- ekran podglądu odczytanych danych,
- tabela faktur,
- ekran eksportu lub pobierania danych.

## Status
Zaimplementowany prosty frontend MVP w katalogu `frontend/`:
- upload dokumentu,
- automatyczne wywołanie processingu bez ręcznego `invoice_id`,
- czytelna tabela danych faktury (pola księgowe),
- panel administratora z metadanymi technicznymi i surowym JSON,
- lista ostatnich dokumentów.