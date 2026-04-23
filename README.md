# Primera clase
# Trabajo Individual - Curso GIT SCESI 2026

## Jose Brayan Cruz Muruchi

---

## Clase 1 - Introducción a GIT

### ¿Qué es GIT?

GIT es un Sistema de Control de Versiones Distribuido (VCS). Básicamente 
nos permite guardar archivos y el historial de cambios de estos a lo largo del tiempo. Una buena manera de entenderlo es como los checkpoints de un  videojuego: si algo sale mal, puedes volver a un punto anterior sin perder todo tu progreso. Además, no es solo una herramienta individual, sino que puede usarla todo un equipo de trabajo al mismo tiempo.

### ¿Cómo nació GIT?

Linus Torvalds, el creador de Linux, recibía contribuciones al kernel de 
Linux por email y las revisaba manualmente una por una. Para organizarse 
mejor, él y su comunidad empezaron a usar BitKeeper, una herramienta de 
control de versiones que tenía una condición: no podías usar ninguna otra 
herramienta similar. En algún momento alguien rompió ese acuerdo y BitKeeper les quitó el acceso. Linus, en lugar de volver al método del email, decidió crear su propia herramienta. En aproximadamente 2 a 3 semanas de puro código y determinación, creó GIT. Así de simple (y dramático) fue su origen.

### ¿Cómo instalar GIT?

1. Ir a https://git-scm.com/install/
2. Descargar el instalador según tu sistema operativo (Windows, macOS o Linux)
3. Seguir los pasos de instalación recomendados
4. Verificar que quedó bien instalado con:

```bash
git --version
```


**Nota para Linux (Ubuntu/Debian):**
```bash
sudo apt-get install git
```

### Configuración inicial

Después de instalar, hay que decirle a GIT quién eres. Esto es importante 
porque cada cambio que hagas va a quedar registrado con tu nombre y correo.

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@correo.com"
git config --global core.autocrlf true
```

Para verificar que quedó guardado:
```bash
git config --global --list
```

### Archivos esenciales en todo repositorio

Todo repositorio debería tener al menos estos dos archivos:

- **README.md** → Es la carta de presentación del proyecto. Explica qué 
  hace, cómo usarlo, quién lo hizo, etc. Se escribe en formato Markdown.
- **.gitignore** → Le dice a GIT qué archivos debe ignorar (credenciales, 
  archivos temporales, etc.). Se verá más en detalle en clases futuras.

### Primeros pasos con GIT (adelanto de la clase)

Para inicializar un repositorio GIT en una carpeta:
```bash
git init
```

Para ver el estado de los archivos:
```bash
git status
```

Para agregar un archivo al seguimiento:
```bash
git add README.md
```

Para guardar los cambios (hacer un commit):
```bash
git commit -m "mi primer commit"
```

Para ver el historial de commits:
```bash
git log
```

### Formato básico de Markdown para el README

```markdown
# Título principal
## Subtítulo
### Sub-subtítulo

Párrafo normal así nomás.

# Bloque de código
código aquí
# fin bloque
```
