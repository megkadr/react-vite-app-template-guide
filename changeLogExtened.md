# Dziennik zmian

Poniżej znajduje się przefiltrowany dziennik zmian, sformatowany w Markdown, zawierający wyłącznie zmiany wpływające na produkt. Usunięto elementy takie jak wewnętrzne zadania CI, aktualizacje zależności, zadania porządkowe oraz niejasne komunikaty, pozostawiając jedynie kluczowe funkcje i poprawki błędów.

---

## 03.02.2025 – 09.02.2025

### Backend 2.1.0 (2025-02-06)
#### 🚀 Nowe funkcje i ulepszenia
- **api:** Logika wykonania dla ActionButtons  
- **functions:** Dodano funkcję do drukowania dokumentów zamówień  
- **functions:** Dodano wysyłki GLS  
- **functions:** Dodano synchronizację zamówień Kaufland  
- **functions:** Dodano synchronizację etykiety dostawy InPost  
- **functions:** Dodano synchronizację zamówień WooCommerce  
- **functions:** Utworzenie przesyłki DPD  
- **functions:** Funkcje zarządzania produktami zamówień  
- **functions:** Zapewniono subiekt voppi  
- **web:** Dodano szczegóły przesyłki  
- **workflows:** Zmiany związane z walidacją workflow  

#### 🐛 Poprawki błędów
- **api:** Dopasowano nazewnictwo ReadDto dla ActionButtons  
- **functions:** Naprawiono Allegro Provider  
- **functions:** Naprawiono synchronizację dla Erli i Mirakl  

---

## 10.02.2025 – 16.02.2025

### Backend 2.2.0 (2025-02-13)
#### 🚀 Nowe funkcje i ulepszenia
- **workflows:** Dodano wysyłkę e-maili  

### Backend 2.2.2 (2025-02-13)
#### 🐛 Poprawki błędów
- Nie waliduj pustych wyrażeń regularnych  

---

## 17.02.2025 – 23.02.2025

### Backend 2.3.0 (2025-02-17)
#### 🚀 Nowe funkcje i ulepszenia
- **functions:** Dodano synchronizację zamówień Amazon  

### Backend 2.4.0 (2025-02-17)
#### 🐛 Poprawki błędów
- **functions:** Naprawiono synchronizację zamówień Amazon (OrderSync)  

### Backend 2.4.1 (2025-02-18)
#### 🐛 Poprawki błędów
- Dodano szczegółowe logowanie i timeouty dla poleceń scalania  
- Dodano brakujące mapowanie dla klienta Amazon  

### Backend 2.4.2 (2025-02-18)
#### 🐛 Poprawki błędów
- Dostosowano czasy wykonania  

### Backend 2.6.0 (2025-02-18)
#### 🚀 Nowe funkcje i ulepszenia
- Zdefiniowano parametr wywołującego  
- Zwiększono rozmiar partii  

#### 🐛 Poprawki błędów
- Naprawiono integrację z Allegro  

### Backend 2.7.0 (2025-02-19)
#### 🚀 Nowe funkcje i ulepszenia
- Dodano domyślną wartość dla polityk  
- **api:** Dodano uprawnienia i polityki  
- **functions:** Dodano agregację statusów zamówień  
- **web:** Lista użytkowników z endpointu API  

#### 🐛 Poprawki błędów
- **api:** Naprawiono GetShipmentStatus  
- **api:** Rozwiązano problemy z najnowszymi błędami i żądaniami nowych funkcji  

### Web 1.10.0 (2025-02-19)
#### 🚀 Nowe funkcje i ulepszenia
- Wyświetlanie źródła w szczegółach zamówienia i na liście zamówień  
- Przycisk powiększania/zmniejszania statusów zamówień  
- Dwie cyfry po przecinku dla kwoty zamówienia  
- Lista użytkowników z endpointu API  

---

### Backend 2.8.0 (2025-02-19)
#### 🚀 Nowe funkcje i ulepszenia
- Dodano politykę ponawiania MassTransit  

### Backend 2.8.1 (2025-02-19)
#### 🐛 Poprawki błędów
- Zmieniono filtry zamówień  

### Backend 2.9.0 (2025-02-20)
#### 🚀 Nowe funkcje i ulepszenia
- **api:** Dodano endpoint GetPaginatedEmagAccounts  
- **api:** Dodano endpoint GetPaginatedWooCommerceAccounts  

#### 🐛 Poprawki błędów
- Naprawiono nieprawidłowe ceny w paginacji  

### Web 1.11.0 (2025-02-20)
#### 🚀 Nowe funkcje i ulepszenia
- Wyświetlanie liczby zamówień dla poszczególnych statusów  
- Uprawnienia użytkowników  

#### 🐛 Poprawki błędów
- Naprawiono filtry zamówień  

---

### Backend 2.10.0 (2025-02-21)
#### 🚀 Nowe funkcje i ulepszenia
- **api:** Dodano endpoint GetPaginatedAmazonAccounts  

#### 🐛 Poprawki błędów
- Ustawiono statusy na 0 dla zamówień bez pozycji  

### Web 1.12.0 (2025-02-21)
#### 🚀 Nowe funkcje i ulepszenia
- Lista kont Kaufland  
- Nowy system komunikatów o błędach i obsługa uprawnień  

#### 🐛 Poprawki błędów
- Naprawiono licznik zamówień w statusach oraz obsługę filtrów

---
