# Merge
---

En la sección anterior vimos cómo crear ramas para trabajar de una manera mas ordenada en nuestros proyectos, pero todavía no sabemos como incorporar los cambios hechos en esta rama a nuestro **master** para que forme parte de una nueva versión de nuestro programa. Para hacer esto usamos el comando **git merge**

Antes que nada debemos situarnos en la rama a la cual queremos traer estos cambios, en nuestro caso **master**

```bash
~/Documentos/ProyectoPtf/$ git checkout master
Switched to branch 'master'
```

Una vez que ya estamos en este branch usamos el comando **git merge** de la siguiente manera

```bash
~/Documentos/ProyectoPtf/$ git merge nueva-funcionalidad
Updating 6113d10..2091931
Fast-forward
 docs/branches.md | 17 +++++++++++++++--
 docs/index.md    |  1 +
 docs/merge.md    | 48 ++++++++++++++++++++++++++++++++++++++++++++++++
 3 files changed, 64 insertions(+), 2 deletions(-)
 create mode 100644 docs/merge.md
```

De esta manera todos los commits que hicimos en el branch nueva-funcionalidad se replican en el branch master.

Es posible que al momento de hacer un merge surjan conflictos por cambios que se hayan hecho en la rama principal despues de que hayamos creado nuestra rama "nueva-funcionalidad".

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
    <a href="branches" class="my-btn">Anterior</a>
    <a href="problemas-al-hacer-merge" class="my-btn">Siguiente</a>
</div>
