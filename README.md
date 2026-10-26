# Guía de Realidad Aumentada (WebAR) con JavaScript y GitHub Pages

Esta aplicación de **Realidad Aumentada Web (WebAR)** permite visualizar una figura geométrica 3D animada (rotación continua, levitación y pulsación) directamente desde el navegador de un celular apuntando a un marcador impreso o mostrado en otra pantalla.

---

## 🚀 ¿Se puede utilizar GitHub Pages?

**¡SÍ, de hecho es la MEJOR opción y la recomendada!**

### ¿Por qué GitHub Pages es ideal para Realidad Aumentada?
1. **Obligatoriedad de HTTPS:** Los navegadores móviles (Google Chrome, Safari, etc.) **bloquean el acceso a la cámara** si el sitio web no tiene un certificado de seguridad SSL (`https://`). GitHub Pages incluye **HTTPS gratis y automático**.
2. **Sin necesidad de instalar servidores:** Como la aplicación está hecha en HTML y JavaScript puro (cliente), no requiere backend, base de datos ni Node.js en producción.
3. **Acceso inmediato desde el celular:** Simplemente abres el enlace generado o escaneas un código QR con la cámara de tu teléfono.

---

## 📂 Archivos del Proyecto

- `index.html`: Aplicación completa con A-Frame, AR.js, controles táctiles y animación 3D.
- `marcador-hiro.png`: Imagen del marcador Hiro que debes enfocar con la cámara del celular.

---

## 🛠️ Cómo publicar en GitHub Pages (Paso a Paso)

### Opción A: Desde la web de GitHub (Sin comandos)
1. Entra a [github.com](https://github.com) e inicia sesión.
2. Crea un nuevo repositorio público (ejemplo: `animacion-ra`).
3. Sube los archivos `index.html` y `marcador-hiro.png` arrastrándolos a la web de GitHub.
4. Ve a la pestaña **Settings** (Configuración) de tu repositorio.
5. En el menú lateral izquierdo, haz clic en **Pages**.
6. En la sección **Branch**, selecciona la rama `main` (o `master`) y la carpeta `/ (root)`. Haz clic en **Save**.
7. En unos 30 a 60 segundos, GitHub te dará tu enlace público:  
   `https://tu-usuario.github.io/animacion-ra/`

---

### Opción B: Mediante Git en tu terminal
```bash
cd "c:\Users\ELITEBOOK\Documents\5to semestre\graficacion\realidad_aumentada"
git init
git add .
git commit -m "Proyecto Realidad Aumentada 3D WebAR"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git
git push -u origin main
```
Luego activas **Pages** en la pestaña *Settings* > *Pages* como se describe arriba.

---

## 📱 Cómo probar la aplicación en tu celular

1. **Abre el enlace de GitHub Pages en tu teléfono** (puedes crear un código QR gratuito de tu URL en [qr-code-generator.com](https://www.qr-code-generator.com/) para abrirlo al instante con la cámara).
2. El navegador te pedirá **Permiso para usar la cámara** -> Presiona **Permitir**.
3. Abre el archivo `marcador-hiro.png` en la pantalla de tu computadora o imprímelo en papel.
4. Apunta la cámara del celular hacia el marcador:
   - Verás la figura 3D aparecer sobre el marcador.
   - Tendrá **animación de rotación multi-eje continua**.
   - Tendrá **efecto de levitación suave**.
   - La esfera interior tendrá **animación pulsante**.
5. Usa los botones en pantalla para interactuar:
   - **🎨 Color:** Cambia los tonos del material.
   - **🔄 Figura:** Alterna entre Cubo, Pirámide/Cono e Icosaedro.
   - **📷 Ver Marcador:** Muestra el marcador directamente si necesitas descargarlo o mostrarlo.
