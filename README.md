# TASK 1
## Subtask 1
8 punktów
## Subtask 3
Zdecydowałam się na udział w projekcie, by zdobyć podstawowe informacje o pracy testera manualnego. Pracując na stanowisku Product Managera, dążę do ciągłego podnoszenia kompetencji związanych z procesem działania produktów, za których działanie i rozwój odpowiadam.

Liczę na to, że po zakończeniu projektu moja wiedza na temat testowania oprogramowania będzie usystematyzowana i poszerzona o aspekty praktyczne - oczywiście w kontekście testów manualnych.

## Subtask 4
**Na czym polega ta aplikacja? Do czego służy?**
 
Aplikacja [scouts-test.futbolkolektyw.pl](https://scouts-test.futbolkolektyw.pl/pl) jest dedykowana łowcom talentów. Udostępnia informacje o graczach piłki nożnej, którzy mają założony profil. Prezentuje dane statystyczne meczów poszczególnych graczy. Użytkownicy aplikacji dodają informacje o graczach, ich udziale w meczach oraz raporty z ich gry w danym spotkaniu. Użytkownik aplikacji może poddać analizie jedynie grę pojedynczego zawodnika. Na stronie brak jest funkcjonalności pozwalających na porównywanie osiągnięć więcej niż jednego zawodnika. 

**Jakie funkcjonalności znajdują się w aplikacji? Co bym zmieniła?**

Aplikacja ma następujące funkcjonalności:
- logowanie się do systemu,
- wylogowanie się z systemu,
- wersje polską i angielską strony,
- link do kontaktu z zespołem deweloperów,
- listę graczy oraz ich mecze i raporty,
- panel do dodawania graczy z formularzem do tego celu,
- panel do dodawania meczów z formularzem do tego celu,
- panel do dodawania raportów z formularzem do tego celu.

Po kliknięciu w link do kontaktu z deweloperami użytkownik przekierowany jest do aplikacji slack i nie wie, w jaki sposób może się z nimi skontaktować.

[Formularz "Dodaj gracza"](https://scouts-test.futbolkolektyw.pl/pl/players/add) wymaga zmian:
- pola nie są odpowiednio walidowane - „Telefon” przyjmuje wszystkie znaki – cyfry, litery i znaki szczególne; „Waga” i „Wzrost” dopuszczają wartości ujemne,
- pole Waga nie ma zdefiniowanej jednostki,
- pola „Główna pozycja” i „Pozycja alternatywna” powinny umożliwiać wybranie pozycji ze zdefiniowanej listy,
- użytkownik korzystający z polskiej wersji strony przy uzupełnianiu formularza otrzymuje komunikaty po angielsku (w przypadku pól obowiązkowych),
- ujednolicenie sposobu pokazywania błędnie wypełnionych pól (wszystkich jednocześnie)
nie ma wyjaśnienia, co oznacza * przy nazwach pól w formularzu,
- dwa pola – „Łączy nas piłka” i „90 minut” – mają niezrozumiałe nazwy – użytkownik nie wie, jakiego rodzaju informacje należy tam wpisać.

Formularz "Dodawanie meczu dla gracza" ma pola, które nie precyzują, jakie informacje należy wpisać. Chodzi o "Numer" (lepiej byłoby podać "Numer na koszulce), "Web match", "General", "Recenzja". Dodatkowo pole "Recenzja" ma mocno sprecyzowane, co można w nim wpisać, można więc dać listę rozwijaną od 0 do 5 z przeskokiem o 0,5. Pole „Czas gry” nie ma zdefiniowanej jednostki.

**Interfejs aplikacji**

Uwagi ogólne: bark spójnej identyfikacji graficznej. Zakładając, że grafika „FUTBOL KOLEKTYW PLATFORMA SKAUTOWA” jest wyróżnikiem, powinna znajdować się na każdej podstronie w stałym miejscu (np. na górze strony przy nazwie „Scouts Panel”). Tymczasem teraz przypisana jest do mało znaczącego boksu dedykowanego konkatowi z zespołem deweloperów. 

Brak jest favicon'u.

Strona główna w wersji desktopowej sprawia wrażenie pustej, mało na niej informacji. Ponadto najważniejsza wartość, czyli gracze, nie jest wyeksponowana. 

Na urządzeniach mobilnych treść wyświetlana na niektórych podstronach nie skaluje się do szerkości urządzenia. Ponadto będąc w zakładkach mecze lub raporty danego gracza na niektórych urządzeniach (np. iPhone SE, iPhone XR, iPhone 12 Pro, Samsung Galaxy S8+) nie widać, dane jakiego gracza śledzimy (w tym celu trzeba rozwinąć menu).

W wielu miejscach, np. na liście graczy nie ma wyróżnika graficznego, że mogę w coś kliknąć.

**Czy aplikacja jest intuicyjna?**

%(#F​​F000​0)[Aplikacja nie jest intuicyjna]. Nie znajduje się w niej wyjaśnienie, co oznaczają pokazywanie dane - np. liczba graczy (czy chodzi o wszystkich biorących udział w rozgrywkach, jeśli tak to o jaki okres czasu chodzi?). Należy podać definicje pojęć (np. w postaci opisów wyświetlanych po najechaniu kursorem na ich nazwę).

Łowca talentów zainteresowany danym graczem – zamiast wchodzić w „Edycję gracza”, powinien widzieć kartę gracza. W aplikacji brakuje jednak takiej funkcjonalności. W karcie gracza, oprócz danych wpisanych w formularzu, widoczne byłoby zdjęcie/zdjęcia. Karta powinna być dopracowana graficznie, a podane w formularzu linki do mediów społecznościowych gracza otwierać się w nowym oknie przeglądarki. Bezpośrednio z kary powinno być możliwe przejście do meczów i raportów.

Wybierając z listy danego zawodnika wchodzi się do „Edycji gracza” - o jak wsponiałam nie jest naturlane, bo powinno się wejśc do karty gracza z informacjami o nim. Obecnie nie jest też jasne, że zakładki „Mecze” i „Raporty” dotyczą tylko tego gracza. Wystarczy graficznie pokazać, że „Mecze” i „Raporty” są zbiorem danych o wybranym graczu. 

Użytkowik, będąc na danym graczu, klikając w "Raporty" i "Dodaj raport" przenszony jest do zakładki "Mecze" bez wyjaśnienia, w jakim celu i jak dodać raport.
Będąc w tym samym miejscu i klikając w ikonę "Dodaj raport" użytkownik kierowany jest do stroni z ID gracza i ID meczu, które są ciągiem nic nie znaczących identyfikatorów.

**Co wydaje mi się błędem? Co bym zmieniła?**

Strona scouts-test.futbolkolektyw.pl powinna mieć uzupełnione podstawowe meta dane pod SEO (title, description) – przynajmniej w celu lepszej prezentacji w wynikach wyszukiwania Google.

Wyszukiwarka w zakładce „Gracze” nie wyszukuje rekordów, gdy wpisze się jednocześnie imię i nazwisko gracza.

Każdy użytkownik może wejść w edycję formularza gracza i dokonywać zmian wedle uznania. Należy dorobić możliwość nadawania różnych poziomów uprawnień. Logując się jako skaut piłki nożnej, nie powinnam mieć uprawnień do modyfikowania danych graczy, których nie jestem "właścicielem".

Po wejściu w [zakładkę „Gracze”](https://scouts-test.futbolkolektyw.pl/pl/players) użytkownik mający uprawnienia do dodawania kolejnych zawodników powinien mieć przycisk „Dodaj gracza”. Tymczasem z tego poziomu nie ma takiej możliwości.

Aplikacja nie zapamiętuje wybranej przez użytkownika konfiguracji tabel (wyboru pól) w zakładce „Gracze”.

Aplikacja nie pokazuje nazwy zalogowanego użytkownika.

Strona zawiera błędy językowe na stronie głównej:
- należy zmienić słowo "meczy" na "meczów",
- zamiast słowa "ilość"  graczy, meczów, raportów, akcji powinno być "liczba",
- nazwa bloku "Aktywnosć" zawiera błąd, poprawnie powinna ona brzmieć "Aktywność".

# TASK 2
## Subtask 1 Pisanie przypadków testowych na podstawie User Story
[Test case'y do US_1 i US_2](https://docs.google.com/spreadsheets/d/1DMfHoQPgy5omYiZJBK7BffYaP-3CouWNOZ_a_Q8A5Pc/edit?usp=sharing)

## Subtask 2 Pisanie przypadków testowych na podstawie "własnych doświadczeń"
[Test case'y na podsatwie moich doświadczeń](https://docs.google.com/spreadsheets/d/1o4-JYAPQDu3kkGRlyiqwiBTxTgPdv4nel22dMsk_7QE/edit?usp=sharing)

## Subtask 3 Po co piszemy test case’y?
**Dzięki test case'om możemy:**
- w przejrzysty i zrozumiały sposów pokazać wiele możliwości obsłużenia poszczególnych modułów systemu,
- po zakończeniu testów budować raport z ich wykonania,
- łatwo wdrożyć nowe osoby w pracę nad systemem (a przy okazji zaoszczędzić nasz czas, który musimy posięcić na "świeżaków" w zespole 	:smiley:),
- przygotować testy akceptacyjne, by potwierdzić działanie aplikacji zgodnie z wymaganiami i oczekiwaniami.

Oprogramowanie, które ma dobre pokrycie przypadkami testowymi, jest lepiej przetestowane. W takim przypadku mamy większą pewność, że sprawdziliśmy wszystkie ważne funkcjonalności.

[![A komu to potrzebne?](https://img.youtube.com/vi/OO3FANjwKHY/0.jpg)](https://www.youtube.com/watch?v=OO3FANjwKHY&t=1s)

