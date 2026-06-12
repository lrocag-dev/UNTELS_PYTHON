# Parte 1: Instalación de Git en Windows 11
## Paso 1: Descargar Git
Abrir Chrome/Edge y buscar "git for windows" o ir a:

```console
https://git-scm.com/download/win
La descarga empezará automáticamente (archivo Git-x.xx.x-64-bit.exe)
```
## Paso 2: Instalar Git
Ejecutar el instalador (dar clic derecho → "Ejecutar como administrador" si pide permisos)

- Aceptar licencia → Next
- Seleccionar ubicación → C:\Program Files\Git → Next
- Componentes → Dejar todo por defecto → Next
- Editor predeterminado → Elegir "Nano" o "VSCode" (recomiendo Nano para principiantes) → Next
- Ajustar PATH → Elegir: "Git from the command line and also from 3rd-party software" → Next
- Opciones HTTPS → Usar "OpenSSL library" → Next
- Configuración de terminal → Elegir "MinTTY" → Next
- Extra options → Dejar por defecto → Next
- Instalar → Esperar 1-2 minutos → Finish

## Paso 3: Verificar instalación
Abrir PowerShell o Símbolo del sistema y escribir:

```console
git --version
Debe mostrar algo como: git version 2.43.0.windows.1
```

# Parte 2: Configurar Git (solo primera vez)
En la terminal (PowerShell o CMD), escribir:
```console
git config --global user.name "lrocag-dev"
git config --global user.email "tu-email@ejemplo.com"
```
Importante: Usar el mismo email con el que creaste la cuenta de GitHub.

Verificar configuración:
```console
git config --global --list
```
# Parte 3: Crear carpeta del proyecto y descargar ejercicios
Clonar el repositorio
```console
# Ir al escritorio o a una carpeta de trabajo
cd C:\Users\TU_USUARIO\Desktop

# Clonar (descargar) el repositorio
git clone https://github.com/lrocag-dev/UNTELS_PYTHON.git

# Entrar a la carpeta
cd UNTELS_PYTHON/ejercicios

# Crear la carpeta persoal
mkdir tu_nombre

# Copias tus respuestas en la carpeta personal
# Agregas la carpeta al git
git add tu_nombre

# Verifica que los archivos han sido agregados
git status

# Subir los ejercicios
git commit -m "Ejercicios - tu_nombre"
git push origin main
```


# Alternativa sin Git
Si algún estudiante tiene problemas con Git, pueden usar GitHub Desktop (interfaz gráfica):

- Descargar: https://desktop.github.com/
- Instalar y loguearse con GitHub
- File → Clone repository → Elegir lrocag-dev/UNTELS_PYTHON
- Arrastrar archivos a la carpeta
- Escribir mensaje y click "Commit to main" → "Push origin"

