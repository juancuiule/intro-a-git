# Instalación
---

Antes de poder empezar a usar git tenemos que instalarlo. El proceso de instalación es simple pero varía dependiendo del sistema operativo en el que desarrollemos.

### Instalación en sistemas GNU/Linux
Para instalar git en un sistema de este tipo podemos usar la consola.

#### Debian/Ubuntu
```bash
$ sudo apt-get install git-all
```

Para ver cómo realizar la instalación en otras distribuciones hacer click [aquí](https://git-scm.com/download/linux)

### Instalación en Windows

Vamos a instalar git por medio de un ejecutable que podemos encontrar haciendo click [aquí](https://git-scm.com/download/win)

### Instalación en Mac

Vamos a instalar git por medio de un ejecutable que podemos encontrar haciendo click [aquí](https://git-scm.com/download/mac)

### Interfaces Gráficas

Si no sos muy amigo de la consola de comandos, existen distintos progrmas que te van a permitir usar git de una manera visual. Si bien no se maneja por comandos los conceptos del manejo de versiones que vamos a ver son los mismos.
Podes encontrar una lista con todos ellos [aquí](https://git-scm.com/downloads/guis)

# Configuración
---

Ahora que ya tenemos git instalado, vamos a configurar el entorno. Sólo necesitamos hacer esto una sola vez, sin embargo es posible cambiarlo en cualquier momento volviendo a ejecutar los comandos que vamos a ver ahora.

Empezemos por configurar nuestra identidad, git usa esta información para confirmar los cambios realizados y para informar quién fue el que los hizo.

```bash
$ git config --global user.name "Juan Cuiule"
$ git config --global user.email juan.cuiule@bue.edu.ar
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
    <a href="index" class="my-btn">Anterior</a>
    <a href="git-init-clone" class="my-btn">Siguiente</a>
</div>
