# ImmigraSmart — Landing Page

Sitio estático para promocionar [ImmigraSmart](https://immigrasmart.streamlit.app/), el asistente de inmigración con IA para estudiantes internacionales en la República Checa.

## 📦 Contenido del proyecto

```
immigrasmart-vercel/
├── index.html       # La página completa (HTML + CSS + JS en un solo archivo)
├── vercel.json      # Configuración de Vercel (headers de seguridad, caching)
├── package.json     # Metadatos del proyecto
└── README.md        # Este archivo
```

No hay paso de build. Es HTML estático puro — se despliega tal cual.

---

## 🚀 Cómo desplegar en Vercel (3 opciones)

### Opción 1 · Drag & drop (la más rápida)

1. Comprime la carpeta `immigrasmart-vercel` en un `.zip`
2. Ve a [vercel.com/new](https://vercel.com/new)
3. Arrastra el zip a la pantalla
4. Vercel detectará automáticamente que es un sitio estático
5. Click en **Deploy** — listo en ~10 segundos

### Opción 2 · Desde GitHub (recomendada para producción)

1. Sube esta carpeta a un repositorio nuevo en GitHub:
   ```bash
   cd immigrasmart-vercel
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/immigrasmart-landing.git
   git push -u origin main
   ```
2. En [vercel.com/new](https://vercel.com/new), conecta tu cuenta de GitHub
3. Selecciona el repo `immigrasmart-landing`
4. Vercel detectará el `package.json` y la configuración. **Framework Preset:** `Other`
5. Click **Deploy**

Cada `git push` a `main` desplegará automáticamente. Ramas y PRs generan preview URLs.

### Opción 3 · Vercel CLI (para desarrolladores)

```bash
# Instala la CLI (una sola vez)
npm i -g vercel

# Desde la carpeta del proyecto
cd immigrasmart-vercel
vercel

# Para producción
vercel --prod
```

---

## 🌐 Dominio personalizado

Después de desplegar:

1. Ve al dashboard del proyecto en Vercel
2. **Settings → Domains**
3. Agrega tu dominio (ej. `immigrasmart.com`)
4. Vercel te dará los registros DNS que debes configurar en tu proveedor (Namecheap, GoDaddy, Cloudflare, etc.)

Los certificados SSL son automáticos y gratuitos.

---

## 🛠 Desarrollo local

Para ver la página localmente antes de desplegar:

```bash
# Opción 1 — abre directo el archivo
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows

# Opción 2 — servidor local (mejor)
npx serve .
# o
python3 -m http.server 8000
```

---

## ✏️ Personalización rápida

Todo está en `index.html`. Variables principales en la parte superior del `<style>`:

```css
:root{
  --cz-blue: #11457E;     /* Azul checo principal */
  --cz-red:  #D7141A;     /* Rojo checo principal */
  --ink:     #0B1B3A;     /* Color de texto principal */
}
```

Cambia esos valores y el resto del sitio se adapta automáticamente.

### Enlaces a actualizar

Si cambias el repo o el dominio del demo, busca y reemplaza:
- `https://immigrasmart.streamlit.app/` → tu URL del demo
- `https://github.com/vanos0600/ImmigraSmart` → tu repo de GitHub

---

## 📋 Checklist post-deployment

- [ ] El sitio carga correctamente en `tu-proyecto.vercel.app`
- [ ] El botón "Launch the live demo" abre `immigrasmart.streamlit.app`
- [ ] El botón "View on GitHub" abre tu repo
- [ ] El sitio se ve bien en móvil (prueba en tu teléfono)
- [ ] Configuras dominio personalizado (opcional)
- [ ] Compartes el link 🚀

---

## 📄 Licencia

MIT — usa, modifica, distribuye libremente.

Hecho con ❤️ en Praga.
# Immigralanding
