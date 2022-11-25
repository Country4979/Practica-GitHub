# Practica-GitHub
Prácticas del módulo de Git

*PREGUNTA 01: ¿Qué comando utilizaste en el paso 11? ¿Por qué?*

He empleado el comando "reset --hard HEAD~1". Al utilizar "--hard" estamos obligando a que el sistema modifique el working copy (si no utilizamos el commando "--hard" no lo hará). Si abrimos el archivo git-nuestro.md, vemos que las modificaciones que le hicimos ya no están.


*PREGUNTA 02: ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?*

He utilizado el comando "git reflog" para localizar el indicador del commit que me interesa. Una vez localizado, uso "git reset --hard <indicador>" (sin  <>) para "recuperar" el commit. Compruebo que es el que quiero con un "git log" y compruebo con "cat git-nuestro.md" que se han recuperado los cambios. Utilizo "gitcommit -m 'Rehago el commit"'.

  
*PREGUNTA 03: El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?*

No, ninguno. Al ser el commit de la rama main el commit padre del commit en el que nos encontramos de la rama styled, las diferencias del archivo git-nuestro.md las considera una actualización del mismo, no un conflicto como tal.

  
*PREGUNTA 04: El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?*

Efectivamente, se ha producido un conflicto porque ambas ramas (styled y hmlify) poseen el mismo archivo git-nuestro.md con diferencias en las mismas líneas, por lo que Git nos lanzará un conflicto. Además, ninguna es padre de la otra como ocurría en el caso anterior.

  
*PREGUNTA 05: El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?*

No ha habido conflictos.Al estar el archivo git-nuestro.md de la rama main desactualizado con respecto a al de la rama styled, lo actualiza.

  
*PREGUNTA 06: ¿Qué comando o comandos utilizaste en el paso 25?*

Utilicé el comando "git log --graph". Aunque es verdad que con virtual studio Code se e mejor el diagrama.

  
*PREGUNTA 07: El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?*
Sí, porque cuando haga el merge, el HEAD sigue teniendo acceso a toda la linea de commits de la rama main.

  
*PREGUNTA 08: ¿Qué comando o comandos utilizaste en el paso 27?*

Utilicé un "git reglog" para buscar el hash del commit anterior al merge que necesitaba. Luego un "git reset <hash>" (sin comillas) para

  
*PREGUNTA 09: ¿Qué comando o comandos utilizaste en el paso 28?*

He empleado el comando "git restore git-nuestro.md".

  
*PREGUNTA 10: ¿Qué comando o comandos utilizaste en el paso 29?*

He usado el comando "git branch -D title".

  
*PREGUNTA 11: ¿Qué comando o comandos utilizaste en el paso 30?*

He hecho un "git reflog", he buscado el hash del merge, lo he copiado y luego he emplado el comando "git reset <hash copiado>" (sin <>).


*PREGUNTA 12: ¿Qué comando o comandos usaste en el paso 32?*

Un "git log" para ver cuál es el SHA del Initial commit, copiar dicha referencia y hacer un "git reset <referencia>" (sin <>). No he hecho un --hard porque no se especifica que modifique el working copy.


*PREGUNTA 13: ¿Qué comando o comandos usaste en el punto 33?*

Tras un "git reflog" para localizar el hash del merge donde hicimos el último paso, hago un "git reset <hash>" (sin <>) para volver a ese punto. Una vez aquí, un "cat git-nuestro.md" para ver el contenido del archivo. "git restore git-nuestro.md" para volver a su versión anterior, con el título.

