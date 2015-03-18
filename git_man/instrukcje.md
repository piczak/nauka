-IGMOROWANIE WYBRANYCH PLIKÓW
    stworzyć plik .gitignore w katalogu głównym projektu
    *.[qw]	- git będzie ignorował pliki kończące sie na .q i .w
    *~		- git będzie ignorował pliki kończące się tyldą
    # komentarz — ta linia jest ignorowana
    # żadnych plików .a
    *.a
    # ale uwzględniaj lib.a, pomimo ignorowania .a w linijce powyżej
    !lib.a
    # ignoruj plik TODO w katalogu głównym, ale nie podkatalog/TODO
    /TODO
    # ignoruj wszystkie pliki znajdujące się w katalogu build/
    build/
    # ignoruj doc/notatki.txt, ale nie doc/server/arch.txt
    doc/*.txt