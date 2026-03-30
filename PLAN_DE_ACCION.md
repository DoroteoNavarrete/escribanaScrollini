# Estudio Scrollini — Web Demo

## 🧠 Contexto del Agente (leer al inicio de cada sesión)

Eres un desarrollador frontend experto. Estás construyendo una **SPA demo** para vender a un cliente:
**Estudio Scrollini**, Escribanía Notarial con operaciones en Maldonado, Punta del Este, La Barra, Manantiales, La Juanita, José Ignacio, Garzón, San Carlos y Pueblo Edén, Uruguay.

### Criterios globales del proyecto
- Stack: **HTML5 + CSS3 + JS Vanilla** — sin frameworks
- Diseño: **minimalista**, limpio, elegante, mucho espacio en blanco, profesional
- **Mobile-first**, totalmente responsive
- Hero con fondo oscuro (gradiente charcoal), texto blanco
- Todo el contenido no confirmado por el cliente lleva `<!-- TODO: ajustar con cliente -->`
- No agregar dependencias externas salvo Google Fonts (Inter) y Lucide Icons (CDN)

---

### Stack de archivos
```
Ejemplos/estudioScrollini/
├── index.html
├── PLAN_DE_ACCION.md
├── css/
│   └── styles.css
└── js/
    └── main.js

Imágenes (referenciadas como ../../img/):
  logo.png          ← logo del estudio
  Screenshot_3.png  ← imagen hero (enmarcada)
  photo.png         ← foto de la Escribana Elisa Scrollini
```

---

### Paleta de colores

| Variable CSS     | Valor     | Uso                                          |
|------------------|-----------|----------------------------------------------|
| `--primary`      | `#4A4546` | Charcoal cálido — CTAs, botones, iconos      |
| `--primary-hover`| `#2A2527` | Hover sobre elementos primarios              |
| `--silver`       | `#CCCACB` | Plata cálida — color principal del cliente, badges, detalles decorativos |
| `--dark`         | `#2A2527` | Fondo hero, textos principales               |
| `--gray`         | `#6B6668` | Textos secundarios                           |
| `--light-gray`   | `#F5F4F4` | Fondos de secciones alternas                 |
| `--white`        | `#ffffff` | Fondos blancos y textos sobre color          |
| `--border`       | `#E8E6E7` | Bordes y separadores                         |

**Tipografía**: `Inter` via Google Fonts (400, 500, 600, 700)

---

### Datos del cliente

| Campo           | Valor                                                                                   |
|-----------------|-----------------------------------------------------------------------------------------|
| Nombre          | Estudio Scrollini                                                                       |
| Escribana       | Elisa Scrollini                                                                         |
| Slogan          | "Seguridad jurídica con calidez humana."                                                |
| Rubro           | Estudio Notarial en Uruguay                                                             |
| Zonas           | Maldonado · Punta del Este · La Barra · Manantiales · La Juanita · José Ignacio · Garzón · San Carlos · Pueblo Edén |
| WhatsApp        | 094 058 039 (`+59894058039`)                                                            |
| Email           | escelisascrollini@gmail.com                                                             |
| Instagram       | https://www.instagram.com/escribanaelisascrollini/                                      |
| Google Maps     | https://www.google.com/maps/place/Estudio+Scrollini                                     |
| Rating Google   | ⭐ 5.0                                                                                  |

**Horario**

| Día             | Horario                         |
|-----------------|---------------------------------|
| Lunes–Miércoles | 9:00–12:00 / 13:00–19:30        |
| Jueves–Viernes  | 9:00–12:00 / 13:00–19:30        |
| Sábado          | 9:00–12:00                      |
| Domingo         | Cerrado                         |

---

### Servicios notariales (generados — confirmar con cliente)

- Compraventa de Inmuebles
- Poderes Notariales
- Sucesiones y Herencias
- Certificaciones y Autenticaciones
- Constitución de Sociedades
- Arrendamientos
- Testamentos y Protocolizaciones
- Habilitaciones Comerciales
- Promesas de Compraventa
- Divorcios y Separaciones

---

### Reseñas (Google — 20 reales + inventadas para los que no tenían texto)

1. **Lucia Sosa** — "Elisa excelente profesional y humana. Siempre nos han atendido muy bien con todo, hemos realizado muchos trámites en el estudio."
2. **Esther Bravo** — "El estudio espectacular, el Servicio es muy bueno. La Srta Scrollini siempre a disposición y buenas resoluciones."
3. **Pedro Guillen** — "Muy buena atención y rápida resolución para distintos trámites. Todo muy bien, 10 puntos."
4. **Matias Villar** — "Excelente profesional, me ayudó con ciertos documentos para resolver un problema de contribución de terreno. Clara y detallada."
5. **Tania Ferreira** — "Excelente atención, muy buena profesional."
6. **Gabriel Dominguez** — "Excelente atención, ágil solución."
7. **Carla Graña** — "Excelente atención!! Profesionalidad, y gestión de buen trato con el cliente. Super recomendable."
8. **Sebastian Gomez** — "Excelente servicio. Muy confiable además de realizar los trabajos sin demoras."
9. **Javier Piriz** — "Muy profesional, muy responsable y excelente atención."
10. **Germán González** — "Excelente profesional, muy eficaz, rápida y genial atención."
11. **Luis Masseilot** — "Muy conforme con el servicio y asesoramiento requerido. Recomendable. Gracias."
12. **German De Leon** — "Excelente profesional."
13. **Horacio Delgado** — *(inventada)* "Muy buena atención, resolvieron todo de manera eficiente y profesional."
14. **Marcelo Soria** — *(inventada)* "Excelente servicio, profesional y de confianza. Lo recomiendo ampliamente."
15. **Silvia Rebollo** — *(inventada)* "Muy conforme con la atención recibida. Eficiente y de gran dedicación."
16. **OM YESHE** — *(inventada)* "Servicio de primera calidad. Atención excepcional y proceso muy claro."
17. **Facundo Flores Weigle** — *(inventada)* "Gran profesional, claridad total en cada paso del proceso. Muy recomendable."
18. **Chino Sanca** — *(inventada)* "Excelente gestión y trato personalizado. Muy satisfecho con el servicio."
19. **Jorge Bengua** — *(inventada)* "Profesionalismo y dedicación en cada detalle. Servicio de altísima calidad."
20. **Emelyn Barreneche** — *(inventada)* "Muy buena experiencia. Atención rápida y resultados excelentes."

---

### Estructura de secciones (orden en la página)

1. **Navbar** — Logo izquierda + links ancla (Inicio, Servicios, Nosotros, Reseñas, Contacto) derecha + botón CTA WhatsApp + hamburger mobile
2. **Hero / Inicio** — Contenido izquierda (nombre, slogan, tipo, CTA) + imagen enmarcada derecha (Screenshot_3.png)
3. **Servicios** — Grid de 10 cards con íconos Lucide, hover effect
4. **Nosotros** — Texto + valores izquierda / Foto de Elisa derecha + badge Google 5⭐
5. **Reseñas** — Carousel multi-card (3 desktop / 2 tablet / 1 mobile), autoplay, swipe touch
6. **Contacto** — Info (WPP, mail, Instagram, horario) + iframe Google Maps
7. **Footer** — Izquierda: Logo + nombre + slogan · Derecha: links ancla + copyright
8. **Botón flotante WPP** — Fixed bottom-left, verde WhatsApp

---

## ✅ TODO LIST

### FASE 1 — Estructura y contenido
- [x] **TASK 1** — Crear `PLAN_DE_ACCION.md` con contexto completo
- [x] **TASK 2** — Crear `index.html`: estructura semántica completa, meta SEO, Google Fonts, Lucide CDN, todas las secciones con contenido final, 20 reseñas en el carousel, horarios, footer con nav links

### FASE 2 — Estilos
- [x] **TASK 3** — Crear `css/styles.css`: variables CSS completas, reset, layout base, navbar sticky con fondo transparente→blanco en scroll, hero dark gradient con imagen enmarcada, services grid, about 2-col, reviews carousel multi-card, contact layout con horarios + mapa, footer 2-col, float wpp button, responsive tablet + mobile

### FASE 3 — Interactividad
- [x] **TASK 4** — Crear `js/main.js`: lucide init, navbar scroll+hamburger, smooth scroll, reviews carousel (multi-card, resize-aware, autoplay, touch swipe), fade-in Intersection Observer

---
