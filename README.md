# OutPost
# Wizja

## Spis treści

1. Wstęp
   
   1.1 Cel dokumentu
   
   1.2 Zakres
   
   1.3 Definicje, akronimy i skróty
   
   1.4 Referencje
   
   1.5 Omówienie dokumentu
   
2. Umiejscowienie problemu
   
   2.1 Korzyści biznesowe
   
   2.2 Zdefiniowanie problemu
   
   2.3 Umiejsowienie produktu
   
3. Charakterystyka użytkowników
   
   3.1 Demografia rynku
   
   3.2 Użytkownicy
   
   3.3 Środowisko użytkownika
   
   3.4 Profile uzytkowników
   
   3.4.1 Nadawca
   
   3.4.2 Odbiorca
   
   3.5 Kluczowe wymagania
   
   3.6 Rozwiązania alternatywne
   
   3.6.1. InPost
   
   3.6.2. DPD
   
   3.6.3. PoczteX
   
4. Omówienie produktu
   
   4.1 Kontekst produktu
   
   4.2 Podsumowanie możliwości
   
   4.3 Założenia i zależności
   
   4.4 Koszty
   
   4.5 Licencje i instalacja
   
5. Funkcjonalność produktu
   
   5.1. Zaloguj się do systemu
   
   5.2. Nadanie Paczki
   
   5.3. Odbierz Paczkę
   
   5.4. Śledź Paczkę
   
   5.5. Zmień datę odbioru
   
   5.6. Złóż zażalenie
   
   5.7. Zmiana Statusu Paczki
   
   5.8. Przydziel zadania Kurierom
   
   5.9. Rozpatrz zażalenie
   
6. Ograniczenia
7. Normy jakościowe
8. Priorytety realizacji
9. Pozostałe wymagania
   
   9.1 Standardy
   
   9.2 Wymagania systemowe
   
   9.3 Wymagania wydajnościowe
   
   9.4 Wymagania środowiskowe
   
10. Wymagana dokumentacja
    
    10.1 Podręcznik użytkownika
    
    10.2 Pomoc online
    
    10.3 Instalacja i konfiguracja

# Wizja

## 1. Wstęp

### 1.1. Cel dokumentu

Celem dokumentu wizji jest zebranie, analiza i zdefiniowanie cech a także zasad funkcjonowania systemu Outpost, który to system jest częścią większego systemu kurierskiego. Wizja projektu określa jego ogólne założenia. Odpowiada na pytania, co dany projekt ma zrobić, po co ma to zrobić i jak orientacyjnie można zrealizować postawione mu zadania. W praktycznym wymiarze dokument wizji może stanowić wskazówkę dla projektantów systemów informatycznych jak i innych podmiotów zaangażowanych w realizację projektu. Dla nich wszystkich może być także narzędziem motywacyjnym, przypominającym o dalekosiężnych celach projektu.

### 1.2. Zakres

Niniejszy dokument wizji opisuje działanie podsystemu firmy kurierskiej. Jest on częścią większego systemu, który zajmuje się logistyką, kwestiami kadrowymi czy zarządza dostępem do baz danych pracowników i przesyłek a także zajmuje się ich ochroną. Zakresem zagadnień omawianego podsystemu jest cały proces obsługi fizycznej przesyłki, od momentu przyjęcia zlecenia na jej dostarczenie, przez proces jej transportu, po rozliczenie się z klientem z wykonania usługi. Zadaniem niniejszego podsystemu jest usprawnienie funkcjonowania firmy kurierskiej w zakresie obsługi przesyłek a także dodanie nowych funkcjonalności do świadczonych usług np. obsługa paczkomatów.
   
### 1.3. Definicje, akronimy i skróty

- Klient – zewnętrzny użytkownik serwisu
- Pracownik – użytkownik systemu zatrudniony przez firmę kurierską
- Klient Nadawca – Klient nadający paczkę przez usługę
- Klient Odbiorca – Klient odbierający przesyłkę z paczkomatu
- Kurier – pracownik, dostawca paczek do domu klienta lub paczkomatu
- Kurier paczkomatowy - Kurier, który dostarcza lub odbiera paczki z/do paczkomatu
- Kurier domowy - Kurier, który dostarcza lub odbiera paczki z/do nie-paczkomatu
- Administracja – pracownik obsugłujący kurierów lub logistykę
- Skaner - urządzenie używane przez Kuriera do używania systemu

### 1.4. Referencje

Płatności internetowe w systemie Outpost są realizowane zgodnie z rekomendacjami dotyczącymi bezpieczeństwa płatności internetowych w państwach członkowskich Unii Europejskiej opracowanymi przez Europejskie Forum ds. Bezpieczeństwa Płatności Detalicznych.

Europejskie Forum ds. Bezpieczeństwa Płatności Detalicznych. (2013) Rekomendacje dotyczące bezpieczeństwa płatności internetowych (Numer katalogowy UE QB-30-13-188-EN-N). https://www.knf.gov.pl/knf/pl/komponenty/img/Rekomendacje_bezpieczenstwo_platnosci_internetowych_37934.pdf


### 1.5. Omówienie dokumentu

Pozostała część dokumentu w pierwszej kolejności zarysuje tło, na którym będzie funkcjonować opisywany system. Omówione zostanie tło biznesowe a także specyfika rynku i użytkowników. W dalszej kolejności system zostanie szczegółowo opisany - idea, koszty, funkcjonalności. Ostatecznie poruszone zostaną tematy prawne, kwestie norm jakościowych a także wymogów systemowych, środowiskowych czy dokumentacyjnych.

## 2. Umiejscowienie problemu

### 2.1. Korzyści biznesowe

- Stworzenie linii komunikacji między użytkowanikami systemu, co spowoduje przyspieszenie obsługi klienta. W związku z powyższym firma będzie w stanie obsłużyć większą ilość klientów.
- Odciążenie firm kurierskich i przewozowych na poziomie logistycznym. Lepsze i oszczędniejsze zaplanowanie trasy kuriera co skutkuje oszczędnościami na paliwie.

### 2.2. Zdefiniowanie problemu

- Problem: Zapotrzebowanie na system obsługujący nadawanie, śledzenie,odbiór przesyłek oraz obsługę paczkomatów.
- Dotyczy: Firmy kurierskiej Outpost
- Którego skutkiem jest: Niski poziom usług kurierskich - problemy ze śledzeniem przesyłek, brak elastyczności terminu oraz miejsca odbioru, 
- Satysfakcjonujacym rozwiązaniem było by: Stworzenie oprogramowania obsługującego nadanie, odbiór paczki z przejrzystym interfejsem

### 2.3. Umiejsowienie produktu

- Dla: Firmy Outpost obsługującej serwisy kurierskie
- Która: Potrzebuje oprogramowania do nadawania oraz obioru przesyłek
- (System Outpost): Aplikacja do obsługi przesyłek
- Który: Jest niezawodny, ma niskie koszty operowania i utrzymania, zapewnia większą elastyczność od podobnych serwisów, jest prosty do rozszerzenia o funkcje w zależności od przyszłych potrzeb firmy Outpost.
- W przeciwienstwie do: Inpost, dpd, pocztex
- Nasz produkt: Pozwala klientom firmy Outpost na zmianę terminu oraz miejsca odbioru przesyłek z minimalnym kosztem ze strony firmy.

## 3. Charakterystyka użytkowników

### 3.1. Demografia rynku

Aplikacja adresowana do użytkowników telefonów komórkowych, liczba użytkowników może sięgać od miliona wzwyż użytkowników, kwota przeznaczana na nadanie paczki powinna oscylować w granicach 15-50 zł, może być nawet wyższa w zależności od gabarytów. Aplikacje zapewniające obsługę paczek, mają na rynku dobrą reputację, jednak jest parę kwestii nad którymi warto pracować, aplikacje umożliwiają klientom nadawanie i odbieranie paczek bez wychodzenia z domu, przy niewielkim nakładzie czasu. Nasza aplikacja umożliwia zachowanie popularnych rozwiązań stosowanych przez dostawców usług obsługi paczek oraz kilka ulepszeń, takich jak na przykład możliwość zmiany miejsca dostawy przez odbiorcę oraz ulepszenie kontaktu z kurierami.

### 3.2. Użytkownicy

| Nazwa | Opis | Rola |
| --- | --- | --- |
| Nadawcy przesyłek | Osoby lub firmy, które wysyłają przesyłki za pośrednictwem serwisu | Wprowadzają szczegóły przesyłek do systemu. Oczekują na potwierdzenie dostawy. Mają możliwość śledzenia przesyłki |
| Odbiorcy przesyłek | Osoby lub firmy, które odbierają przesyłki dostarczone przez kurierów. | Odbierają przesyłki. Potwierdzają dostawę. Mogą zgłaszać problemy z dostawą. Mogą w określonym zakresie zmieniać termin oraz miejsce odbioru Mają możliwość śledzenia przesyłki |
| Kurierzy | Pracownicy firmy Outpost | Przewożą paczki między magazynem a paczkomatem lub adresem klienta. Korzystają z systemu przez aplikacje skanera paczek. |
| Administracja | Pracownicy firmy Outpost | Przydzielają pojazdy i grafik kurierom. Rozpatrują skargi klientów. Udzielają pomocy klientom. |

### 3.3. Środowisko użytkownika

Środowisko użytkownika:

- Cykl między 1 a 4 dni roboczych do momentu, kiedy paczka jest gotowa do odbioru zależy od trasy przesyłki oraz ilości realizowanych przesyłek na tej trasie.
- Nadanie paczki przez klienta: w domu/biurze na komputerze lub gdziekolwiek używając aplikacji mobilnej
- Przy odbiorze paczki z paczkomatu przez klienta: przy paczkomacie korzystając z aplikacji mobilnej lub wyświetlając powiadomienie e-mailowe/smsowe
- Podczas pracy kuriera: w samochodzie dostawczym na skanerze przesyłek
- Czas nadania przesyłki nie powinien przekraczać dla przeciętnego użytkownika 3 minut podczas użycia aplikacji oraz 5 przy użyciu przeglądarki.
- Działanie aplikacji w ograniczonym zakresie w trybie offline
- Aplikacje do obsługi zleceń kurierskich firm przewozowych, systemy płatności internetowej w obu przypadkach aplikacja zapewnia odpowiednie API do bezproblemowego współdziałania

### 3.4. Profile uzytkowników

#### 3.4.1. Nadawca

| | |
| --- | --- |
| Reprezentant | Nadawca|
| Opis | Aplikacja powinna być prosta w obsłudze, osoba może być w dowolny wieku, nie musi obsługować na co dzień aplikacji, mogą to być osoby starsze, nie musi posiadać większej wiedzy na temat procesu dostarczania paczek |
| Typ | Przypadkowy użytkownik |
| Rola | Opłata za nadanie paczki, nadanie w aplikacji, adresowanie przesyłki, wypełnienie danych, sprawdzenie poprawności danych, dokonanie przelewu |
| Kryteria sukcesu | Nadanie przesyłki bez większych problemów, duża dostępność paczkomatów, możliwość dojazdu kuriera, łatwe poruszanie się w aplikacji, szybkość całego procesu |
| Zaangażowanie | Umiejętnośc nadania przesyłki, wydruk etykiety, opakowanie paczki, niewielkie zaangażowanie |
| Uwagi | |

#### 3.4.2. Odbiorca

| | |
| --- | --- |
| Reprezentant | Odbiorca |
| Opis | Aplikacja powinna być prosta w obsłudze, osoba może być w dowolny wieku, nie musi obsługować na co dzień aplikacji, mogą to być osoby starsze, nie musi posiadać większej wiedzy na temat procesu dostarczania paczek |
| Typ | Przypadkowy użytkownik |
| Rola | Śledzenie przesyłki, otrzymywanie informacji na temat statusu przesyłki, odbiór z paczkomatu/ od kuriera |
| Kryteria sukcesu | Brak problemów z obsługą interfejsu, dobry kontakt z kurierem, możliwość określenia dokładnego czasu przybycia przesyłki do punktu docelowego |
| Zaangażowanie | Śledzenie przesyłki, kontakt z kurierem, zaangażowanie minimalne |
| Uwagi | |

### 3.5. Kluczowe wymagania

| Potrzeba | Priorytet | Przyczyna | Aktualne rozwiązanie | Proponowane rozwiązanie |
| --- | --- | --- | --- | --- |
| Możliwość zmiany terminu oraz miejsca odbioru przesyłki | wysoki | Zmiany planów odbiory w czasie realizacji dostawy | | |
| Śledzenie przesyłki i planowanej daty dostarczenia | wysoki | | | |
| Uproszczenie i przyspieszenie procesu nadania | średni | | | |

### 3.6. Rozwiązania alternatywne

#### 3.6.1. InPost

#### 3.6.2. DPD

#### 3.6.3. PoczteX

## 4. Omówienie produktu

### 4.1. Kontekst produktu

Niniejszy dokument wizji opisuje działanie podsystemu o nazwie Outpost firmy kurierskiej Outpost, który został opracowany przez zewnętrzną firmę informatyczną Datagility i sprzedany firmie Outpost do wyłącznego rozporządzania. Podsystem ten jest częścią większego systemu, który zajmuje się logistyką, kwestiami kadrowymi i płacowymi czy zarządza dostępem do baz danych pracowników i przesyłek a także zajmuje się ich ochroną. Zadaniem niniejszego podsystemu jest usprawnienie funkcjonowania firmy kurierskiej w zakresie obsługi przesyłek a także dodanie nowych funkcjonalności do świadczonych usług np. obsługa paczkomatów. W zakresie obsługi przesyłek produkt jest kompletny i możliwy do implementacji w innych miejscach z innymi bazami danych, jednak w założeniu powstał on wyłącznie dla firmy Outpost i dalsza jego odsprzedaż czy licencjonowanie nie jest, póki co, przewidziane . Powstał on w odpowiedzi na nieusatysfakcjonowanie społeczne istniejącymi wcześniej systemami kurierskimi, które nie gwarantowały wystarczającej elastyczności, dopasowania się do klienta a także przewidywały wysokie opłaty i mnóstwo formalności w przypadku naruszenia terminów i formy nadania czy odbioru przesyłki.

### 4.2. Podsumowanie możliwości

| Korzyści konsumenckie | Cechy produktu |
| --- | --- |
| Klient nie musi czuć się zmuszony do przebywania w zadeklarowanym z dużym wyprzedzeniem miejscu na czas odbioru przesyłki | Możliwość jednorazowej bezpłatnej zmiany adresu doręczenia przesyłki i/lub formy doręczenia (kurier/paczkomat) najpóźniej dnia poprzedzającego planowany termin doręczenia |
| Ograniczenie sformalizowanych i długotrwałych procesów zwrotów nieodebranych przesyłek | Możliwość odbioru przesyłek w magazynie przesyłkowym po przekroczeniu czasu odbioru przez 4 dni bez dodatkowych opłat|
| Klient nie ponosi kar w przypadku wystąpienia sytuacji losowych, których nie mógł przewidzieć | Jeśli paczka klienta ma status w paczkomacie -> do magazynu lub w magazynie, klient ma możliwość skontaktowania się z kurierem i wybrania innego terminu odbioru paczki z listy |
| Klient jest w stanie współplanować odbiór/nadanie przesyłki z innymi ważnymi dla niego aktywnościami w podobnym czasie | Możliwość doprecyzowania godziny przyjazdu kuriera z dokładnością +-1godzina |

### 4.3. Założenia i zależności

Projekt nie wymaga użycia bardzo nowoczesnej technologii, od której mógłby być uzależniony. Wystarczy użycie już sprawdzonych urządzeń elektronicznych i oprogramowania.
Projekt zakłada, że samo użycie nowatorskich rozwiązań, nieoferowanych przez konkurencję, przyniesie sukces biznesowy. Jeśli rynek nie zareaguje wystarczająco entuzjastycznie albo jeśli konkurencja szybko wprowadzi podobne rozwiązania, dokument wizji prawdopodobnie będzie musiał zostać wzbogacony o dodatkowe rozwiązania.

### 4.4. Koszty

- 60000zł - koszt wytworzenia podsystemu Outpost przez firmę Datagility. Podsystem Outpost nie jest sam w sobie systemem ERP (całym systemem służącym do planowania 		zasobów przedsiębiorstwa). Jest jedynie jednym z modułów tego systemu i jedynie w razie potrzeby wymiany informacji zachowuje z nim łączność. Dlatego też 		koszt takiego systemu jest względnie niski na tle kompletnych systemów ERP kosztujących w granicach 100000-200000zł
- 10000zł - instalacja systemu przez firmę zewnętrzną Datagility i jego synchronizacja z obecnym systemem ERP. Personalizacja i optymalizacja podsystemu
- 2000zł/msc - pakiet serwisowy wykupiony u firmy zewnętrznej Datagility. Obejmuje całodobową opiekę nad sprawnością działania podsystemu i priorytetowe usuwanie 			pojawiających się błędów a także gotowość do wykonywania dalszych zleceń z zakresu rozbudowy podsystemu o nowe funkcjonalności czy modyfikację obecnych
- 2000zł/msc - dodatkowy pakiet zwiększający bezpieczeństwo danych przechodzących przez system. Zawiera wzmocnioną ochronę sieci a także bardziej funkcjonalny 			menadżer haseł. W kosztach został uwzględniony wzrost wynagrodzenia dla obecnego pracownika działu cybersecurity
- 5000zł - przeszkolenie pracowników firmy przez zarząd firmy Outpost i pracowników firmy Datagility z użytkowania nowego podsystemu

### 4.5 Licencje i instalacja

Produkt został zakupiony przez firmę Outpost, która zyskała wszelkie prawa do rozporządzania nim, w tym do wydawania licencji na jego używanie przez podmioty trzecie, jak i do całkowitej odsprzedaży produktu.

Instalacja i pielęgnacja zostały zlecona firmie, która utworzyła podsystem.
	
Firma zakupiła licencje na bardziej użyteczny i rozbudowany menadżer haseł a także na oprogramowanie wzmacniające ochronę sieci.

## 5. Funkcjonalność produktu

System Outpost daje możliwość zakupu usługi oferowanej przez firmę (nadanie i przeslanie paczek lub paczki).
Ułatwia komunikacje między klientem a pracownikami firmy.

*System Outpost posiada takie funkcjonalności dla klientów firmy Outpost:*
- Nadanie Paczki – wykupienie usługi na przesłanie paczki 
- Odbiór Paczki – odebranie paczki bezpośrednio od kuriera lub z paczkomatu 
- Śledzenie Paczki	- możliwość zobaczenia statusu paczki.
- Zmiana daty odbioru paczki
- Złożenie zażalenia
- Kontakt z kurierem (w wypadku odbioru i doreczenia z/do innego miejsca niż paczkomat)

*Funkcjonalności zapewniane przez system Outpost dla pracowników firmy Outpost:*

*Dla kurierów:*
- Obszar pracy – lista adresów + adres magazynu
- Tryb pracy
- Przydzielone auto
- Możliwość zmiany statusu paczki
- Kontakt z klientem (jesli tryb pracy inny niż z/do paczkomatu)

*Dla administracji:*
- Kontakt z klientami - Dział obsługi klienta 
- Przydzielanie zadań kurierom – łatwiejsza i szybsza komunikacja

### 5.1. Zaloguj się do systemu

Klient/pracownik po wpisaniu loginu i hasła loguje się do systemu. System wyświetla interfejs klienta/pracownika.

### 5.2. Nadanie Paczki

Klient nadaje paczkę w dogodnym dla niego paczkomacie. Lub Klient przekazuje paczkę kurierowi po wcześniejszym uzgodnieniu terminu z kurierem.

### 5.3. Odbierz Paczkę

Klient odbiera paczkę w podanym wcześniej przez niego paczkomacie.
Lub Klient odbiera paczkę od kuriera po wcześniejszym uzgodnieniu terminu z kurierem.

### 5.4. Śledź Paczkę

Klient posługując się numerem ID paczki sprawdza jej status.

### 5.5. Zmień datę odbioru

Jeśli paczka klienta ma status w paczkomacie -> do magazynu lub w magazynie, klient ma możliwość skontaktowania się z kurierem i wybrania innego terminu odbioru paczki z listy.

### 5.6. Złóż zażalenie

Klient wypełnia formularz reklamacji. Formularz zostaje wysłany do pracownika administracji.

### 5.7. Zmiana Statusu Paczki

Kurier  skanuje kod paczki, informacja ta jest przesyłana do systemu. System wyświetla domyślna zmianę statusu paczki. Kurier zatwierdza status lub wybiera inny status paczki z listy. 

### 5.8. Przydziel zadania Kurierom

Pracownik administracji przydziela konkretnemu kurierowi obszar pracy, auto i tryb pracy.

### 5.9. Rozpatrz zażalenie

Pracownik administracji rozpatruje złożone wnioski. Rozpatrzony wniosek oznacza statusem “rozpatrzony”. Pracownik rozpatruje wnioski a nastepnie postepuje zgodnie z polityka firmy Outpost.

## 6. Ograniczenia 

1. Logowanie
	- Hasło musi byc ciagiem znakow o dlugosci przynajmniej 8
	- Login musi byc unikalnym ciagiem znaków
1. Formularz (Dla osob prywatnych)
	- Imie I Nazwisko nadawcy (ciag znakow)
	- Dane kontaktowe nadawcy (mail lub telefon) (ciag znakow lub 9 cyfr)
	- Adres odbiorcy (miasto, ulica, nr domu, nr mieszkania(opcjonalne),kod pocztowy)
	- dane kontaktowe odbiorcy (mail lub telefon)
1. API Dla firm
	- Sposob nadania -lista skladajaca sie z dwoch opcji(kurier,paczkomat)
	- Sposob odebrania -lista skladajaca sie z dwoch opcji(kurier,paczkomat)
	- Wystawienie faktury(opcjonalne) -pole do zaznaczenia
1. Płatność
	- Płatnosc organizowana przez system platnosci elektronicznych

## 7. Normy jakościowe

Wydajność i funkcjonalność: patrz sekcja 9.3

Odporność na błędy: Żaden użytkownik nie powinien móc zrobić niczego, co ma wpływ na funkcjonalność serwisu dla innych użytkowników.

## 8. Priorytety realizacji

1. Polepszenie istniejących procesów
   - Interfejs z istniejącym systemem logistycznym
   - Obsługa skanerów paczek dla kurierów
   - System dla klienta usług kurierskich (bez paczkomatów):
      - Tracking paczek
      - Zakup usług kurierskich
      - Uzgadnianie dostarczenia paczki
   - Pozostała funkcjonalność (drobne części funkcjonalności)
2. Nowy system paczkomatowy
   - Obsługa paczkomatów (z punktu widzenia kurierów i logistyki)
   - Odbiory z paczkomatów (dla klientów)
   - Nadawanie przesyłek z paczkomatów
   - Zwroty z paczkomatów
   - Pozostała funkcjonalność (drobne części funkcjonalności)

## 9. Pozostałe wymagania

### 9.1 Standardy

- HTTPS (HTTP/1.1, HTTP/2, TLS 1.2, TLS 1.3) - strona internetowa i aplikacja mobilna
- JSON, OpenAPI - backend strony i aplikacji, API dla biznesów
- ISO 27001, ISO 9001
- ISO 668, ISO 19160, ISO 6346
- RFC 3339, RFC 3629
- UPU S*
- PCI DSS Level 1 - system obsługi klienta
- GDPR, ePrivacy (ePD oraz ePR) - wszystkie zewnętrznie dostępne systemy
- Dodatkowe wymogi prawne

### 9.2. Wymagania systemowe

- Systemy operacyjne / Platformy:
    - Linux (Alpine) / Docker / Kubernetes (wszystkie serwery)
    - Android, iOS (aplikacja mobilna)
    - Web (HTML5, CSS3, JS) - strona internetowa
    - Android (aplikacja skanera - urządzenia przyznawane kurierom przez firmę kurierską)
- Urządzenia (minimum):
    - Serwery: Kubernetes (n.p. GKE, AWS EKS)
    - Urządzenia klientów:
        - Android API Level 24 (Android Nougat, 2016)
        - iOS 12 (2018)
        - Chrome 85+ (2020)
        - Firefox 65+ (2019)
        - Safari 16.0+ (2022)
    - Skanery: Android API Level 29

### 9.3. Wymagania wydajnościowe

- API:
    - p95 < 500ms dla API biznesowego
    - p95 < 50ms dla API do trackingu przesyłek
    - p95 < 100ms dla pozostałych funkcji API dla klientów indywidualnych (backend dla strony internetowej i aplikacji mobilnej)
- Wszystkie serwisy sieciowe:
    - 99.5% uptime minimum
    - Autoskalowanie do dowolnej liczby równoczesnych użytkowników

### 9.4. Wymagania środowiskowe

- skanery:
    - dowolna pogoda
    - dowolna pora roku
    - dowolny czas dnia
    - bateria minimum 9 godzin, pełne ładowanie podczas nocy
    - spadek z 1,5m bez uszkodzeń
- inne: nie dotyczy

## 10. Wymagana dokumentacja

### 10.1. Podręcznik użytkownika

Podręcznik użytkownika powinien być podzielony na kilka części:
1. Strona internetowa i aplikacja mobilna
2. Publiczne API (w tym biznesowe)
3. Skaner
4. Administracja i logistyka

Pierwsze dwie z tych sekcji powinne być dostępne publicznie przez internet, pozostałe są wewnętrzne dla firmy kurierskiej Outpost i dostępne tylko dla pracowników.

Pierwsza sekcja powinna być napisana w stylu samouczka dla użytkownika, podzielona na niezależne części dla poszczególnych czynności.
Druga sekcja powinna być napisana w stylu podręcznika referencyjnego, opisując wszystkie szczegóły API.
Trzecia i czwarta sekcja powinny zawierać informacje niezbędne do używania systemu przez kurierów (3) i pozostałych pracowników Outpost (4), i powinny być napisane w obu stylach, zależnie od opisanej sytuacji.
Nie ma potrzeby wydruku instrukcji użytkownika; będzie on dostępny przez internet oraz na skanerach.

### 10.2. Pomoc online

Oprócz wyżej wymienionego podręcznika, powinna być również dostępna pomoc online obejmująca dwie pierwsze sekcje podręcznika. Pomoc powinna być podzielona na krótkie (2-4 zdania) części dotyczące różnych sytuacji, w których użytkownik może potrzebować pomocy, i odwoływać się do podręcznika użytkownika w razie potrzeby większej ilości detali.

### 10.3 Instalacja i konfiguracja 

System będzie instalowany i konfigurowany przez firmę informatyczną na zlecenie Outpost, więc instrukcje instalacji, konfiguracji, i administracji oprogramowania będą dostępne wyłącznie wewnętrznie dla administratorów systemu w firmie informatycznej. Changelog będzie publikowany w dokumentacji (patrz 10.1) publicznego API bez przewidywanych zmian wstecznie niekompatybilnych.
