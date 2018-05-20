Instrukcja instalacji i uruchomienia aplikacji 


1. Pobierz i zainstaluj œrodowisko:

*node wersja 8
*npm wersja 5
*git

2. Pobierz plik .7zip który zawiera wszystkie potrzebne pliki

3. Wypakuj pliki w ³atwo dostêpnym miejscu - bêdziesz czêsto u¿ywaæ tej œcie¿ki dostêpu

4. Katalog sk³ada siê z czêœci backend oraz frontend. Otwórz teraz konsolê cmd i wejdŸ do katalogu backend. Nastêpnie wpisz w konsoli:

	npm install

5. Mo¿esz przetestowaæ czy wszystko dobrze zainstalowa³eœ wpisuj¹c w konsolê cmd

	npm run app

A nastêpnie otwórz przegl¹darkê internetow¹ i wpisz:

http://localhost:3000/call 
oraz
http://localhost:3000/status 

Jeœli podczas testu w konsoli wyrzuca b³êdy spróbuj przejœæ przez kroki jeszcze raz upewniaj¹c siê, ¿e pobra³eœ w³aœciwe wersje.

Jeœli twój test skoñczy³ sie powodzeniem przejdŸ do kroku nastêpnego.

6. Krok nastêpny to instalacja Angulara. Uruchom konsolê cmd i nie wchodz¹c w ¿aden katalog wpisz

	npm install -g @angular/cli

Nastêpnie przejdŸ do katalogu frontend i wpisz

	ng serve

Jeœli konsola nie wyrzuca b³êdów mo¿esz przejœæ do instalacji bibliotek.

- w katalogu front w konsoli wpisz:

	npm install --save socket.io-client

7. Uruchomienie aplikacji
UWAGA! 
ZnajdŸ w katalogu backend app.js i w³¹cz tryb edycji(wystarczy w notatniku np notepad++).
ZnajdŸ linijkê Dialer.configure. Odkomentuj j¹ i uzupe³nij pola login, pasword i url poni¿szymi:

login: 'focus08' 
password: 's7cksbvnvl' 
url: 'https://uni-call.fcc-online.pl'

I Otwórz konsolê cmd, wejdŸ do katalogu z projektem aplikacji - backend, a nastêpnie wpisz:

	node app.js

O poprawnym wyniku konsola poinformuje komunikatem 
'Sitecall app listening on port 3000!'

II Otwórz drug¹ konsolê cmd, wejdŸ do katalogu z projektem aplikacji - front, a nastêpnie wpisz:

	ng serve

O poprawnym wyniku konsola poinformuje komunikatem 
Complete

III Uruchom teraz przegl¹darkê internetow¹ i wpisz:

http://localhost:4200

IV Aby wykonaæ po³¹czenie wpisz numer na który ma zadzwoniæ aplikacja

V Poczekaj na po³¹czenie, o powodzeniu zostaniesz poinformowany na stronie aplikacji oraz w konsoli komunikatem: 'socket connected'
