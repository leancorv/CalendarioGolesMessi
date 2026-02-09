# 🔄 Cómo Actualizar los Datos

Esta guía explica cómo agregar nuevos goles al calendario cuando Messi marque.

## 📝 Método Simple: Editar CSV Local

Los datos del calendario se cargan desde el archivo `messi_goles.csv` en el repositorio.

### ✨ Pasos para actualizar:

1. **Edita el CSV**
   - Abre `messi_goles.csv` en tu editor favorito (VS Code, Excel, Google Sheets, etc.)
   - Inserta una nueva fila al **principio** (fila 2, justo después del header)

2. **Completa los datos**
   - Sigue el formato exacto del resto de filas
   - Ver formato detallado abajo ⬇️

3. **Guarda el archivo**
   - Asegúrate de guardar como CSV (UTF-8)

4. **Commit y Push**
   ```bash
   git add messi_goles.csv
   git commit -m "Agregar gol #897 - [fecha]"
   git push origin main
   ```

5. **¡Listo!**
   - GitHub Pages se actualiza automáticamente en 1-2 minutos
   - Refresca la página del calendario para ver el nuevo gol

## 📝 Formato de Datos

### Campos requeridos (en orden):
1. **Índice**: Número correlativo del gol (897, 898, 899...)
2. **Fecha**: Formato DD-MM-YYYY (ej: 23-11-2025)
3. **Equipo Local**: Nombre del equipo local
4. **Resultado**: Score final (ej: 0-4)
5. **Equipo Visitante**: Nombre del equipo visitante
6. **Marcador**: Score cuando hizo el gol (ej: 0-1)
7. **Tipo**: "Gol de campo", "Penal", "Tiro libre", "Solo run"
8. **Cómo**: "Pie izquierdo", "Pie derecho", "Cabeza"
9. **Competición**: Nombre de la competición
10. **Camiseta**: Número de camiseta (normalmente 10)
11. **Minuto**: Minuto del gol (ej: 19, 45+2, 90+6)
12. **Video**: URL de YouTube (opcional, deja vacío si no hay)

### Ejemplo de fila nueva:
```csv
897,25-02-2026,Real Madrid,1-3,Inter Miami CF,1-2,Gol de campo,Pie izquierdo,Amistoso Internacional,10,67,https://www.youtube.com/watch?v=XXXXX
```

## ⚠️ Importante

- **Orden**: Los goles más recientes van primero (orden descendente por índice)
- **Formato de fecha**: Estrictamente DD-MM-YYYY (con guiones, no slashes)
- **Sin comas extras**: Si un campo necesita comas, envuélvelo en comillas dobles
- **Video opcional**: Puedes dejar la columna vacía si no hay video disponible
- **Encoding**: Guarda el CSV como UTF-8 para mantener los caracteres especiales (tildes, ñ)

## 🐛 Troubleshooting

### El gol no aparece en el calendario
- **Verifica el formato de fecha**: Debe ser DD-MM-YYYY exactamente
- **Revisa las comas**: Debe haber exactamente 11 comas por fila
- **Espera**: GitHub Pages puede tardar 1-2 minutos en actualizar
- **Limpia caché**: Refresca con Ctrl+Shift+R (Windows) o Cmd+Shift+R (Mac)

### Error al cargar la página
- **Causa**: Probablemente hay un error de sintaxis en el CSV
- **Solución**: 
  - Verifica que todas las filas tengan la misma cantidad de columnas
  - Asegúrate de que las comillas estén balanceadas
  - Usa un validador de CSV online si no encuentras el error

### Los caracteres especiales se ven mal (ñ, á, é, etc.)
- **Causa**: El archivo no está guardado en UTF-8
- **Solución**:
  - VS Code: Abajo a la derecha click en "UTF-8" → "Save with Encoding" → "UTF-8"
  - Excel: "Guardar como" → Tipo: "CSV UTF-8 (delimitado por comas)"

## 💡 Tips

✅ **Usa un editor de texto**: VS Code o Sublime son mejores que Excel para CSVs  
✅ **Verifica antes de commitear**: Abre index.html localmente para probar  
✅ **Commit descriptivo**: Usa mensajes claros como "Agregar gol #897 vs Real Madrid"  
✅ **Backup**: GitHub guarda historial, pero no está de más tener un backup  

## 📞 Ayuda

Si tienes problemas:
1. Verifica el formato del CSV con un validador online
2. Compara tu nueva fila con las filas existentes
3. Revisa la consola del navegador (F12) para errores
4. Abre un [issue en GitHub](https://github.com/leancorv/CalendarioGolesMessi/issues) con:
   - Descripción del problema
   - La fila que estás intentando agregar
   - Screenshot del error (si aplica)

Los datos del calendario se cargan automáticamente desde [este Google Sheet](https://docs.google.com/spreadsheets/d/1-MQcfFuBED9VTE1vsruclxFfYNlSkQmf422NaY7Xb84/edit?usp=sharing).

### ✨ Pasos para actualizar:

1. **Abre el Google Sheet**
   - Click en el [link del Google Sheet](https://docs.google.com/spreadsheets/d/1-MQcfFuBED9VTE1vsruclxFfYNlSkQmf422NaY7Xb84/edit?usp=sharing)
   - (Necesitas permisos de edición - contacta al owner si no los tienes)

2. **Agrega el nuevo gol**
   - Inserta una nueva fila al principio (fila 2, después del header)
   - Completa todos los campos siguiendo el formato

3. **Guarda**
   - Los cambios se guardan automáticamente en Google Sheets

4. **¡Listo!**
   - Refresca la página del calendario
   - El nuevo gol aparecerá automáticamente
   - **No necesitas tocar código ni hacer commits**

## 📝 Formato de Datos

### Campos requeridos (en orden):
1. **Índice**: Número correlativo del gol (897, 898, 899...)
2. **Fecha**: Formato DD-MM-YYYY (ej: 23-11-2025)
3. **Equipo Local**: Nombre del equipo local
4. **Resultado**: Score final (ej: 0-4)
5. **Equipo Visitante**: Nombre del equipo visitante
6. **Marcador**: Score cuando hizo el gol (ej: 0-1)
7. **Tipo**: "Gol de campo", "Penal", "Tiro libre", "Solo run"
8. **Cómo**: "Pie izquierdo", "Pie derecho", "Cabeza"
9. **Competición**: Nombre de la competición
10. **Camiseta**: Número de camiseta (normalmente 10)
11. **Minuto**: Minuto del gol (ej: 19, 45+2, 90+6)
12. **Video**: URL de YouTube (opcional, deja vacío si no hay)

### Ejemplo de fila nueva:
```
897 | 25-02-2026 | Real Madrid | 1-3 | Inter Miami CF | 1-2 | Gol de campo | Pie izquierdo | Amistoso Internacional | 10 | 67 | https://www.youtube.com/watch?v=XXXXX
```

## 🔧 Configuración Técnica

### URL del Google Sheet
```
Sheet ID: 1-MQcfFuBED9VTE1vsruclxFfYNlSkQmf422NaY7Xb84
Export URL: https://docs.google.com/spreadsheets/d/1-MQcfFuBED9VTE1vsruclxFfYNlSkQmf422NaY7Xb84/export?format=csv&gid=0
```

### Permisos necesarios
- El Google Sheet debe estar configurado como "Cualquier persona con el enlace puede ver"
- Para editar necesitas permisos de editor

### Si cambias el Google Sheet ID
Edita el archivo `index.html` y actualiza la constante:
```javascript
const GOOGLE_SHEET_URL = 'https://docs.google.com/spreadsheets/d/TU-NUEVO-SHEET-ID/export?format=csv&gid=0';
```

## ⚠️ Importante

- **Orden cronológico inverso**: Los goles más recientes van primero
- **Formato de fecha estricto**: DD-MM-YYYY (con guiones, no slashes)
- **Sin comas en los campos**: Si un campo necesita comas, envuélvelo en comillas dobles
- **Video opcional**: Puedes dejar la columna vacía si no hay video

## 🐛 Troubleshooting

### El calendario no carga
- **Causa**: El Google Sheet no es público
- **Solución**: 
  1. Abre el Sheet
  2. Click en "Compartir"
  3. Cambia "Acceso restringido" a "Cualquier persona con el enlace"
  4. Asegúrate que el rol sea "Lector"

### El gol no aparece en el calendario
- **Verifica el formato de fecha**: Debe ser DD-MM-YYYY
- **Revisa las comas**: Asegúrate de que haya exactamente 11 comas por fila
- **Refresca con cache limpio**: Ctrl+Shift+R (Windows) o Cmd+Shift+R (Mac)

### Error "Failed to fetch"
- **Causa**: Problemas de CORS o permisos
- **Solución**: Verifica que el Sheet sea público y que la URL de export sea correcta

### Los datos se ven mal
- **Causa**: Caracteres especiales o saltos de línea
- **Solución**: Envuelve los campos problemáticos en comillas dobles

## 💡 Ventajas de Google Sheets

✅ **Sin código**: Actualiza datos sin tocar el código  
✅ **Tiempo real**: Los cambios se reflejan inmediatamente  
✅ **Colaborativo**: Múltiples personas pueden actualizar  
✅ **Historial**: Google Sheets guarda versiones anteriores  
✅ **Accesible**: Edita desde cualquier dispositivo  
✅ **No necesitas Git**: Cero commits para actualizar datos  

## 📞 Ayuda

Si tienes problemas:
1. Verifica que el Google Sheet sea público
2. Refresca la página con caché limpio
3. Revisa la consola del navegador (F12) para errores
4. Abre un [issue en GitHub](https://github.com/leancorv/CalendarioGolesMessi/issues) con:
   - Descripción del problema
   - Screenshot del error (si aplica)
   - La fila que estás intentando agregar
