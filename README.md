# AI4Green Platform

Plataforma educativa para integrar Inteligencia Artificial y Sostenibilidad en educación STEAM.

## 🚀 Instalación

### Requisitos previos

- Ruby >= 2.7
- RubyGems
- GCC y Make

### Instalación local

1. **Clona el repositorio**
```bash
git clone https://github.com/eloisa-glez/AI4Green-Platform_v4.git
cd AI4Green-Platform_v4
```

2. **Instala las dependencias**
```bash
bundle install
```

3. **Ejecuta Jekyll localmente**
```bash
bundle exec jekyll serve
```

4. **Abre en tu navegador**
```
http://localhost:4000/AI4Green-Platform_v4/
```

## 📁 Estructura del Proyecto

```
AI4Green-Platform_v4/
├── _config.yml           # Configuración del sitio
├── _layouts/             # Plantillas HTML
│   ├── base.html        # Layout principal con diseño de 3 paneles
│   ├── home.html        # Layout para página de inicio
│   └── page.html        # Layout para páginas regulares
├── _materials/          # Colección de materiales educativos
├── index.md             # Página de inicio
├── materials.md         # Página de materiales
├── project.md           # Información del proyecto
├── team.md              # Equipo del proyecto
├── Gemfile              # Dependencias Ruby
└── README.md            # Este archivo
```

## 🎨 Personalización

### Cambiar colores

Edita las variables CSS en `_layouts/base.html`:

```css
:root {
    --sidebar-width: 300px;
    --bg-green: #0a4f4f;      /* Color verde principal */
    --accent: #fec107;         /* Color de acento (amarillo) */
}
```

### Modificar el menú

Edita `_config.yml`:

```yaml
menu:
  - title: Home
    url: /
  - title: Tu Nueva Sección
    url: /nueva-seccion/
```

### Añadir páginas

Crea un nuevo archivo `.md` en la raíz:

```markdown
---
layout: page
title: Mi Nueva Página
breadcrumb: MI PÁGINA
---

Contenido de tu página...
```

## 📝 Añadir Contenido Educativo

### Crear un nuevo material

1. Crea un archivo en `_materials/`:

```markdown
---
layout: page
title: "Nombre del Material"
description: "Breve descripción"
---

Contenido del material...
```

### Usar Markdown

El contenido usa Markdown estándar:

```markdown
# Título 1
## Título 2

**Negrita** y *cursiva*

- Lista
- De elementos

[Enlace](https://ejemplo.com)

![Imagen](ruta/imagen.jpg)
```

## 🌐 Despliegue en GitHub Pages

1. **Sube tu código a GitHub**

2. **Activa GitHub Pages**:
   - Ve a Settings > Pages
   - Source: Deploy from branch
   - Branch: main (o master)
   - Carpeta: / (root)

3. **Tu sitio estará en**:
   ```
   https://eloisa.glez.github.io/AI4Green-Platform_v4/
   ```

## 🎯 Características del Diseño

### Navegación de 3 Paneles

- **Panel Izquierdo**: Menú lateral (oculto inicialmente)
- **Panel Central**: Página de inicio con logo AI
- **Panel Derecho**: Contenido con menú lateral visible

### Controles de Navegación

- **Scroll horizontal**: Cambia entre paneles
- **Flechas del teclado**: ← → para navegar
- **Click en intro**: Va al contenido
- **Botón menú**: Muestra panel lateral

## 🔧 Comandos Útiles

```bash
# Servir el sitio localmente
bundle exec jekyll serve

# Servir con drafts
bundle exec jekyll serve --drafts

# Servir en un puerto diferente
bundle exec jekyll serve --port 4001

# Build para producción
bundle exec jekyll build

# Limpiar archivos generados
bundle exec jekyll clean
```

## 📚 Recursos

- [Documentación Jekyll](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Pages](https://docs.github.com/es/pages)

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo licencia MIT. Ver `LICENSE` para más detalles.

## 👥 Contacto

**AI4Green Team**
- Email: contact@ai4green.org
- GitHub: [@eloisa-glez](https://github.com/eloisa-glez)

## 🙏 Agradecimientos

- Programa Erasmus+ por financiar este proyecto
- Todos los educadores y estudiantes participantes
- La comunidad Jekyll por las herramientas

---

**Nota**: Este es un proyecto educativo financiado por Erasmus+ (2024-2027)
