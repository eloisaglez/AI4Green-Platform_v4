# 🚀 Guía Rápida de Inicio - AI4Green Jekyll

## ✅ Lo que tienes ahora

Tu proyecto Jekyll está completamente configurado con:

✓ Diseño de 3 paneles (menú lateral, intro, contenido)
✓ 4 páginas creadas (Home, Materials, Project, Team)
✓ Sistema de navegación con scroll y teclado
✓ Configuración lista para GitHub Pages
✓ Ejemplo de material educativo
✓ Despliegue automático con GitHub Actions

## 📦 Estructura de Archivos

```
AI4Green-Jekyll/
├── _config.yml              ← Configuración principal
├── _layouts/
│   ├── base.html           ← Layout con diseño de 3 paneles
│   ├── home.html           ← Para página de inicio
│   └── page.html           ← Para páginas normales
├── _materials/             ← Tus materiales educativos
│   └── ml-for-climate.md   ← Ejemplo de material
├── index.md                ← Página de inicio
├── materials.md            ← Página de materiales
├── project.md              ← Página del proyecto
├── team.md                 ← Página del equipo
├── Gemfile                 ← Dependencias Ruby
├── README.md               ← Documentación completa
└── .github/workflows/
    └── jekyll.yml          ← GitHub Actions para despliegue
```

## 🏃 Pasos para Usar

### Opción 1: Probar Localmente (Recomendado primero)

1. **Instala Ruby** (si no lo tienes):
   - Windows: https://rubyinstaller.org/
   - Mac: `brew install ruby`
   - Linux: `sudo apt-get install ruby-full`

2. **Navega a la carpeta del proyecto**:
   ```bash
   cd AI4Green-Jekyll
   ```

3. **Instala dependencias**:
   ```bash
   bundle install
   ```

4. **Ejecuta Jekyll**:
   ```bash
   bundle exec jekyll serve
   ```

5. **Abre en el navegador**:
   ```
   http://localhost:4000/AI4Green-Platform_v4/
   ```

### Opción 2: Subir a GitHub Pages (Para publicar)

1. **Crea un repositorio en GitHub** llamado `AI4Green-Platform_v4`

2. **Sube los archivos**:
   ```bash
   cd AI4Green-Jekyll
   git init
   git add .
   git commit -m "Initial commit - AI4Green Platform"
   git branch -M main
   git remote add origin https://github.com/eloisa-glez/AI4Green-Platform_v4.git
   git push -u origin main
   ```

3. **Activa GitHub Pages**:
   - Ve a Settings > Pages
   - Source: GitHub Actions (ya está configurado)
   - ¡Espera 2-3 minutos y estará listo!

4. **Tu sitio estará en**:
   ```
   https://eloisa.glez.github.io/AI4Green-Platform_v4/
   ```

## ✏️ Personalización Rápida

### Cambiar título y descripción

Edita `_config.yml`:
```yaml
title: AI4Green
description: Empowering Sustainability with AI
```

### Añadir una nueva página

1. Crea `mi-pagina.md` en la raíz:
```markdown
---
layout: page
title: Mi Nueva Página
breadcrumb: MI PÁGINA
---

Contenido aquí...
```

2. Añádela al menú en `_config.yml`:
```yaml
menu:
  - title: Mi Página
    url: /mi-pagina/
```

### Crear un nuevo material educativo

Crea un archivo en `_materials/`:
```markdown
---
layout: page
title: "Nombre del Material"
breadcrumb: MATERIALS / MI MATERIAL
---

Contenido del material...
```

### Cambiar colores

En `_layouts/base.html`, busca:
```css
:root {
    --bg-green: #0a4f4f;    ← Color verde
    --accent: #fec107;       ← Color amarillo
}
```

## 🎨 Características del Diseño

### Navegación
- **Scroll horizontal**: Cambia entre paneles
- **Flechas ← →**: Navegación con teclado
- **Click en intro**: Va al contenido
- **Botón menú**: Muestra panel lateral

### Páginas
- **Home** (`index.md`): Con intro animada "ai"
- **Otras páginas**: Empiezan directamente en el contenido

## 📝 Formato de Contenido

Usa Markdown estándar:

```markdown
# Título Grande
## Título Mediano
### Título Pequeño

**Negrita** y *cursiva*

- Lista
- De elementos

1. Lista
2. Numerada

[Enlace](https://ejemplo.com)

![Imagen](ruta/imagen.jpg)

> Cita en bloque
```

Nota especial:
```markdown
<div class="note">
<strong>IMPORTANTE</strong>
Texto destacado
</div>
```

## 🐛 Solución de Problemas

### Jekyll no arranca
```bash
bundle update
bundle exec jekyll serve --trace
```

### Cambios no se ven
```bash
bundle exec jekyll clean
bundle exec jekyll serve
```

### Errores en GitHub Pages
- Revisa el tab "Actions" en GitHub
- Asegúrate que `_config.yml` tiene la URL correcta

## 🆘 Necesitas Ayuda?

1. Lee el `README.md` completo
2. Revisa la documentación de Jekyll: https://jekyllrb.com
3. Busca en los Issues de GitHub
4. Contacta al equipo: contact@ai4green.org

## 🎯 Próximos Pasos

1. ✅ Prueba localmente con `bundle exec jekyll serve`
2. ✅ Personaliza los colores y textos
3. ✅ Añade tus propios materiales educativos
4. ✅ Sube a GitHub
5. ✅ Activa GitHub Pages
6. ✅ ¡Comparte tu sitio!

---

**¡Éxito con tu proyecto AI4Green! 🌱🤖**
