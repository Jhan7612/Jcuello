# 🚀✨  ¡Pasos para desplegar tu Pokedex en Azure con Estilo! 🌐💡

### Link de la web en la nube: [WEB EN LA NUBE](https://nice-cliff-073b80310.6.azurestaticapps.net)

📚 **Información del Proyecto**  
- 🖋️ **Autor:** Jhan Carlos Cuello Vergara  
- 💻 **Repositorio:** [GitHub: Jcuello](https://github.com/Jhan7612/Jcuello)  
- 🏫 **Asignatura:** Sistemas Distribuidos  
- 🎓 **Semestre:** 9º Semestre - Ingeniería de Sistemas  
- 📅 **Fecha:** 25 de abril de 2025  

---

🌟 **¡Prepárate para llevar tu Pokedex a la nube!** Sigue esta guía paso a paso para desplegarla con éxito en Azure, de una forma sencilla, segura y ¡con estilo! 🚀🌈

## 1. 🍴 ¡A Clonar el Código! (Forking Time!) 🛠️

1.  Ve directo al corazón del código Pokedex: [https://github.com/rcuello/ac4dem1a/tree/master/sistemas-distribuidos/poke-dex-lab](https://github.com/rcuello/ac4dem1a/tree/master/sistemas-distribuidos/poke-dex-lab)
2.  En la esquina superior derecha, ¡busca el botón **Fork** y haz clic! 👆
3.  Ponle un nombre genial a tu copia, como **albertacho**, ¡y dale a **Create fork**! 🎉

---

## 2. 🗺️ ¡Navegando a la Ubicación Correcta! (App Location Adventure!) 🧭

1.  ¡Tu nuevo hogar para el código! 🏡 Visita: [https://github.com/Jhan7612/Jcuello](https://github.com/Jhan7612/Jcuello) 
2.  Sumérgete en las carpetas: **(https://github.com/Jhan7612/Jcuello)** 📂
3.  Encuentra el archivo mágico **azure-static-web-apps-delightful-field-02ef8bb10.yml** (¡puede tener un nombre  diferente!).
4.  ¡Es hora de editar! ✏️ Haz clic en el icono del lápiz.

    ```yaml
    app_location:
    ```
6.  ¡Reemplaza lo que esté entre las comillas por esta ruta secreta! 🤫
    ```yaml
    app_location: "./sistemas-distribuidos/poke-dex-lab/source/pokedex-angular"
    ```
7.  ¡Guarda los cambios con un clic en **Commit changes**! ✅

---

## 3. 🚦 ¡EMPEZEMOS! (Checking the Magic!) ✨

1.  En la parte superior de tu repo, ¡haz clic en **Actions**! 🎬
2.  Verás un flujo de trabajo en acción (o ya terminado) de Azure Static Web Apps. ¡Espera a que diga "completado" para estar seguro! ⏳

---

## 4. 🚀 ¡Despegue a la Nube de Azure! (Azure Deployment!) ☁️

1.  ¡Dirígete a tu **App Services** en Azure! 🌠
2.  Haz clic en el nombre de tu Static Web App.
3.  ¡Busca el botón **Ir al recurso** y haz clic con emoción! 😄
4.  En la sección de **URL**, ¡encontrarás el enlace mágico a tu Pokedex en la web! 🌐 ¡Haz clic para verlo! 👀

---

## 5. 🛡️ ¡Añadiendo Escudos de Seguridad y Rutas Inteligentes! (Security & Navigation!) 🧭

1.  De vuelta a tu repositorio: [https://github.com/Jhan7612/Jcuello](https://github.com/Jhan7612/Jcuello) 
2.  Navega a: **sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/** 📂
3.  ¡Crea un nuevo archivo! ➕ Haz clic en **Add file** y luego en **Create new file**.
4.  ¡Nómbralo con estilo! 🏷️ **staticwebapp.config.json**
5.  ¡Pega este código secreto para la seguridad y navegación! 🔒
    ```json
    {
      "globalHeaders": {
        "Content-Security-Policy": "default-src 'self'; img-src 'self' [https://raw.githubusercontent.com](https://raw.githubusercontent.com) [https://pokeapi.co](https://pokeapi.co) [https://assets.pokemon.com](https://assets.pokemon.com); script-src 'self' 'unsafe-inline'; style-src 'self' 'unsafe-inline' [https://fonts.googleapis.com](https://fonts.googleapis.com); font-src 'self' [https://fonts.gstatic.com](https://fonts.gstatic.com); connect-src 'self' [https://beta.pokeapi.co](https://beta.pokeapi.co)",
        "X-Frame-Options": "DENY",
        "Permissions-Policy": "geolocation=(), microphone=(), camera=()"
      },
      "navigationFallback": {
        "rewrite": "/index.html",
        "exclude": ["/images/", "/css/", "/js/*", "/favicon.ico"]
      }
    }
    ```
6.  ¡Guarda los cambios con **Commit changes**! ✅
7.  Ve a **Actions** de nuevo y espera a que la magia de Azure Static Web Apps se complete. ✨

---

## 6. 🖼️ ¡Dando Vida a los Pokémon con Imágenes! (Loading Pokemon Images!) 🎨

1.  Ve a esta ruta en tu repo: **Jcuello/sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/src/environments/** 📂
2.  ¡Edita el archivo **environment.prod.ts**! ✏️
3.  Busca la línea de la ruta de las imágenes:
    ```typescript
    imagesPath: 'pokedex-angular/assets/images',
    ```
4.  ¡Cámbiala a esta ruta mágica! ✨
    ```typescript
    imagesPath: '/assets/images',
    ```
5.  ¡Guarda los cambios con **Commit changes**! ✅
6.  ¡Una última visita a **Actions**! ⏳ Espera a que termine el proceso. ¡Y listo! 🎉 Tus imágenes de Pokémon deberían aparecer.

¡Enhorabuena! 🎊 Tu Pokedex ya está funcionando en Azure Static Web Apps y ha quedado espectacular. Ahora está listo para brillar en la nube, ¡disfrútalo al máximo! 🚀☁️ 🚀

---

---

## 🧑‍💻 **¿Quién creó este programa?**
El creador del programa es **Jhan Carlos Cuello Vergara**, experto en diversas áreas que aportan valor a este proyecto:

### **Experiencias destacadas**
- **👨‍💻 Desarrollador de software**: Diseñando soluciones técnicas innovadoras.
- **📋 Líder de proyectos institucionales**: Gestionando y ejecutando proyectos estratégicos.
- **📈 Marketing digital**: Impulsando la presencia de marcas en el ecosistema digital.
- **🖥️ Digitalizador**: Transformando procesos tradicionales en eficiencias modernas.




