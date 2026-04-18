📱 Mobile Automation & Cloud-Ready Testing Suite

Prowadzący: mgr Mariusz Dworniczak
Student: Paweł Bieniecki
Numer Albumu: 87364

🏗️ Architektura Projektu (Marketing & Tech Stack)

Projekt przedstawia kompletny ekosystem testowy oparty na podejściu Cloud-Ready / Headless. Zamiast korzystać z ciężkich emulatorów, wykorzystano narzędzia CLI, analizę statyczną, konteneryzację (Docker) oraz automatyzację procesów (pipeline).

Główne technologie:

Język: Python 3.10+
Automatyzacja UI: Appium 2.x
Infrastruktura: Docker & Docker Compose
Raportowanie: Allure Framework
Analiza: MobSF (Static Analysis) & ADB CLI
📅 PRZEBIEG LABORATORIUM (Kamienie Milowe)
🔹 BLOK 1: Tooling & Environment (Infrastruktura)

Przygotowanie środowiska w modelu kontenerowym.

Co zrobiono: Pobranie i konfiguracja obrazów appium, android-sdk oraz mobsf.
Wniosek: Docker pozwala uniknąć problemów z konfiguracją środowiska i zapewnia powtarzalność — każdy uruchamia identyczne środowisko niezależnie od systemu.
🔹 BLOK 2: Debugowanie i Analiza Statyczna (MobSF)

Zrozumienie działania aplikacji przed testami.

Co zrobiono: Skanowanie plików APK pod kątem podatności i uprawnień.
Wniosek: Analiza statyczna pozwala wykryć potencjalne problemy bezpieczeństwa i błędy bez uruchamiania aplikacji.
🔹 BLOK 3-4: Fundamenty Skryptowania (Python for QA)

Budowa podstaw logiki testowej.

Co zrobiono: Praca ze strukturami danych (listy, słowniki), funkcjami oraz podstawową obsługą plików i wyjątków.
Wniosek: Python umożliwia szybkie tworzenie czytelnych i łatwych w utrzymaniu testów.
🔹 BLOK 5-7: Hybrydowe Testowanie API (Requests & Pytest)

Testowanie warstwy backendowej aplikacji.

Co zrobiono: Testowanie endpointów REST (JSONPlaceholder), obsługa kodów HTTP i asercje danych JSON.
Wniosek: Testy API pozwalają wykryć błędy wcześniej i są szybsze niż testy UI.
🔹 BLOK 8: Appium UI Automation (Deep Dive)

Automatyzacja interfejsu użytkownika.

Co zrobiono: Wykorzystanie selektorów (ID, XPath), symulacja kliknięć, wpisywania tekstu oraz nawigacji w aplikacji.
Wniosek: Testy UI odwzorowują realne zachowanie użytkownika, ale są bardziej kosztowne i wolniejsze.
🔹 BLOK 9: Konteneryzacja Serwera (Docker Compose)

Oddzielenie środowiska testowego od systemu.

Co zrobiono: Utworzenie pliku docker-compose.yml do zarządzania serwerem Appium.
Wniosek: Konteneryzacja upraszcza zarządzanie zależnościami i umożliwia szybkie uruchamianie środowiska.
🔹 BLOK 10: MASTER PIPELINE (Capstone Project) 🏆

Automatyzacja pełnego procesu testowego.

Co zrobiono: Stworzenie skryptu pipeline.py, który:
Uruchamia środowisko Docker
Wykonuje testy API i UI
Generuje raport Allure
Czyści środowisko po zakończeniu
Wniosek: Pipeline automatyzuje cały proces testowy i pozwala na łatwe wdrożenie w CI/CD.
📊 Raportowanie Wyników (Allure)

Projekt wykorzystuje raportowanie Allure, które umożliwia:

Śledzenie kroków testowych (@allure.step)
Analizę błędów wraz z załącznikami (screeny, logi)
Dokumentowanie środowiska w sekcji Environment