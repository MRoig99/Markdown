Exercici GIT 1: Creació i actualització de repositoris
#

Exercici 1
-

Crea un repositori nou amb el nom llibre i mostra el seu contingut.

	mkdir llibre
	cd llibre/
	git init
	ls -la
 
Configura Git definint el nom de l'usuari, el correu electrònic i activa l'exida en color. Mostra la configuració final.

	git config --global user.name"Miguel Angel"
	git config --gloval user.email "miguelangel@gmail.com
	git config --global color.ui auto
	git config --list
	
Exercici 2
-

Comprova l'estat del repositori.

	git status
 
Crea un fitxer índex.txt amb el següent contingut:

	echo "Capitol 1:Introduccio a Git">index.txt
	echo "Capitol 2:Flux de treball basic">>index.txt
	echo "Capitol 3:Repositoris remots">>index.txt
 
Comprova de nou l'estat del repositori.

	git status
 
Afegeix el fitxer a la zona d'intercanvi temporal.

	git add index.txt
 
Torna a comprovar una vegada més l'estat del repositori.

	git status

Exercici 3 
-
Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i revisa l'estat del repositori.

	git commit -m"Afegit index del llibre"

Exercici 4
-
Canvia el fitxer índex.txt perquè continga el següent:

	nano index.txt

Mostra els canvis respecte a l'última versió guardada al repositori.

	git status
 
Fes un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de branques".

	git commit -m"Afegit capitol 3 sobre gestio de branques"

Exercici 5
-
Mostra els canvis de l'última versió del repositori respecte a l'anterior.

	git diff
 
Canvia el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques a l'índex."

	git commit --amend -m"Afegit capitol 3 sobre gestio de branques a l'index"
 
Torna a mostrar els últims canvis del repositori.

	git diff

Exercici 6
-

Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).

	touch .gitignore
	nano .gitignore
