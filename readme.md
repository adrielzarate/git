# Práctica del curso de git, gitHub y Sourcetree

## Ejercicio 1

* ¿Qué comando utilizaste en el paso 11? ¿Por qué?

Utilicé el comando *git reset --hard HEAD~1*, porque *git reset HEAD~1* vuelve un commit hacia atrás, y con el modificador *--hard* elimino los cambios del working copy

* ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Utilicé el comando *git reflog* y *git reset --hard < commit_id >* , porque con *reflog* puedo ver todos los commits de nuestro repo, y con *git reset --hard* reseteamos el branch al punto que le indiquemos. Agregando el identificador del commit especificado, lo haremos hasta ese punto.

* El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No causó conflicto porque el cambio que hicimos lo deshacimos y ese era el primer cambio después de hacer el branch desde master, es decir, lo dejamos igual a como estaba de master y no tuvo conflictos.

* El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

El merge causó conflico porque el archivo git-nuestro.mg de la rama styled no tiene el mismo contenido que el de la rama htmlify que quiso absorver.

* El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

El merge no causó ningún conflicto porque elegimos el contenido de la rama styled, que ya habíamos dejado igual que cuando fue creada a partir de la rama master

* ¿Qué comando o comandos utilizaste en el paso 25?

Para dibujar el diagrama utilicé el comando *git log --graph*

* El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Sí, podría haberlo hecho fast foward porque la rama title la cree directamente de master y cuando volví a unirla a master, master no tenía ningún cambio, por lo que la unión se podría haber hecho directamente sobre lo hecho en la rama title


* ¿Qué comando o comandos utilizaste en el paso 27?

Utilicé el comando *git reset HEAD~1*

* ¿Qué comando o comandos utilizaste en el paso 28?
Utilicé el comando *git checkout -- git-nuestro.md*

* ¿Qué comando o comandos utilizaste en el paso 29?

Utilicé el comando *git branch -D title*

* ¿Qué comando o comandos utilizaste en el paso 30?

Utilicé el comando *git reflog* para encontrar el merge y git checkout para dirigirme hacia él a través de su código de identificacion. Luego con *git checkout -d title* cree la rama title nuevamente. Volí a master con *git checkout master* y rehice el merge con title.

* ¿Qué comando o comandos usaste en el paso 32?

Utilicé el comando *git reflog* para obtener el id del primer commit y luego *git reset --hard < id_commit >*

* ¿Qué comando o comandos usaste en el punto 33?

Utilicé el comando *git reflog* para obtener el id del ultimo commit y luego *git reset --hard < id_commit >*
