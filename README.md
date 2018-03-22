# Projekt 3
## Budowa systemu typu CRM z wykorzystaniem AngularJS


### 1. Cel projektu

Celem projektu jest stworzenie warstwy klienckiej aplikacji webowej będącej systemem `CRM`.

### 2. Opis technologii

Projekt polega na napisaniu aplikacji typu `SPA` komunikującego się z zewnętrznym `RESTful API` za pomocą protokołu `HTTP`.
Projekt powinien zostać napisany w języku JavaScript z użyciem frameworka `AngularJS` oraz biblioteki `AngularJS Material`.


### 4. Wymagania projektowe

#### Struktura danych

System `CRM` powinien przechowywać następujące informacje o klientach w postaci obiektów `JavaScript` serializowanych do formatu `JSON` o podanych nazwach:
  - `id` - Identyfikator klienta
  - `name` - Imię i nazwisko
  - `company` - Firma
  - `email` - Adres e-mail
  - `phone` - Numer telefonu
  - `date` - Data rejestracji


#### Komunikacja z RESTful API

Aplikacja powinna implementować podstawowe metody `CRUD` do zarządzania klientami według poniższej tabeli:

| Opis                                                                | Metoda HTTP  | Adres URL       |
|---------------------------------------------------------------------|:-------------|:----------------|
| Dodawanie klienta do bazy aplikacji                                 | `POST`       | `/add`          |
| Pobranie listy klientów                                             | `GET`        | `/customers`    |
| Pobranie informacji szczegółowych klienta o danym identyfikatorze   | `GET`        | `/customer/:id` |
| Aktualizacja danych klienta                                         | `PUT`        | `/update/:id`   |
| Kasowanie informacji o kliencie                                     | `DELETE`     | `/delete/:id`   |

Do komunikacji z `REST API` aplikacja powinna wykorzystywać prezentowane na zajęciach `Fetch API` bądź serwis `$http` z frameworku AngularJS.

Należy pamiętać o odpowiednich nagłówkach podczas wysyłania zapytań do API:
- `Content-Type: application/json`
- `Access-Control-Allow-Origin: *`


#### Struktura aplikacji

Użytkownik aplikacji powinien mieć możliwość przeglądania oraz zarządzania danymi osobowymi na podstronach:

- `/customers/list` – Lista wszystkich klientów zawierająca podstawowe informacje
- `/customers/add` – Formularz tworzenia nowego wpisu klienta
- `/customers/edit/:id` – Formularz edycji danych klienta
- `/customers/details/:id` – Profil klienta zawierający wszystkie dostępne informacje


#### Wygląd aplikacji

Aplikacja powinna wykorzystywać bibliotekę `AngularJS Material` oraz przynajmniej kilka dostępnych w niej komponentów, takich jak:
- `mdButton`
- `mdCard`
- `mdIcon`
- `mdInput`
- `mdList`
- `mdToolbar`
- `mdTooltip`

Aplikacja powinna mieć zaaplikowany dowolny, nie-domyślny motyw kolorystyczny.


#### Środowisko programistyczne

Aplikacja może być zaimplementowana w dowolnym środowisku programistycznym z dowolną strukturą plików, np.
- jako pojedynczy plik `HTML` z osadzonym skryptem `JavaScript` implementujacym funkcjonalności
- jako projekt w `ES6` z podziałem na pliki, na podstawie dostępnego na portalu `GitHub` startera
- jako projekt z użyciem platformy [StackBlitz](https://stackblitz.com/edit/angularjs-gcjape)


### 5. Praca w grupach

Projekt może być realizowany samodzielnie, bądź w maksymalnie 4 osobowych grupach.


### 6. Zasady zaliczenia projektu

Zaliczenie projektu odbędzie się na podstawie przekazanych plików źródłowych w określonym terminie.


### 7. Linki zewnętrzne

- https://docs.angularjs.org/api – dokumentacja frameworka `AngularJS`
- https://material.angularjs.org/latest/ – dokumentacja biblioteki `AngularJS Material`
- https://pl.wikipedia.org/wiki/Hypertext_Transfer_Protocol – opis metod `HTTP`
- https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API - dokumentacja `Fetch API`
- https://docs.angularjs.org/api/ng/service/$http - dokumentacja serwisu `$http`
- https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS - opis nagłówków protokołu `HTTP` odpowiadających za `CORS`

