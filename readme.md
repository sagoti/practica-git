# PracticaGit - Respuestas



**- ¿Qué comando utilizaste en el paso 11? ¿Porqué?**
git reset --hard HEAD~1
Porque de este modo se "borra" del working copy definitivamente, mientras que con git reset HEAD~1 solo se borra del staging area


**- ¿Qué comando o comandos utilizaste en el paso 12?¿Porqué?**
git reflog 
+
git reset --hard 899b4d2

Al entrar en git reflog comprobamos el paso al que queremos volver y hacemos un git reset --hard e incluimos detrás el número correspondiente a la linea que queremos volver 



 **- El merge del paso 13,¿Causó algún conflicto?¿Porqué?**
 
 No hay conflicto, ya que ya están incluidas: Already up-to-date.
 
 
 **- El merge del paso 19, ¿Causó algún conflicto?¿Porqué?**
Sí, porque hay dos estados diferentes, el de la rama styled y el de la rama htmlify
**- El merge del paso 21, ¿Causó algún conflicto?¿Porqué?**
No, se hace un merge Fast-forward

**- ¿Qué comando o comandos utilizaste en el paso 25?**
git graph 

wifialu57-133:practica-git saragt$ git graph 
*   8992b98061909ba97648b9bb2da24e386444b7dc (HEAD -> master, styled) modifico archivo y me quedo con el contenido de la rama styled
|\  
| * e581af9435afc1b864654f838c16ea627a62b7d7 (htmlify) modifico texto en la rama htmlify ponemos cursivas
* | 899b4d2dda299acf71ec479b6bbeb30731c953d4 modifico el archivo con negritas
|/  
* 2cb7c56d768cf7e6b88dbd309b2552714c004044 añado archivo al repositorio
wifialu57-133:practica-git saragt$ 

**- El merge del paso 26, ¿Podría ser fast forward?¿Porqué?**
Sí que puede ser fast-forward porque title se ha creado desde la rama master y únicamente se han hecho avances en la rama title
**- ¿Qué comando o comandos utilizaste en el paso 27?**
git reflog 
+
git reset 

**- ¿Qué comando o comandos utilizaste en el paso 28?**

No hay cambios nuevos, por tanto no se pueden descartar. Teniendo en cuenta que se ha creado la rama title se le ha añadido el título al archivo y se ha hecho un commit, después se ha fusionado la rama master con la rama title y finalmente se ha vuelto un paso atrás deshaciendo el merge, sin embargo, a mi entender no se ha hecho ningún cambio más en el archivo y es por eso que no se pueden descartar cambios ni aplicar ningun comando. 
**- ¿Qué comando o comandos utilizaste en el paso 29?**

git branch -D title
**- ¿Qué comando o comandos utilizaste en el paso 30?**

git reflog 
+
git reset --hard 7ec41af
**- ¿Qué comando o comandos usaste en el paso 32?**
git reflog 
+
git reset --hard 2cb7c56

**- ¿Qué comando o comandos usaste en el punto 33?**


git reflog 
+
git reset --hard 7ec41af 