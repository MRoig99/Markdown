Exercici 1
-

Crea una nova branca bibliografia i mostrar les branques del repositori.
	
        git branch bibliografia
        git branch

Exercici 2
-
1. Crear el fitxer capítols/capitol4.txt i afegir el següent text
   
        cd capitols/
        echo "En aquest capítol veurem com utilitzar GitHub per allotjar repositoris en
        remot">capitol4.txt

2. Afegir els canvis a la zona d'intercanvi temporal.
   
        git add capitol4.txt

3. Fer un commit amb el missatge "Afegit capítol 4."
   
        git commit -m ‘’Afegit capítol 4’’

5. Mostrar la història del repositori incloent totes les branques.
   
        git log –all

Exercici 3
-
1. Canvia a la branca bibliografia.
   
        git checkout bibliografia

2.  Crea el fitxer bibliografia.txt i afegir la següent referència:
   
        echo "Chacon, S. and Straub, B. Pro Git. Apress">bibliografia.txt

3. Afegeix els canvis a la zona d'intercanvi temporal.
   
        git add bibliografia.txt

4. Fes un commit amb el missatge "Afegida primera referència bibliogràfica."
   
        git commit -m "Afegit primera referencia bibliografica"

5. Mostra la història del repositori incloent totes les branques.
   
        git log –all

Exercici 4
-
1. Fusiona la branca bibliografia amb la branca master.
   
        git checkout master
        git merge bibliografia

2. Mostra la història del repositori incloent totes les branques.
   
        git log --all

3. Elimina la branca bibliografia.
   
        git branch -d bibliografia

4. Mostra de nou la història del repositori incloent totes les branques.
   
        git log

Exercici 5
-
1. Crea la branca bibliografia.

        git branch bibliografia

3. Canvia a la branca bibliografia.
   
        git checkout bibliografia

5. Canvia el fitxer bibliografia.txt perquè continga les següents referències:
   
        nano bibliografia.txt

7. Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge
"Afegida nova referència bibliogràfica."

        git add bibliografia.txt
        git commit -m"Afegida nova referencia bibliogràfica"

9. Canvia a la branca master.
    
        git checkout master

11. Canvia el fitxer bibliografia.txt perquè continga les següents referències:
    
        nano bibliografia.txt

13. Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge
"Afegida nova referència bibliogràfica."

        git add bibliografia.txt
        git commit -m"Afegida nova referencia bibliogràfica"

15. Fusiona la branca bibliografia amb la branca master.
    
        git checkout master
        git merge bibliografia

17. Resol el conflicte deixant el fitxer bibliografia.txt amb les referències:
    
        nano bibliografia.txt

10.Afegeix els canvis a la zona d'intercanvi temporal i fes un commit amb el missatge
"Resolt conflicte de bibliografia."

        git add .
        git commit -m ‘’Resol conflicte de bibliografia’’
 
11.Mostra la història del repositori incloent totes les branques.

        git log
