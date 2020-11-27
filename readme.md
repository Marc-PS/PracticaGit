#Respuestas de la practica

11 - `git reset --hard HEAD~1` Utilizo el hard para que se hagan
también los cambios en mi working copy.

12 - `git reflog`Para buscar el hash del commit que hicimos
anteriormente. Después `git reset --hard ea976c2` para volver al commit
perdido con todos los cambios en el working copy.

13 - Desde styled hacemos `git merge master`No causa ningun conflicto
porque en la rama styled contenemos toda la rama master en su completo.

19 - Primero hacer `git checkout styled`. Después `git merge htmlfy`
causando un conflicto en el archivo git-nuestro.md, dado que hemos
realizado cambios en las mismas lineas en ambas ramas.

21 - No, porque al estar en un commit anterior de la misma "linea",
ha podido hacer el merge fast-forward, poniendose asi al mismo nivel.

25 - `git graph`porque lo habiamos guardado como predefinido de
`git log --graph --decorate --pretty=oneline`

26 - Si, dado que title esta en la misma "linea" que master, por tanto
master podia "subir" el commit de diferencia e igualarse con ff.

27 - `git reset HEAD~1`

28 - `git restore git-nuestro.md`

29 - `git branch -D title`

30 - Hacer reflog para ver el hash del commit que se creó con el merge,
y luego hacer `git merge b536174`desde master para hacer merge con ff.

32 - Primero un reflog para ver el hash del commit inicial, y luego
`git checkout e6943ba` para mover HEAD al commit inicial.

33 - Como dejamos la rama master alli, hacemos `git checkout master`
