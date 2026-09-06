Cel to przedstawienie w jak najczytelniejszy sposób danych o tym:

lata 2016-2025

- z jakich państw przyjeżdżają do Polski turyści?
- jakie regiony Polski są najczęściej odwiedzane i jak się różnią preferencje turystów w zależności od kraju? (mamy dane do poziomu gminy)
- jak na przestrzeni lat zmieniała się liczba turystów zagranicznych i popularność Polski jako destynacji turystycznej wśród osób z różnych krajów?
- które miesiące i pory roku są najpopularniejsze wśród turystów?
- jakie obiekty noclegowe wybierają turyści zagraniczni i jak to się różni od preferencji polskich turystów?
-  ...a może wpadniesz na jeszcze inny pomysł? 🙂

Odbiorca: ogół Polaków / przeciętny „Kowalski”

Plik Geojson użyty w projekcie, wg poniższej licencji:
MIT License

Copyright (c) 2019 Piotr Patrzyk

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

To Do:
Przeczytać punkt "Synteza" z opracowania pdf z GUSu

Pułapki: 
    - te dane nie uwzględniają podróży jednodniowych - jest wymagany nocleg w bazie noclegowej
    - nie każda kwatera prywatna zgłasza do GUSu
    - obejmuje obiekty noclegowe o liczbie miejsc 10+ (95 % turystów obejmuje te noclegi 10+ miejsc)
    - 97 % odpowiada, GUS stosuje inputację (3%) - od 2016 roku
    - dane dotyczące liczby turystów może zawierać duplikaty - 1 osoba w 3 miejscach to jak 3 osoby - mamy dodatkowo liczby noclegów
    - w danych rocznych jest inny zestaw niż w danych miesięcznych

Pytania:
    - Jak zmieniała się na poziomie krajów z których przybywają turyści?
    - Jakie regiony Polski przyciągają turystów zagranicznych?
    - Liczba turystów w odniesieniu do powierzchni/ poopulacji - obciążenie
    - Jakie sezony/ miesiące wybierają turyści i czy to się różni w zależności od kraju przybycia?
    - jak różni się średnia długość pobytu w Polsce w zależności od kraju przybyia, regionu
    - Jaki jest wpływ COVID-19?
    - Jakie obiekty noclegowe wybierją turyście (hotele, pensjonaty, kempingi) 
    - Jaka częśc turystów to sąsiedzi, a inny?

    - sprawdź region w którym mieszkasz!     

To do:
    - Poprawki:   
        - mapa Azure - zrobić, żeby nie znikało jak się przeklika z turystów na noclegi
	    - Scalić Turystów i noclegi w jedną stronę
        - Usunąć tytuły osi tam gdzie niepotrzbne - opisać je w tytule wykresu
	    - Opis modelu danych
        - Opis repozytorium
       
    - Opis:
        - Dodałem metodologię
        - Poprawiłem Opisy, tytuły, usunąłem zbędne opisy osi
        - Zmieniłem CAGR na średni wzrost wg linii trendu (zostawiam dla prezentacji, choć docelowo wróciłbym do CAGR)
        - W turystach Polska vs Wlkp - zostawiłem wybór jednorotny - albo turyści albo noclegi, tytuły zmieniają się adfekwatnie,
        Dodatkowo zostawiłem kolor tylko dla Wielkopolski
        - Wpływ wojny w Ukrainie - rozszerzyłem czas żeby pokazać że Ruskie i tak spadali jeśli chodzi o liczby, dodałem punkt wybuchu wojny

    - Pytania:
        - czy na stronach turyści i noclegi zostawić slicer? osobiście nie lubię jak skaczą filtry, ale z drugiej strony są niepotrzebne
        - Czy CAGR zastąpić lepiej nachyleniem linii trendu?
        - CAGR, YoY - 1 miejsce po przecinku

    - Zrobione:
        - heat map (ze służbowego kompa)
        - wpływ wojny w Ukrainie  - rok wybuchu wojny
        - metodologia
            - Opisać YoY i CAGR 
        - Zastanowić się nad CAGR
        - Turyści zagraniczni w wlkp. vs Polskac - rozbić YoY i CAGR na dwa osobne
        - Ogólny - domyślnie zaznaczone Turyści lub noclegi
        - heat mapa - usunąć Poznań
            - mapa azuer - tytuł
            - mapa azuere - co się pojawia na mapie? Czy turyści czy noclegi? Opisać i zrobić żeby nie znikało jak się przeklika turystów
         - Wpływ Covid - po co mapa? 
        - Slicer Rok - wielkość czcionki
        - Poprawić model danych
        - KPI_Measures

    - anulowane 
        - miara: miejsce noclegowe per zagraniczny turysta
        - Jedne dane, dodaj podział na województwa
            - czy miasto powiatowe czy powiat
            - czy sąsiad Polski
            - Kontynent
        - Strony noclegi i turyści
        - Strona Polska
            - Porównanie województw - na którym miejscu jest Wlkp?

        - Współczynniki
            - Rolling CAGR 3-letni
            - Volatility
        
        - Drill-through ?

        - Porównanie z bazą noclegową?

