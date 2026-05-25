# 🌸 Álbum de Alaia — PWA de Recuerdos Familiares

> Aplicación web progresiva (PWA) para guardar y compartir los recuerdos de **Alaia**, primera nieta de la familia Marín en Caucasia, Antioquia.

---

## 📋 Descripción

Álbum digital de fotos y videos diseñado para que la mamá pueda guardar todos los momentos especiales de Alaia directamente desde el celular. Funciona como una app instalable, sin conexión a internet, con panel de administración protegido por PIN.

---

## ✨ Características principales

- 📸 **Galería de fotos** organizada por etapas de vida
- 🎬 **Sección de videos** con reproductor integrado
- 📖 **Historia en carrusel** con fotos y videos mezclados
- 💜 **Sección "Sobre Alaia"** con carta del abuelo
- 🔐 **Panel de administración** protegido por PIN de 4 dígitos
- 💾 **Exportar / Importar** álbum completo (fotos + videos en formato .json)
- 🖨️ **Imprimir / Guardar como PDF**
- 💬 **Compartir por WhatsApp** — fotos, videos y resumen del álbum
- 📊 **Estadísticas** por etapa de vida
- ⚙️ **Configuración completa** — nombre, textos, carta del abuelo, PIN

---

## 🗂️ Estructura del proyecto

```
album-alaia/
├── index.html        ← Aplicación completa (archivo único)
└── README.md         ← Este archivo
```

---

## 🚀 Instalación y despliegue

### Opción 1 — Abrir directamente en el celular
1. Descargar `index.html`
2. Abrir con Chrome (Android) o Safari (iOS)
3. Listo para usar

### Opción 2 — GitHub Pages
```bash
git init
git add .
git commit -m "Album Alaia v1.0"
git remote add origin https://github.com/haroldco45/album-alaia.git
git push -u origin main
```
Activar GitHub Pages en **Settings → Pages → Branch: main**

### Opción 3 — Netlify (drag & drop)
1. Ir a [netlify.com](https://netlify.com)
2. Arrastrar la carpeta al área de deploy
3. URL disponible al instante

---

## 🔐 Acceso al panel de administración

| Campo | Valor por defecto |
|-------|------------------|
| PIN   | `1234`           |

> ⚠️ **Cambiar el PIN** desde Panel → Config → Cambiar PIN después del primer uso.

---

## 💾 Sistema de almacenamiento

Los datos se guardan automáticamente en el dispositivo usando `localStorage`. Para no perder los recuerdos:

1. **Exportar regularmente** desde Panel → Respaldo → Exportar todo
2. El archivo `.json` descargado contiene **todas las fotos y videos reales**
3. Para restaurar: Panel → Respaldo → Importar álbum

---

## 📱 Etapas de vida disponibles

| Etapa | Descripción |
|-------|-------------|
| Baby Shower | Celebración previa al nacimiento |
| Antes de nacer | Fotos del embarazo |
| Recién nacida | Primeros días de vida |
| Primeras semanas | Semanas 1-4 |
| 1 mes — 6 meses | Seguimiento mensual |
| Creciendo | Hitos de desarrollo |
| Primer año | El gran cumpleaños |

---

## 🛠️ Tecnologías utilizadas

| Tecnología | Uso |
|-----------|-----|
| HTML5 / CSS3 / JavaScript | Base de la aplicación |
| Google Fonts (Playfair Display + Lato) | Tipografía |
| localStorage / window.storage | Persistencia de datos |
| FileReader API | Carga de fotos y videos |
| Web Share / wa.me | Compartir por WhatsApp |
| window.print() | Exportar a PDF |

---

## 📤 Formato de exportación `.json`

```json
{
  "version": "3.0",
  "exportado": "2026-05-25T...",
  "nombreAlbum": "Alaia",
  "totalFotos": 12,
  "totalVideos": 3,
  "config": { ... },
  "fotos": [
    {
      "titulo": "Primera sonrisa",
      "desc": "Descripción",
      "emoji": "💜",
      "etapa": "Primeras semanas",
      "img": "data:image/jpeg;base64,...",
      "ts": 1748000000000
    }
  ],
  "videos": [ ... ]
}
```

---

## 👨‍💻 Desarrollado por

**Vibras Positivas HM**
- 🌐 GitHub: [github.com/haroldco45](https://github.com/haroldco45)
- 📱 WhatsApp: [3117700431](https://wa.me/573117700431)
- 📧 Email: haroldco45@gmail.com
- 📍 Caucasia, Antioquia — Colombia

---

> *Desarrollada por Vibras Positivas HM — Derechos de Autor Reservados*
