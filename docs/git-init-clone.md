# Git Init y Clone

## Creando un repositorio desde cero
---

Para iniciar nuestro proyecto vamos a crear una nueva carpeta en "Documentos".
Una vez que tengamos esta carpeta creada debemos ingresar a ella por medio de la línea de comandos y usar el comando **git init** para inicializar el repositorio.

```bash
~/Documentos/$ mkdir ProyectoPtf
~/Documentos/$ cd ProyectoPtf
~/Documentos/ProyectoPtf/$ git init
Initialized empty Git repository in /home/juancuiule/Documentos/ProyectoPtf/.git/
```

Este comando crea una carpeta llamada **.git** que contiene todo lo necesario para que git pueda empezar a monitorear los cambios en el proyecto.

## Clonando un repositorio existente

Muchas veces usamos código de otros o queremos hacer modificaciones a código ajeno.
Si queres tener una copia de un repositorio existente el comando que tenemos que usar es **git clone [url]**
Por ejemplo si quisieras clonar el repositorio donde esta este tutorial podrias hacer:

```bash
~/Documentos$ git clone https://github.com/juancuiule/intro-a-git.git
Cloning into 'intro-a-git'...
remote: Counting objects: 125, done.
remote: Compressing objects: 100% (91/91), done.
remote: Total 125 (delta 69), reused 77 (delta 28), pack-reused 0
Receiving objects: 100% (125/125), 137.74 KiB | 0 bytes/s, done.
Resolving deltas: 100% (69/69), done.
Checking connectivity... done.
```

Este comando se encarga de crear una carpeta con el nombre del proyecto (**intro-a-git**) y copiar dentro de esta todos los archivos del repositorio que clonamos. Cuando clonamos el repositorio por medio de este comando no es necesario ejecutar **git init** porque el repositorio ya está inicializado.

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
    <a href="instalacion-configuracion" class="my-btn">Anterior</a>
    <a href="haciendo-cambios" class="my-btn">Siguiente</a>
</div>
