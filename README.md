# Cordillera Grupo Constructor — Sitio web

**Legalizamos y construimos tus sueños.**

Sitio web estático (HTML + CSS, sin dependencias). No necesita instalar nada ni compilar: Vercel lo publica tal cual.

## Estructura

```
cordillera-web/
├── index.html      ← todo el contenido de la página (textos, secciones, enlaces)
├── css/
│   └── styles.css  ← colores, tipografías y diseño
├── img/            ← logo, favicon y fotos
├── robots.txt
└── README.md
```

## Cómo hacer cambios comunes

| Quiero cambiar…            | Dónde                                                                 |
|----------------------------|-----------------------------------------------------------------------|
| Un texto                   | `index.html`, busca el texto y cámbialo. Cada sección tiene un comentario `<!-- ===== NOMBRE ===== -->`. |
| Una foto                   | Reemplaza el archivo en `img/` **con el mismo nombre** (por ejemplo `img/detalle-licencias.jpg`). |
| El teléfono / WhatsApp     | En `index.html` busca `3138447395` y `313 844 7395` y reemplaza todas las apariciones. |
| El correo                  | En `index.html` busca `cordilleragrupoconstructor@gmail.com`.         |
| Los colores                | Al inicio de `css/styles.css`, en `:root` (`--navy`, `--blue`, `--green`, `--cream`…). |

Consejo: las fotos funcionan mejor en `.jpg`, de unos 1200–1600 px de ancho y menos de 400 KB.

## Publicar por primera vez

### 1. Subir a GitHub
1. Entra a <https://github.com/new>, ponle un nombre (ej. `cordillera-web`) y crea el repositorio.
2. Haz clic en **"uploading an existing file"**, arrastra **el contenido** de esta carpeta (`index.html`, `css`, `img`, etc.) y pulsa **Commit changes**.

   (Si usas Git en tu computador:)
   ```bash
   git init
   git add .
   git commit -m "Primera versión del sitio"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/cordillera-web.git
   git push -u origin main
   ```

### 2. Publicar en Vercel
1. Entra a <https://vercel.com> e inicia sesión con tu cuenta de GitHub.
2. **Add New → Project**, elige el repositorio `cordillera-web` y pulsa **Import**.
3. Framework Preset: **Other**. No cambies nada más y pulsa **Deploy**.
4. En un minuto tendrás tu sitio en una dirección `https://cordillera-web.vercel.app`.

### 3. Tu propio dominio (opcional)
En Vercel: **Project → Settings → Domains → Add**, escribe tu dominio (ej. `cordillerags.com`) y sigue las instrucciones para configurar los DNS donde lo compraste.

## Actualizar el sitio
Cada vez que guardes un cambio en GitHub (editando un archivo con el lápiz ✏️ o subiendo uno nuevo y pulsando **Commit changes**), Vercel publica la nueva versión automáticamente en uno o dos minutos.

---
© 2026 Cordillera Grupo Constructor · Bogotá, D.C. Colombia · 313 844 7395
