Komendy gita z przykladami

https://github.com/piczak/nauka.git

gitk				-graficzny git

git status			-pokazuje pliki ktróre zostały zmienione

git diff			-pokazuje zmiany z poza poczekalni

git diff --cached		-zmiany z poczekalni

git add -A  			-dodaje wszystkie pliki i rozpoczyna sledzenie ich

git commit -m "komentarz" 	-tworzy commit z komentarzem "komentarz"

git commit -a -m ""		-pomija poczekalnie dla sledzonych plików (git add jest wtedy zbedne)

git clone url			-pobiera istniejące repozytorium wraz ze wszystkimi rewizjami

git remote add origin url	-przypisanie url do wyrazu "origin"

git branch test			-tworzy gałąź o nazwie "test"

git checkout test		-przełącza się na gałąź "test"

git checkout -b test		-tworzy i przełącza się na gałąź "test"

git pull origin test:test	-pobiera ze zdlanego repozytorium zawartość gałęzi "test" i wrzuca ją do gałęzi test loklanie, jeśli lokalnie taka gałąź nie istnieje to tworzy ją

git push origin test:test	-jak powyżej z tym że w drugą stronę, lokalne repozytorium wysyla na zdalne, gdy nie ma gałęzi zdlanie, tworzy ją.

git push origin :test		-kasuje gałąź "test" na zdlanym repozytorium

git push origin +test		-wymusza wyslanie galezi "test" na zdalane repozytorium

rm nazwa.pliku
git rm nazwa.pliku		-pierwsza komenda kasuje plik, druga kasuje info z poczekalni - po commit należy wymusić używając -f

git rm --cached nazwa.pliku	kasuje plik tylko z poczekalni,sam plik zostaje w katalogu

git rm test/\*.log		-kasuje pliki z rozszerzeniem .log z katalugu "test"

git rm \*~			-kasuje wszystkie pliki konczące się tyldą

git mv README.txt README	-zmienia nazwę pliku z README.txt na README nie wywalając z poczekalni

git log				-przeglądanie historii od najnowszych zmian

git log -p -2			-pokazuje różnice wprowadzone z każdą wersiją -p, oraz ogranicza zbiór do 2 ostatnich wpisów -2

git log --stat			-skrócone statystyki

git log --pretty=oneline	-pokazuje wyniki w jednej linii
git log --pretty=short		-krótka wersja
git log --pretty=full		-zwykle
git log --pretty=fuller		-pelne
git log --pretty=format:"%h - %an "	-pokazuje informacje - w tym wypadku "skróconą sumę kontrolną - nazwiskoautora"

Opcja 	Opis
%H 	Suma kontrolna zmiany
%h 	Skrócona suma kontrolna zmiany
%T 	Suma kontrolna drzewa
%t 	Skrócona suma kontrolna drzewa
%P 	Sumy kontrolne rodziców
%p 	Skrócone sumy kontrolne rodziców
%an 	Nazwisko autora
%ae 	Adres e-mail autora
%ad 	Data autora (format respektuje opcję -date=)
%ar 	Względna data autora
%cn 	Nazwisko zatwierdzającego zmiany
%ce 	Adres e-mail zatwierdzającego zmiany
%cd 	Data zatwierdzającego zmiany
%cr 	Data zatwierdzającego zmiany, względna
%s 	Temat

git commit -m 'initial commit'			- gdychcemy poprawic rewizję, np dodac jakis plik do juz zacommitowanej rewizji
git add jakis.plik
git commit --amend


skonczone na 2.4 Podstawy Gita - Cofanie zmian
http://git-scm.com/book/pl/v1/Podstawy-Gita-Cofanie-zmian


