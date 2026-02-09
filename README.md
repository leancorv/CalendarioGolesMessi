# ⚽ Cada Día con Messi - Calendario de Goles

Un calendario interactivo que muestra todos los días del año en los que Lionel Messi ha marcado goles a lo largo de su carrera. ¿Hizo Leo un gol el día de tu cumpleaños? ¡Descúbrelo!

## 🌟 Demo

👉 **[Ver Demo en Vivo](https://leancorv.github.io/CalendarioGolesMessi/)**

![Preview del Calendario](preview.png)

## ✨ Características

- 📅 **Calendario anual único**: Visualiza los 365 días del año
- ⚽ **896+ goles documentados**: Cada gol de la carrera de Messi
- 🎯 **284+ días con goles**: Más del 75% del año tiene al menos un gol
- 🎬 **Links a videos**: Ver los goles directamente en YouTube
- 📱 **Responsive**: Funciona perfectamente en móvil y desktop
- 🎨 **Diseño moderno**: Interfaz elegante con animaciones suaves
- ⚡ **Ultra rápido**: Vanilla JavaScript, sin frameworks pesados

## 🎯 Concepto

A diferencia de un calendario tradicional por año, este proyecto agrupa los goles **por día del año** (día y mes), sin importar el año. Por ejemplo:

- **5 de Marzo**: Muestra todos los goles que Messi marcó un 5 de marzo (2015, 2018, 2023, etc.)
- **19 de Septiembre**: ¡El día con más goles! 10 goles en diferentes años

Es como un "calendario de cumpleaños de goles" - perfecto para descubrir si Messi hizo magia el día de tu cumpleaños.

## 🚀 Cómo se Creó

Este proyecto fue desarrollado mediante **vibe coding** - un proceso colaborativo entre humano e IA:

### 🛠️ Stack Tecnológico
- **HTML5 + CSS3 + Vanilla JavaScript**: Sin frameworks, máxima performance
- **Google Fonts**: Bebas Neue y Outfit para una tipografía distintiva
- **Diseño responsivo**: CSS Grid y Flexbox
- **CSV local**: Datos en el repositorio para máxima simplicidad

### 🤖 Proceso de Desarrollo

1. **Recolección de datos** (Manual)
   - Limpieza de datos de múltiples fuentes
   - Verificación manual de información
   - Formato CSV estructurado

2. **Diseño UI/UX** (Claude + Gemini)
   - Prototipado rápido del concepto
   - Iteración de diseño visual
   - Optimización de experiencia de usuario

3. **Desarrollo** (Claude)
   - Parsing de CSV a estructura de datos optimizada
   - Renderizado dinámico del calendario
   - Sistema de modals interactivos
   - Animaciones y micro-interacciones

4. **Refinamiento** (Humano + IA)
   - Testing en diferentes dispositivos
   - Ajustes de diseño y copy
   - Optimización de performance

### 🧠 Herramientas Utilizadas
- **Claude (Anthropic)**: Desarrollo, diseño de interfaz, arquitectura
- **Gemini (Google)**: Asistencia en prototipado inicial
- **Limpieza manual de datos**: Verificación y corrección de información

## 📊 Datos

Los datos se cargan desde `messi_goles.csv` en el repositorio e incluyen:

- ✅ Fecha del gol
- ✅ Equipos (local y visitante)
- ✅ Resultado del partido
- ✅ Marcador cuando hizo el gol
- ✅ Tipo de gol (campo, penal, tiro libre)
- ✅ Cómo lo hizo (pie izquierdo, derecho, cabeza)
- ✅ Competición
- ✅ Minuto
- ✅ Link al video (cuando está disponible)

### 📁 Estructura de Datos

```csv
Índice,Fecha,Equipo Local,Resultado,Equipo Visitante,Marcador,Tipo,Cómo,Competición,Camiseta,Minuto,Video
896,23-11-2025,FC Cincinnati,0-4,Inter Miami CF,0-1,Gol de campo,Cabeza,Major League Soccer Play Offs,10,19,https://www.youtube.com/watch?v=...
```

## 🔄 Actualizar los Datos

Para agregar nuevos goles:

1. Edita `messi_goles.csv` con el nuevo gol
2. Commit y push al repositorio
3. GitHub Pages se actualiza automáticamente

Ver [UPDATING.md](UPDATING.md) para detalles completos.

## 🎨 Características de Diseño

- **Gradiente eléctrico**: Fondo azul vibrante que evoca el espíritu deportivo
- **Dorado para goles**: Color distintivo que resalta los días especiales
- **Modals elegantes**: Presentación limpia de información detallada
- **Animaciones sutiles**: Mejoran la experiencia sin distraer
- **Tipografía deportiva**: Bebas Neue para títulos impactantes

## 📱 Compatibilidad

- ✅ Chrome/Edge (últimas 2 versiones)
- ✅ Firefox (últimas 2 versiones)
- ✅ Safari (últimas 2 versiones)
- ✅ Dispositivos móviles (iOS y Android)

## 🚀 Deploy en Vercel

```bash
# Instalar Vercel CLI (si no lo tienes)
npm i -g vercel

# En la carpeta del proyecto
vercel

# Seguir las instrucciones
# ¡Listo! Tu sitio estará en vivo
```

O simplemente arrastra la carpeta a [vercel.com](https://vercel.com) para deploy instantáneo.

## 📈 Estadísticas del Proyecto

- **Goles totales**: 896+
- **Días únicos con goles**: 284+ de 365 (77.8%)
- **Día con más goles**: 19 de Septiembre (10 goles)
- **Años cubiertos**: 2004-2025
- **Líneas de código**: ~600 (HTML + CSS + JS)
- **Tamaño total**: ~380 KB (HTML + CSV)
- **Tiempo de carga**: < 1 segundo

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si encuentras algún error en los datos o tienes ideas para mejorar el proyecto:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

### 💡 Ideas para Contribuir

- [ ] Filtros por competición
- [ ] Gráficas de estadísticas
- [ ] Comparador de días
- [ ] Sistema de búsqueda
- [ ] Compartir en redes sociales
- [ ] Modo oscuro/claro
- [ ] Exportar estadísticas personales
- [ ] PWA (Progressive Web App)
- [ ] Agregar goles nuevos cuando Messi marque

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 🙏 Agradecimientos

- A Lionel Messi por ser una fuente inagotable de inspiración
- A la comunidad de fanáticos que documentan cada gol
- A Claude y Gemini por hacer posible el vibe coding
- A todos los que han contribuido con datos y feedback

## 📬 Contacto

Creado por [@leancorv](https://github.com/leancorv)

¿Preguntas o sugerencias? Abre un [issue](https://github.com/leancorv/CalendarioGolesMessi/issues)

---

⭐ Si te gustó el proyecto, ¡dale una estrella en GitHub!

**#Messi #WebDevelopment #VibeCoding #DataVisualization**

## 🌟 Demo

👉 **[Ver Demo en Vivo](https://leancorv.github.io/CalendarioGolesMessi/)**

![Preview del Calendario](preview.png)

## ✨ Características

- 📅 **Calendario anual único**: Visualiza los 365 días del año
- ⚽ **896+ goles documentados**: Cada gol de la carrera de Messi
- 🎯 **284+ días con goles**: Más del 75% del año tiene al menos un gol
- 🔄 **Actualización automática**: Conectado a Google Sheets
- 🎬 **Links a videos**: Ver los goles directamente en YouTube
- 📱 **Responsive**: Funciona perfectamente en móvil y desktop
- 🎨 **Diseño moderno**: Interfaz elegante con animaciones suaves
- ⚡ **Ultra rápido**: Vanilla JavaScript, sin frameworks pesados

## 🎯 Concepto

A diferencia de un calendario tradicional por año, este proyecto agrupa los goles **por día del año** (día y mes), sin importar el año. Por ejemplo:

- **5 de Marzo**: Muestra todos los goles que Messi marcó un 5 de marzo (2015, 2018, 2023, etc.)
- **19 de Septiembre**: ¡El día con más goles! 10 goles en diferentes años

Es como un "calendario de cumpleaños de goles" - perfecto para descubrir si Messi hizo magia el día de tu cumpleaños.

## 🚀 Cómo se Creó

Este proyecto fue desarrollado mediante **vibe coding** - un proceso colaborativo entre humano e IA:

### 🛠️ Stack Tecnológico
- **HTML5 + CSS3 + Vanilla JavaScript**: Sin frameworks, máxima performance
- **Google Sheets API**: Fuente de datos dinámica y fácil de actualizar
- **Google Fonts**: Bebas Neue y Outfit para una tipografía distintiva
- **Diseño responsivo**: CSS Grid y Flexbox

### 🤖 Proceso de Desarrollo

1. **Recolección de datos** (Manual)
   - Limpieza de datos de múltiples fuentes
   - Verificación manual de información
   - Migración a Google Sheets para actualizaciones fáciles

2. **Diseño UI/UX** (Claude + Gemini)
   - Prototipado rápido del concepto
   - Iteración de diseño visual
   - Optimización de experiencia de usuario

3. **Desarrollo** (Claude)
   - Integración con Google Sheets
   - Parsing de CSV a estructura de datos optimizada
   - Renderizado dinámico del calendario
   - Sistema de modals interactivos
   - Animaciones y micro-interacciones

4. **Refinamiento** (Humano + IA)
   - Testing en diferentes dispositivos
   - Ajustes de diseño y copy
   - Optimización de performance

### 🧠 Herramientas Utilizadas
- **Claude (Anthropic)**: Desarrollo, diseño de interfaz, arquitectura
- **Gemini (Google)**: Asistencia en prototipado inicial
- **Google Sheets**: Base de datos y gestión de contenido
- **Limpieza manual de datos**: Verificación y corrección de información

## 📊 Datos

Los datos se cargan automáticamente desde [este Google Sheet](https://docs.google.com/spreadsheets/d/1-MQcfFuBED9VTE1vsruclxFfYNlSkQmf422NaY7Xb84/edit?usp=sharing) e incluyen:

- ✅ Fecha del gol
- ✅ Equipos (local y visitante)
- ✅ Resultado del partido
- ✅ Marcador cuando hizo el gol
- ✅ Tipo de gol (campo, penal, tiro libre)
- ✅ Cómo lo hizo (pie izquierdo, derecho, cabeza)
- ✅ Competición
- ✅ Minuto
- ✅ Link al video (cuando está disponible)

## 🔄 Actualizar los Datos

**¡Ahora es súper fácil!** Solo edita el [Google Sheet](https://docs.google.com/spreadsheets/d/1-MQcfFuBED9VTE1vsruclxFfYNlSkQmf422NaY7Xb84/edit?usp=sharing):

1. Agrega una nueva fila con el gol
2. Guarda el cambio
3. Refresca la página del calendario
4. ¡El nuevo gol aparecerá automáticamente!

No necesitas tocar código ni hacer commits. Todo se actualiza en tiempo real.

### 📝 Formato de Datos

```
Índice | Fecha | Equipo Local | Resultado | Equipo Visitante | Marcador | Tipo | Cómo | Competición | Camiseta | Minuto | Video
```

Ver [UPDATING.md](UPDATING.md) para detalles completos.

## 🎨 Características de Diseño

- **Gradiente eléctrico**: Fondo azul vibrante que evoca el espíritu deportivo
- **Dorado para goles**: Color distintivo que resalta los días especiales
- **Modals elegantes**: Presentación limpia de información detallada
- **Animaciones sutiles**: Mejoran la experiencia sin distraer
- **Tipografía deportiva**: Bebas Neue para títulos impactantes

## 📱 Compatibilidad

- ✅ Chrome/Edge (últimas 2 versiones)
- ✅ Firefox (últimas 2 versiones)
- ✅ Safari (últimas 2 versiones)
- ✅ Dispositivos móviles (iOS y Android)

## 🚀 Deploy en Vercel

```bash
# Instalar Vercel CLI (si no lo tienes)
npm i -g vercel

# En la carpeta del proyecto
vercel

# Seguir las instrucciones
# ¡Listo! Tu sitio estará en vivo
```

O simplemente arrastra la carpeta a [vercel.com](https://vercel.com) para deploy instantáneo.

## 📈 Estadísticas del Proyecto

- **Goles totales**: 896+
- **Días únicos con goles**: 284+ de 365 (77.8%)
- **Día con más goles**: 19 de Septiembre (10 goles)
- **Años cubiertos**: 2004-2025
- **Líneas de código**: ~600 (HTML + CSS + JS)
- **Tamaño del archivo**: ~30 KB (sin datos embebidos)
- **Tiempo de carga**: < 1 segundo
- **Fuente de datos**: Google Sheets (actualización en tiempo real)

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si encuentras algún error en los datos o tienes ideas para mejorar el proyecto:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

### 💡 Ideas para Contribuir

- [ ] Filtros por competición
- [ ] Gráficas de estadísticas
- [ ] Comparador de días
- [ ] Sistema de búsqueda
- [ ] Compartir en redes sociales
- [ ] Modo oscuro/claro
- [ ] Exportar estadísticas personales
- [ ] PWA (Progressive Web App)

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 🙏 Agradecimientos

- A Lionel Messi por ser una fuente inagotable de inspiración
- A la comunidad de fanáticos que documentan cada gol
- A Claude y Gemini por hacer posible el vibe coding
- A Google Sheets por facilitar la gestión de datos
- A todos los que han contribuido con datos y feedback

## 📬 Contacto

Creado por [@leancorv](https://github.com/leancorv)

¿Preguntas o sugerencias? Abre un [issue](https://github.com/leancorv/CalendarioGolesMessi/issues)

---

⭐ Si te gustó el proyecto, ¡dale una estrella en GitHub!

**#Messi #WebDevelopment #VibeCoding #DataVisualization #GoogleSheets**
