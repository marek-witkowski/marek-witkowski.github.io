

## Wdrożenia pomysłów:


### Automatyczne sprawdzanie pisowni (MS Word, VBA)

W trakcie tłumaczeń pojawiały się liczne czeskie i interpunkcyjne błędy w tekście. Stworzyłem prosty program używający API MS Worda do sprawdzania pisowni i wyrzucający listę błędów do osobnego pliku. 

Korzyści:
* Wzrost jakości pracy - na każde 1000 stron tekstu skrypt wychwytywał 30-50 niezauważonych wcześniej błędów.


### Aplikacja urlopowa (ASP, MS SQL Server)

Zamiast biegać z papierami albo wysyłać maile do przełożonych pracownik wypisywał sobie na stronie podanie o urlop. Przełożony dostawał maila, z informacją o prośbie o zatwierdzenie urlopu. Jak zatwierdził, pracownik (a za nim kadry) dostawał maila, że ma urlop, w przeciwnym razie dostawał maila z odmową. 

Korzyści:
* Przyspieszenie obiegu dokumentów z paru godzin lub dni do ok. godziny
* Podgląd stanu pracowników przez PMów
* Oszczędność czasu pracowników oraz PMów na wypełnianiu pisemnej formy dokumentów.
* Używana przez ok. 100 osób
* Podgląd działu HR w plany urlopowe.


### Zamówienia wewnętrzne (ASP, MS SQL Server)

Rodzaj sklepu internetowego, w którym pracownik, jeśli miał jakieś potrzeby związane z finansowaniem przez firmę, wypełniał formularz, opisując potrzebę i budżet. Najpierw „podanie” musiał zatwierdzić kierownik, a potem dział finansowy. Jeśli obie instancje zaakceptowały - dostawał zgodę na zakup. 

Korzyści:
* Przyspieszenie obiegu dokumentów z paru godzin lub dni do ok. godziny
* Oszczędność czasu pracowników oraz PMów na wypełnianiu pisemnej formy dokumentów.
* Dyrektor finansowy ma stały i aktualny podgląd dot. realizacji potrzeb zakupowych pracowników.


### Słownik online (C#, ASP, MS SQL Server)

W testowaniu tłumaczeń pracownicy używali Excela albo plików TXT z funkcją “szukaj”. Wdrożyłem aplikację własnego pomysłu opartą o aplikację desktopową (później webową) + baza danych. 

Korzyści:
* Większa spójność tłumaczeń - wszyscy korzystali z tego samego słownika, (ok. 50 osób)
* Znacznie większa prędkość pracy oraz skuteczność wyszukiwania – nawet 5-ciokrotne przyspieszenie.
* Dzięki zwiększeniu skuteczności wyszukiwania - zmniejszyła się liczba błędów o ok. 10-15%


### Odblokowywacz(Java, C#)

W starym systemie księgowo-sprzedażowym był błąd polegający na niespodziewanym blokowaniu dokumentów do edycji. Napisałem aplikację pozwalającą naprawić błędnie założone blokady pracownikom, przez co nie potrzebowali wsparcia działu IT.

Korzyści:
* Szybsza praca biura - oszczędzono ok. 16 roboczogodzin miesięcznie
* Brak zatorów w IT spowodowanych ilością próśb o odblokowanie czegoś zwłaszcza pod koniec miesiąca. (oszczędzono ok. 8 roboczogodzin miesięcznie)
* Używana przez ok. 20 osób/4 działy.
  
Projekt na GitHubie (Java): https://github.com/marek-witkowski/jUnLocker
Projekt na GitHubie   (C#): https://github.com/marek-witkowski/UnLocker


### Raportownik (Java, Oracle)

Aplikacja wyciągająca z systemu raporty sprzedażowe i wysyłająca je kontrahentom. 

Korzyści:
* Firma zaoszczędziła na płaceniu firmie zew. ok. 10000 za aplikację oraz ok. 500 miesięcznie za obsługę,
* Zmniejszył się czas rozwiązywania problemów z paru godzin (firma zewnętrzna) do kwadransa (lokalny dział IT)
* W związku ze znacznym zmniejszeniem awaryjności oraz szybszymi reakcjami na problemy zwiększył się poziom zadowolenia kontrahentów otrzymujących raporty.

Projekt na GitHubie: https://github.com/marek-witkowski/EasyReports

## Archiwizator faktur (MS SQL, C#)

Faktury w dużych ilościach były drukowane i wysyłane klientom wraz z towarem. Napisałem program archiwizujący wysłane faktury w formie plików PDF, dzięki czemu pracownicy potrzebujący ponownie wysłać komuś dokument albo księgowość chcąc coś sprawdzić - nie musieli ponownie drukować dokumentu (wada starego systemu), tylko korzystali z archiwum plikowego. 

Korzyści:
* Oszczędność kosztów tonera oraz czasu serwisowania drukarek (z tygodnia do 1 godziny)
* Szybszy dostęp do dokumentów oszczędził czas pracy księgowości oraz ekspedycji (z paru minut do poniżej minuty na dokument).

Projekt na GitHubie: https://github.com/marek-witkowski/ArchiwizatorFaktur

## Wykres obciążenia magazynów (PHP, JS)

Kierownicy magazynu mieli wykresy, na których widzieli, ile zamówień spływa na konkretne magazyny i wg tego mogli kierować pracą zespołu.

Korzyści:
* optymalizacja pracy załogi - dzięki stałemu podglądowi on-line decyzje kierowników na magazynie mogły być niemal natychmiastowe,
* brak kosztów związanych z wynajęciem firmy zewnętrznej do tworzenia aplikacji - oszczędność ok. 3000 PLN

Projekt na GitHubie: https://github.com/marek-witkowski/WarehouseTraffic

### Punkty POI w placówkach klienckich (Linux, Raspberry Pi)

Wymiana komputerów wyświetlających reklamy u klientów (system kosztowny i skomplikowany) na system mojego pomysłu i wykonania. 

Korzyści:
* Obniżono koszty zakupu nowych urządzeń z 25 000 do 2 500
* Uproszczono zarządzanie treścią - dało to oszczędność w pracy osoby obsługującej rzędu 10-20%
* Zminimalizowano przerwy w pracy ze względu na problemy z siecią/awarię aplikacji z ok 70% do 99%


### Generator lokalizacji (C#, ZPL>)

Łatka na system, umożliwiająca pracownikom magazynu drukować naklejki magazynowe na drukarkach etykiet. 

Korzyści:
* Pracownicy mogli sobie drukować potrzebne materiały bez pomocy działu IT, co wyeliminowało czas oczekiwania na druk oraz potrzebę chodzenia po wydruki do działu IT – aplikacja obsługiwała wszystkie drukarki etykiet w firmie.

Projekt na GitHubie: https://github.com/marek-witkowski/GeneratorLokalizacji


## Projekty, w których brałem udział:

* Wdrożenie w firmie systemu klasy ERP oraz organizowanie szkoleń.
* Wymiana systemu drukowania. Korzyści:
  * Optymalizacja zużycia materiałów eksploatacyjnych
  * Zmniejszenie przestojów urządzeń z paru dni do jednej godziny
* Wymiana telefonii z analogowej na VoIP. Korzyści:
  * obniżenie kosztów o połowę
  * uproszczenie infrastruktury telekomunikacyjnej
* Wdrożenie systemu monitoringu infrastruktury. Korzyści:
  * szybszy czas wykrywania i eliminowania problemów w infrastrukturze (z parędziesięciu do ok minuty)
  * Dzięki szybszemu czasowi wykrywania problemów - zmniejszenie przestoju firmy do 1% czasu pracy
* Wdrożenie RODO oraz organizacja szkoleń.
