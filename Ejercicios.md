1. Tienes que modificar la escena 5 de Hamlet en el fichero scene-5.txt. En dicha escena Hamlet encuentra al fantasma de su padre. Añade este texto al fichero:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting flames
> Must render up myself.

--Primero inicializamos git y nos traemos el repositorio con git clone https://github.com/IESJacaranda/deshaciendo-cambios-y-gestion-de-ramas-SVRoman25.git una ves que tenemos el repositorio en nuestro ordenador accedemos al archivo con nano scene-5.txt y añadimos la modificacion

2. Añade scene-5.txt al área de preparación.

--Lo añadimos con git add scene-5.txt

3. Haz un commit con los cambios con un buen mensaje de commit.

--hacemos commit git commit -m 'un buen mensaje de commit'

4. Modifica las palabras del fantasma. Aquí tienes una sugerencia divertida:
> Ghost: 
> My hour is almost come,
> When I to sulphurous and tormenting balloons
> Must render up myself.

 --con nano scene-5.txt añadimos la frase 

5. Devuelve el fichero al estado del último commit.
 
 --con git reset --hard
 
6. Cambia el nombre de LARRY por LAERTES en los ficheros scene-3.txt y scene-7.txt.
 
 --nano scene-5.txt y nano scene-7.txt y hacemos las modificaciones
 
7. Añade los ficheros al área de preparación usando un único comando git.
 
 --it add scene-3.txt scene-7.txt

8. Vamos a cometer un error a propósito. Borra cualquier línea del fichero scene-2.txt.
  
  --no scene-2.txt y borramos la linea
 
9. Añade scene-2.txt al área de preparación.
 
 --it add scene-2.txt

10. Comprueba el estado del repositorio.

  --t status 
  
11. Devuelve scene-2.txt al directorio de trabajo.

 --git reset HEAD scene-2.txt

12. Haz un commit para guardar los cambios realizados en el nombre de Larry por Laertes.
 
 --git commit -m 'cambio larry por laertes'

13. Busca el primer commit que has hecho y vuelve a dicho commit. Indica como has buscado el commit anterior y como has vuelto a él.
  
  --Buscamos el commit con git log pero no se puede deshacer el commit 

14. Crea una nueva rama llamada **reinventando_hamlet**

--git branch reinventando_hamlet  

15. Cámbiate a dicha rama
 
 --git checkout reinventando_hamlet
  
16. Mejora la escena 2 como creas conveniente.
 
 --nano scene-2.txt

17. Haz un commit con los cambios con un mensaje adecuado.

--git commitscene-2.txt  -m 'mensaje adecuado'

18. Vuelve a la rama master.
 
 --git checkout master

19. Elimina la rama **reinventando_halet**
  

20. Crea una nueva rama, modifica algo en la rama master, haz commit y llévate los cambios a la rama que has creado.
21. Provoca un conflicto entre la rama master y la rama que has creado (indica lo que has hecho). Une la rama a la rama master resolviendo el conflicto.
