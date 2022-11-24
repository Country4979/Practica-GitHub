# Practica-GitHub
Prácticas del módulo de Git
PREGUNTA 01: ¿Qué comando utilizaste en el paso 11? ¿Por qué?

He empleado el comando "reset --hard HEAD~1". Al utilizar "--hard" estamos obligando a que el sistema modifique el working copy (si no utilizamos el commando "--hard" no lo hará). Si abrimos el archivo git-nuestro.md, vemos que las modificaciones que le hicimos ya no están.

PREGUNTA 02: ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

He utilizado el comando "git reflog" para localizar el indicador del commit que me interesa. Una vez localizado, uso "git reset --hard <indicador>" (sin  <>) para "recuperar" el commit. Compruebo que es el que quiero con un "git log" y compruebo con "cat git-nuestro.md" que se han recuperado los cambios.
  
PREGUNTA 03: El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

PREGUNTA 04: El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

PREGUNTA 05: El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

PREGUNTA 06: ¿Qué comando o comandos utilizaste en el paso 25?

PREGUNTA 07: El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

PREGUNTA 08: ¿Qué comando o comandos utilizaste en el paso 27?

PREGUNTA 09: ¿Qué comando o comandos utilizaste en el paso 28?

PREGUNTA 10: ¿Qué comando o comandos utilizaste en el paso 29?

PREGUNTA 11: ¿Qué comando o comandos utilizaste en el paso 30?

PREGUNTA 12: ¿Qué comando o comandos usaste en el paso 32?

PREGUNTA 13: ¿Qué comando o comandos usaste en el punto 33?
