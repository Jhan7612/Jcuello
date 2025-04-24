# 🚀 Despliega tu Pokedex en Azure con Estilo 🌟

¡Lleva tu Pokedex a la nube de manera súper sencilla y visual! ☁️

📌 **Información del Proyecto**
- **Web:** [Delightful Field](https://delightful-field-02ef8bb10.6.azurestaticapps.net/)
- **Autor:** Alberto José Hincapié Martínez
- **Repositorio:** [albertacho](https://github.com/Albertohincapie11/albertacho)
- **Asignatura:** Sistemas Distribuidos
- **Semestre:** Noveno semestre - Ingeniería de Sistemas
- **Fecha:** 13/04/2025

---

## 🎯 Pasos para el Despliegue

### 🍴 Paso 1: ¡A Bifurcar el Código! 🛠️
- Dirígete al repositorio original del código de Pokedex: [Pokedex Lab](https://github.com/rcuello/ac4dem1a/tree/master/sistemas-distribuidos/poke-dex-lab).
- Haz clic en **Fork** en la esquina superior derecha.
- Asigna un nombre como `albertacho` y presiona **Create Fork** 🎉.

---

### 🗺️ Paso 2: Navegando a la Ubicación Correcta 🧭
- Accede a tu nuevo repositorio: [albertacho](https://github.com/albertacho/albertacho).
- Navega hasta `albertacho/.github/workflows/`.
- Encuentra el archivo `azure-static-web-apps-delightful-field-02ef8bb10.yml` y haz clic en el ✏️ **ícono del lápiz**.
- Edita la línea #31:
  ```yaml
  app_location: "./sistemas-distribuidos/poke-dex-lab/source/pokedex-angular"
Guarda los cambios con Commit changes ✅.

🚦 Paso 3: ¡Luces, Cámara, Actions! ✨
Ve a la pestaña Actions en tu repositorio.

Verifica que el flujo de trabajo de Azure Static Web Apps esté ejecutándose. Espera a que diga "completado" ⏳.

🚀 Paso 4: Despegue a la Nube ☁️
Accede a App Services en Azure.

Haz clic en el nombre de tu Static Web App.

En la sección de URL, encontrarás el enlace mágico a tu Pokedex 🌐. ¡Haz clic y disfruta! 👀

🛡️ Paso 5: Configuración de Seguridad 🔒
Desde tu repositorio albertacho, navega a sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/.

Crea un archivo llamado staticwebapp.config.json.

Añade el siguiente contenido:
{
  "globalHeaders": {
    "Content-Security-Policy": "default-src 'self'; img-src 'self' https://raw.githubusercontent.com https://pokeapi.co https://assets.pokemon.com; script-src 'self' 'unsafe-inline'; style-src 'self' 'unsafe-inline' https://fonts.googleapis.com; font-src 'self' https://fonts.gstatic.com; connect-src 'self' https://beta.pokeapi.co",
    "X-Frame-Options": "DENY",
    "Permissions-Policy": "geolocation=(), microphone=(), camera=()"
  },
  "navigationFallback": {
    "rewrite": "/index.html",
    "exclude": ["/images/", "/css/", "/js/*", "/favicon.ico"]
  }
}

Guarda los cambios con Commit changes ✅.

🖼️ Paso 6: Carga de Imágenes de Pokémon 🎨
Ve a albertacho/sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/src/environments/.

Edita environment.prod.ts y cambia la ruta de imágenes:
imagesPath: '/assets/images';
Guarda los cambios con Commit changes ✅.

🎉 ¡Todo Listo!
Verifica nuevamente en Actions que el proceso haya terminado.

¡Tu Pokedex está desplegado en la nube con imágenes funcionando perfectamente! 🎨

¡Ahora disfruta de tu creación y compártela con el mundo! 🚀





