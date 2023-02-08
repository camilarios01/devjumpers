Git-Github : Ejercitación Final

```Repositorio Devjumpers - Paso a paso```


Desde la página Github cree un repositorio con el nombre “Devjumpers”

En mi Pc cree una carpeta llamada git-github donde utilizando la aplicación "git bash here" clone mi repositorio en la carpeta utilizando el comando “Git clone + el link de mi repositorio”

Para poder pasar de la carpeta git-github a mi Repositorio Utilice el comando “cd devjumpers”


``` README```


Ya dentro de la carpeta devjumpers (mi repositorio) cree el archivo Readme.dm utilizando el comando “touch + Readme.dm”

Para saber si se había creado con éxito utilice el comando “ ls “

Una vez verificado que se creó con éxito el archivo realice un “ git add . “ el cual prepara mi archivo para poder subirlo a la nube,
seguido de ese comando hice “ git status “ para asegurarme que ya estaba listo


```Commit Inicial + Push inicial```


Utilizando el código “ git commit -m “ realice el commit, Para subir todo a la nube realice un “ git push “ . 
Finalizé verificando desde la web si se había actualizado mi repositorio

```Ignorar Archivos```

Desde la aplicacion Visual Studio Code abri mi repositorio, cree un Archivo llamado Privado.txt y una carpeta llamada privada
 
Realice un " git status " para verificar que se crearon con exito

Despues de eso cree el archivo que me va ayudar a que git ignore las carpetas mensocionadas enteriormente que es .gitignore
dentro de ese arhivo escribi los comando que quiero que git ignore que fueron /privada y /privado.txt

realice nuevamente un " git status " para estar segura que git esta ignorando el archivo txt y la carpeta.

 ```Añadir fichero```
 
  Realizo " touch 1.txt " en el main y creo un archivo  
  
  ```Crear una rama v0.2 y subir cambios al dispositivo remoto```
   
   Para crear una  nueva rama realice un " git branch v0.2 "
   
   Con el comando " git checkout v0.2 " me direccione a la rama 
   
   Dentro de la rama cree un archivo llamado 2.txt con el comando " touch 2.txt "
   
   Realice un " git add . " seguido de eso realice un "git commit -m" donde dice  que cree de dos arcivos de txt uno en rama v0.2 y otro en main
   
   realice un git push y me salto un Erro el cual lo solucione poniendo lo que decia que fue 
  
  git push --set-upstream origin v0.2

    ```Merge directo```
    
  Me redirecciono a el main con el comando " git checkout main " dentro de el realizo un merge 
  pero a la rama v0.2 con el comando "git merge v0.2"


   ```Merge con conflicto```

 Desde la rama Main realizo un cambio en el archivo 1.txt colocandole hola con el comando " echo "hola" >1.txt "
 genero un " git add . " y seguido de eso realizo un commit con el comando " git commit -m "modificacion en el archivo 1.txt" "
 
 Me posiciono en la rama v0.2 realizando " git checkout v0.2 " y desde ahi edito el archivo 1.txt con el codigo " echo "adios" >1.txt "
como hice con anterioridad realizo un " git add . " y un commit con  " git commit -m "modificacion en el archivo 1.txt desde la rama v0.2" "

vuelvo al Main con el comando " git checkout main "y realizo un merge a la rama v2.0 con el comando " git merge v0.2 "
(me salta que hay un conflicto)

 lista de ramas:
 

con merge git branch --merged


sin merge git branch --no-merged

``` Solucion del conflicto anterior ```

realizo un " git add . " y utilizo un " git commit -m "conficto solucionado" " para informar que solucione el problema 

utilizando " git branch -d v0.2 " borro la rama v0.2

para finalizar genero un " git push " para actualizar mi repositorio en la nube.

 ```Listado de cambios```
 utilice: git log --oneline --decorate --all --graph
 
 *   11d503c (HEAD -> main, origin/main) conficto solucionado
|\
| * bf8a88c modificacion en el archivo 1.txt desde la rama v0.2
* | 0c47b4f modificacion en el archivo 1.txt
|/
* fd124e4 (origin/v0.2)  creacion de dos arcivos de txt uno en rama v0.2 y otro en main
* 8bcda55 commit inicial

 NOMBRE          /            GITHUB
 
 Damian Coronel             https://github.com/Damsh-bit

Armando Torres Quintana     https://github.com/ArmaTQ 
 
 Ivan de la parte           https://github.com/ivandelaparte
 
 camila calegari            https://github.com/camilacalegari
 
  ```COLABORADOR```
 Lucas Emmanuel Gimenez
 
