# Problemas al hacer un merge
---

En la sección anterior vimos cómo "mergear" nuestros cambios de un branch a otro...
Pero no siempre los merges van a ser tan simples, al trabajar en equipo puede suceder que dos personas hayan modificado un mismo archivo haciendo que la unión de las dos versiones sea imposible de solucionar automaticamente para git.

Esto puede suceder cuando un determinado archivo sufre cambios distintos hechos desde dos branches distintos.
Para probar esto cree un nuevo branch desde el master y lo llame 'nueva-funcionalidad'. Después (desde ese branch) hice algunos cambios en el archivo, los agregue a la zona de stage (add) e hice un commit. Luego volví al branch master (git checkout master) e hice cambios en el mismo archivo, los agregue a la zona de stage y también hice un commit generando conflictos entre estas dos versiones que se encuentran en dos branches distinos.

```bash
~/Documentos/ProyectoPtf/$ git merge nueva-funcionalidad
Auto-merging archivoEjemplo.txt
CONFLICT (content): Merge conflict in archivoEjemplo.txt
Automatic merge failed; fix conflicts and then commit the result.
```
Como vemos en el mensaje de arriba git no pudo hacer el merge de manera automatica debido a conflictos en el archivo en cuestión.
Para esto nos pide que solucionemos ese o esos conflictos y volvamos a hacer un commit.

Ahora si miramos el archivo en cuestión vamos a encontrarnos con esto.

```
Hello World!
<<<<<<< HEAD
Editando segunda linea del archivo desde branch 'master'
=======
Hola Mundo desde el branch 'nueva-funcionalidad'
>>>>>>> nueva-funcionalidad
```

Git nos esta indicando cuales son los cambios que provienen de cada branch, permitiendonos saber que es lo que sucedio y dandonos la posibilidad de corregir los cambios.

Una vez que hayamos corregido los conflictos no queda mas que hacer un nuevo commit.

```
Hello World!
Editando segunda linea del archivo desde branch 'master'
Hola Mundo desde el branch 'nueva-funcionalidad'
```

En este caso solo voy a borrar los comentarios hechos por git y voy a hacer un nuevo commit.

```bash
~/Documentos/ProyectoPtf/$ git add archivoEjemplo.txt
~/Documentos/ProyectoPtf/$ git commit -m "fix conflicto de merge"
```

---

<br>
<style>
.my-btn {
    height: 50px;
    width: 120px;
    display: inline;
    text-align: center;
    color: rgba(255, 255, 255, 0.6);
    background-color: #159957;
    background-image: linear-gradient(120deg, #155799, #159957);
    transition: color 0.2s ease-in-out;
    border-radius: 0.3rem;
    padding: 12px;
}

.my-btn:hover {
    color: #FFFFFF;
}

.Grid {
    display:flex;
    justify-content: space-around;
}
</style>
<div class="Grid">
    <a href="merge" class="my-btn">Anterior</a>
    <a href="problemas-al-hacer-merge" class="my-btn">Siguiente</a>
</div>
