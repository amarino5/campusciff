# campusciff - Practica Ejercicio 1

##Repositorio campusciff
###Creacion del repositorio:
-<https://github.com/amarino5/campusciff>
###Clonacion del repositorio de campusciff
git clone git@github.com:amarino5/campusciff.git

##README
touch README.md

##Commit inicial
git add -A

git commit -m 'commit inicial'

##Push inicial
git push origin master

##Ignorar archivos
###Crear archivo privado.tt
touch privado.txt
###Crear directorio privado
mkdir privado
###Realizar cambios oportunos para ignorar la subida de los ficheros privados.
touch .gitignore

echo "privado" > .gitignore

echo "privado.txt" >> .gitignore

##Añadir 1.txt
touch 1.txt 

git add -A

git commit -m "Añadir los .gitignore, fichero y directorio privados, y 1.txt"

git log

##Crear tag v0.1
git tag -a "v0.1" -m "creacionde tag" 06927da9beb4ee5bb9c0daee4918798a03d40529

##Subir el tag v0.1
git push origin master

git push --v0.1 origin master

##Uso Social de GitHUB
| NOMBRE | COMPAÑERO | 
| ------ | ------: | 
| Jorge Maza    | https://github.com/jorgemaza |
| Mark Wellings | https://github.com/Mark-Wellings |
| Juan Garcia   | https://github.com/juangarciaciff |
| Anna Lawrenc  | https://github.com/annalawrenc |
| Araceli Maria | https://github.com/araceliMacia |

##Commiteo final de la practica
git add -A

git commit -m "Final de la practica 1"

##Autor
![Autor](https://avatars0.githubusercontent.com/u/7388117?v=3&s=460)


#Practica 2
##Crear una rama v0.2
git branch v0.2

git checkout v0.2

##Aañadir el fichero 2.txt en la v0.2
touch 2.txt

git add -A

git commit -m 'añadir fichero 2.txt en la rama v0.2'
##Crear una rama remota
git push origin v0.2

##Merge directo 
###Posicionarse en la rama master
git checkout master

###Hacer un merge de la rama v0.2 con la rama master
git merge origin v0.2

##Merge con conflicto
###En la rama master añadir Hola en el fichero 1.txt
echo "Hola" >> 1.txt
git add -A
git commit -m "Añadir hola en el fichero 1.txt"

###Posicionarse en la rama v0.2, añadir "Adios" en el fichero 1.txt y hacer commit
git checkout v0.2
echo "Adios" >> 1.txt
git add -A
git commit -m "Añadido Adios al fichero 1.txt"

###Posicionarse de nuevo en la rama master y hacer un merge con la rama v0.2
git checkout master
git merge master v0.2

##Listado de ramas
git branch -v 

~~~javascript
sboxes@osboxes:~/PycharmProjects/campusciff$ git branch -v
* master b61bd63 [ahead 5] Añadir hola en el fichero 1.txt
  v0.2   b2f06b6 Añadir ADIOS  en el fichero 1.txt
~~~

##Arreglar conflicto



