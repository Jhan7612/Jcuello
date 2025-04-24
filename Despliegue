# 🌐 **Despliegue de un Sitio en Azure Static Web Apps (100% en la nube)**

¡Aprende cómo desplegar tu aplicación en la nube con este tutorial increíblemente dinámico y 100% práctico! 🚀

---

## 📋 **Información del Proyecto**
- **🌟 Autor:** Jhan Carlos Cuello Vergara 
- **📂 Repositorio:** [Enlace al repositorio de GitHub](https://github.com/Jhan7612/Jcuello)  
- **📚 Asignatura:** Sistemas Distribuidos  
- **🎓 Semestre:** 9no Semestre - Ingeniería de Sistemas  
- **📅 Fecha:** 25/04/2025  
- **🔗 URL del sitio desplegado:** [Delightful Field](https://nice-cliff-073b80310.6.azurestaticapps.net)  

---

## 🛠 **Requisitos Previos**
Antes de empezar, asegúrate de contar con:
- ✅ Una cuenta en **GitHub**.
- ✅ Una cuenta activa en **Azure**.
- ✅ Entre **5 y 10 minutos** de tu tiempo.

---

## 🌀 **1. Haz un Fork del Repositorio**
### Pasos:
1. Ve al repositorio original en GitHub: [Haz clic aquí](https://github.com/Albertohincapie11/albertacho).
2. Pulsa el botón **"Fork"** (arriba a la derecha).
3. Selecciona tu cuenta de GitHub como destino del fork.
4. *(Opcional)* Cambia el nombre del repositorio si lo deseas.

🎉 ¡Ahora tienes tu propia copia del repositorio!

---

## ☁️ **2. Crea una Static Web App en Azure**
### Pasos:
1. Accede al **Portal de Azure**: [Ir al portal](https://portal.azure.com).
2. Busca "Static Web Apps" y haz clic en **Crear**.
3. Completa los siguientes campos:
   - **Subscription:** Tu suscripción activa en Azure.
   - **Resource Group:** Crea uno nuevo o selecciona uno existente.
   - **Name:** Elige un nombre único para tu aplicación.
   - **Region:** Selecciona la región más cercana a tus usuarios.
   - **Deployment Source:** Elige **GitHub**.
4. Autoriza a Azure a acceder a tu cuenta de GitHub si es tu primera vez.
5. Selecciona el **repositorio fork** que creaste.
6. Escoge la rama principal (**main** o **master**).
7. En **Build Details**, configura lo siguiente:
   - **Build Presets:** El tipo de aplicación (React, Angular, Vue, etc.) o selecciona **Custom**.
   - **App Location:** Ruta raíz del código fuente (`/` si está en la raíz).
   - **Output Location:** Carpeta donde se genera el sitio compilado (`dist/`, `build/`, etc.).
8. Revisa todo y haz clic en **Crear**.

⏳ ¡Azure se encargará del resto! 🚀

---

## 🛡️ **3. Agrega Cabeceras de Seguridad**
1. Crea un archivo llamado `staticwebapp.config.json` en tu repositorio.
2. Copia y pega el siguiente contenido para mejorar la seguridad HTTP:

```json
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
---

## 🧑‍💻 **¿Quién creó este programa?**
El creador del programa es **Jhan Carlos Cuello Vergara**, experto en diversas áreas que aportan valor a este proyecto:

### **Experiencias destacadas**
- **👨‍💻 Desarrollador de software**: Diseñando soluciones técnicas innovadoras.
- **📋 Líder de proyectos institucionales**: Gestionando y ejecutando proyectos estratégicos.
- **📈 Marketing digital**: Impulsando la presencia de marcas en el ecosistema digital.
- **🖥️ Digitalizador**: Transformando procesos tradicionales en eficiencias modernas.
