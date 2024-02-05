Exercici GIT 2: Ús de l'historial de canvis
=

Exercici 1
-

Mostra l'historial de canvis del repositori.

	git log

Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:

	mkdir capititols
 	cd capitols/
	echo "Git és un sistema de control de versions ideat per Linus Torvalds">capitol1.txt

Afegeix els canvis a la zona d'intercanvi temporal (staging area)

	git add capitol1.txt
  
Fes un commit dels canvis amb el missatge "Afegit capítol 1."

	git commit -m ‘’Afegit capítol 1’’
  
Torna a mostrar l'historial de canvis del repositori.

	git log

Exercici 2
-

Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:

	echo "El flux de treball basic am git Consisteix en: 1- Fer canvis al repositori. 2- Afegir els canvis a
	la zona d'intercanvi temporal. 3- Fer un commit dels canvis.">capitol2.txt

Afegeix els canvis a la zona d'intercanvi temporal.

	git add capitol2.txt

Fes un commit dels canvis amb el missatge "Afegit capítol 2."

	git commit -m "Afegit capitol 2"
  
Mostra les diferències entre l'última versió i les dues versions anteriors.

	git diff HEAD~1
	git diff HEAD~2 HEAD~1

Exercici 3
-

Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text:

	echo "Gits permet la creació de branques, la qual cosa permet tindre distintes versions del mateix
	projecte i treballar simultàniament en elles.">capitol3.txt

Afegeix els canvis a la zona d'intercanvi temporal.

	git add capitol3.txt

Fes un commit dels canvis amb el missatge "Afegit capítol 3."

	git commit -m"Afegit capitol 3"
  
Mostra les diferències entre la primera i l'última versió del repositori.

	git diff HEAD~3 HEAD

Exercici 4
-

Afegir al final del fitxer índex.txt la següent línia:

	cd..
	nano index.txt

Afegir els canvis a la zona d'intercanvi temporal.

	git add index.txt

Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex."

	git commit -m"Afegit capitol 5 a l'index"
  
Mostrar qui ha fet canvis sobre el fitxer índex.txt.

	git blame index.txt
