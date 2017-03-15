# Branches - Ramas
---

Cuando hablamos de ramas o branches, hacemos referencia a una funcionalidad de git que nos permite dejar de trabajar en una única rama **master** para poder desarrollar sin comprometer el funcionamiento del programa en la rama principal. Esto nos permite manejar de una mejor manera el trabajo que hacemos para nuevas funcionalidades que desarrollemos o soluciones de errores particulares.

Por ejemplo si estamos trabajando en un aplicación web y tenemos una versión estable y que funciona de manera esperada en la rama principal **master** y queremos desarrollar una funcionalidad nueva podriamos armar un branch nuevo para trabajar en ella sin poner en peligro el funcionamiento de la aplicación.

> Antes de que creemos el branch nuestro repositorio se encuentra en un estado similar al siguiente

![Estado inicial](media/antes-del-nuevo-branch.png)

> Ahora usamos el siguiente comando para crear un nuevo branch y "movernos" hacia este branch para trabajar en él

```bash
~/Documentos/ProyectoPtf/$ git checkout -b nueva-funcionalidad
Switched to a new branch 'nueva-funcionalidad'
```

> Luego de crear el branch el estado de nuestro repositorio pasa a ser este

![Branch creado](media/creado-el-branch.png)

Luego de hacer algunos cambios hacemos el proceso que ya aprendimos para hacer un commit

```bash
~/Documentos/ProyectoPtf/$ git commit -m "primer commit en nueva funcionalidad"
[nueva-funcionalidad e5a6a0f] primer commit en nueva funcionalidad
 1 file changed, 10 insertions(+), 1 deletion(-)
```

![Branch despues del commit](media/despues-del-commit-en-branch.png)

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
    <a href="repositorio-remoto-2" class="my-btn">Anterior</a>
    <a href="merge" class="my-btn">Siguiente</a>
</div>
