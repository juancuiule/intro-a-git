# Git - Repositorios Remotos

En esta sección vamos a seguir viendo un poco mas sobre repositorios remotos. Como dijimos anteriormente la mayoría de las veces que desarrollamos software lo hacemos en equipo con lo cual es muy importante mantener un orden que nos permita evitar o minimizar conflitos entre los integrantes de este grupo. Varias personas pueden trabajar en un mismo repositorio y para evitar conflictos es muy importante la comunicación entre nosotros que nos va a permitir estar atentos a cuando otro haga un cambio y saber como puede esto afectar el código que tenemos de manera local en nuestras maquinas.

Cuando otra persona "pushea" commits al repositorio remoto tenemos que traer esos cambios a nuestro repositorio local para no terminar trabajando sobre lo mismo y pisando código que puede ser útil.

El sinonimo de "traer cambios" para git es **git pull**
```bash
~/Documentos/ProyectoPtf/$ git pull origin master
remote: Counting objects: 3, done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From https://github.com/juancuiule/intro-a-git
 * branch            master     -> FETCH_HEAD
   8fd9c95..9fea9f2  master     -> origin/master
Merge made by the 'recursive' strategy.
 README.md | 21 +++++++++++++++++++--
 1 file changed, 19 insertions(+), 2 deletions(-)
```

En este caso podemos ver que hubo cambios en el archivo README.md
Es recomendable chequear que no haya cambios en el repo remoto que no hayamos traido al local para evitar conflictos al querer subir nuestros cambios.

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
    <a href="repositorio-remoto" class="my-btn">Anterior</a>
    <a href="branches" class="my-btn">Siguiente</a>
</div>
