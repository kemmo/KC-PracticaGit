# Preguntas ejercicio 1


### 1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?

~~~~
git reset --hard HEAD~1
~~~~

Para retroceder al nodo anterior movemos el puntero *HEAD* una posición con el *~1* y con la opción *--hard* dejamos limpio el working copy

### 2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

~~~~
git reflog
git reset --hard HEAD@{1}
~~~~

Primero utilizo reflog para obtener el histórico de los pasos que hemos hecho en nuestro repositorio.
Entonces localizo el que quiero rehacer, que está a un paso de donde estoy ahora *HEAD@{1}*, y lo referencio mediante su posición en el reflog.

### 3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No. Porque la rama *master* ya está contenida en *styled*, por lo que no hay nada que mergear.

### 4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si. Porque hemos intentado mergear dos ramas, *styled* y *htmlify*, en la que se han modificado las mismas lineas del mismo fichero.

#### 5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No. Porque los nodos de *master* y *styled* forman una "linea", es decir no modificamos las mismas lineas del mismo fichero en diferentes ramas y por ello se puede realizar un merge fast-forward.

#### 6. ¿Qué comando o comandos utilizaste en el paso 25?

~~~
git log —graph
~~~~

#### 7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Si, podría ser fast-forward ya que los nodos de ambas ramas forman una "linea" y se podría haber colocado el puntero diréctamente en la rama *title* sin necesidad de crear un nuevo commit.

#### 8. ¿Qué comando o comandos utilizaste en el paso 27?

~~~~
git reset HEAD~1
~~~~

#### 9. ¿Qué comando o comandos utilizaste en el paso 28?

~~~~
git reset --hard
~~~~

#### 10. ¿Qué comando o comandos utilizaste en el paso 29?

~~~~
git branch -D title
~~~~

#### 11. ¿Qué comando o comandos utilizaste en el paso 30?

~~~~
git reflog
git reset --hard HEAD@{2}
~~~~

#### 12. ¿Qué comando o comandos usaste en el paso 32?

~~~~
git checkout 100f57a
~~~~

#### 13. ¿Qué comando o comandos usaste en el punto 33?

~~~~
git checkout master
~~~~
