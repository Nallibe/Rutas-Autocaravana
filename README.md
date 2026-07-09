# 🚐 Viajes de Sunny - Planificador de Rutas en Autocaravana

> **Planificador de rutas inteligente para viajes en autocaravana. Calcula distancias, peajes, consumo de combustible y gestiona tus paradas con opciones de rutas alternativas.**

🌐 **[Accede aquí →](https://nallibe.github.io/Rutas-Autocaravana/)**

---

## 📋 Tabla de Contenidos

- [Características](#características)
- [Novedades Recientes](#novedades-recientes)
- [Cómo Usar](#cómo-usar)
- [Guía de Rutas](#guía-de-rutas-alternativas)
- [Stack Técnico](#stack-técnico)
- [Instalación Local](#instalación-local)
- [Viajes Predefinidos](#viajes-predefinidos)
- [APIs Utilizadas](#apis-utilizadas)
- [Autor](#autor)

---

## ✨ Características

### 🗺️ Mapa Interactivo
- Mapa en tiempo real con Leaflet + OpenStreetMap
- Marcadores de paradas, ferrys y puntos opcionales
- Visualización de rutas por carretera (cálculo automático con OSRM)
- GPS en vivo: sigue tu ubicación en el mapa

### 📍 Planificación de Paradas
- **19 paradas predefinidas** en la ruta Italia (20 días)
- Información detallada por parada:
  - 🅿️ **Aparcamientos** (gratis o de pago)
  - 🏕️ **Campings** con web, teléfono y precio
  - ⛽ **Precios de gasolina** por zona
  - 🎥 **Enlaces a vídeos** (YouTube)
  - 🧭 **Navegación GPS** a cada parada

### 💰 Presupuesto Detallado
- **Distancia total**: calculada automáticamente
- **Peajes**: editables por tramo
- **Combustible**: estimado según consumo y precio
- **Ferry**: Civitavecchia → Barcelona (~520€)
- **Costo total del viaje**

### 🛣️ Rutas Alternativas (NUEVO)
- **Múltiples opciones de ruta** entre cada parada
- **Selecciona la que prefieras**: rápida, económica o escénica
- **Info de cada ruta**: distancia, tiempo, consumo
- Similar a Google Maps

### 🎯 Gestión de Paradas (NUEVO)
- ✏️ **Editar paradas**: cambiar nombre, ubicación, servicios
- ➕ **Insertar nuevas paradas**: entre cualquier dos puntos
- ⏭️ **Saltar paradas**: ir directamente al siguiente (eliminar intermedias)
- 🗑️ **Eliminar rutas**: quita una parada sin perder el resto
- 🔄 **Reorganización automática**: los días se renumeran automáticamente

### 🚨 Alertas y Seguridad
- **Alertas de tráfico**: búsqueda en tiempo real de incidentes
- **Alertas meteorológicas**: lluvia, nieve, hielo, temperaturas extremas
- **Consejos de viaje**: ZTL en Italia, costa Amalfitana, peajes, vignettes

### 💾 Multi-Viaje
- Crea varios viajes (Italia, Portugal, Francia, etc.)
- **Exporta/Importa** viajes en JSON
- **Guarda automáticamente** en LocalStorage
- Restaura la ruta original con un click

---

## 🆕 Novedades Recientes

### Modal Mejorado (v1.1)
✅ **Pantalla completa**: edita paradas sin scroll problemático  
✅ **Botón X**: cierra rápidamente  
✅ **Deslizable**: arrastra hacia abajo para cerrar (en móvil)  
✅ **Sin interferencias**: scroll independiente del mapa  

### Rutas Alternativas (v1.1)
✅ **Selecciona entre 3 rutas**: rápida, económica, escénica  
✅ **Información clara**: km, tiempo, consumo estimado  
✅ **Visual intuitivo**: marca activa con color azul  

### Gestión de Paradas (v1.1)
✅ **⏭️ Saltar a siguiente**: elimina una parada intermediaria  
✅ **🗑️ Eliminar ruta**: quita la conexión entre dos puntos  
✅ **🔄 Reorganización automática**: D1, D2, D3... se actualizan solos  

---

## 🎮 Cómo Usar

### 1️⃣ Abre la Aplicación
```
https://nallibe.github.io/Rutas-Autocaravana/
```

### 2️⃣ Comienza tu Viaje
- Haz click en **"¡Zarpar! 🏴‍☠️"** para cerrar la portada
- Se cargará el mapa con 19 paradas (ruta Italia 20 días)

### 3️⃣ Explora el Mapa
- **Zoom**: rueda del ratón o dedos (móvil)
- **Desplazamiento**: arrastra el mapa
- **Parada**: haz click en cualquier marcador
- **Ver ruta completa**: botón verde **"Ver ruta"**

### 4️⃣ Edita tu Ruta
- Panel derecho → parada → **"✏️ Editar"**
- Cambia: nombre, ubicación, aparcamiento, camping, etc.
- Verás **rutas alternativas** entre esta parada y la siguiente
- Haz click **"Guardar cambios"**

### 5️⃣ Elige Ruta Alternativa
En el modal de edición:
- Bajo **"🛣️ Rutas disponibles"**
- Haz click en una ruta (ej: "Alt 2")
- Se marca en azul y se carga información
- Haz click **"Guardar cambios"**

### 6️⃣ Salta Paradas
- En el modal → **"⏭️ Saltar a siguiente"**
- Elimina la parada siguiente
- Viajas directamente de esta parada a la otra
- Los días se reorganizan automáticamente

### 7️⃣ GPS en Vivo
- Botón **"📍 GPS"** en la barra superior
- Tu ubicación se muestra en el mapa
- La autocaravana 🚐 te sigue en tiempo real
- Arrastra para dejar de seguir

### 8️⃣ Presupuesto
- Panel izquierdo → **"🗺️ Ruta"**
- Ve:
  - Total km
  - Número de días
  - Peajes totales
  - Coste de combustible estimado

### 9️⃣ Alertas de Tráfico
- Panel derecho → pestaña **"🚨 Tráfico"**
- Botón **"🔍 Buscar incidentes en mi ruta"**
- Detecta: obras, accidentes, controles
- Muestra alertas en el mapa

### 🔟 Exporta/Importa
- **Exportar**: botón **"Exportar"** (descarga JSON)
- **Importar**: botón **"Importar"** (carga un viaje guardado)
- Comparte rutas con amigos

---

## 🛣️ Guía de Rutas Alternativas

### ¿Cómo funcionan?

Cuando editas una parada, la app busca **automáticamente** 3 rutas alternativas usando OSRM:

1. **📍 Ruta recomendada** (más rápida por defecto)
2. **🔄 Alt 2** (ruta alternativa)
3. **🔄 Alt 3** (otro camino)

### Información de cada ruta
```
🛣️ Ruta recomendada
   285 km · 4h 35 min
```

### Cómo cambiar de ruta
1. Haz click en la ruta que prefieres
2. Se marca en azul (activa)
3. Click **"Guardar cambios"** para confirmar
4. La ruta se actualiza en el mapa

### ¿Por qué son útiles?
- **Evita congestión**: elige ruta diferente si hay tráfico
- **Económica vs rápida**: compara peajes y distancia
- **Escénica**: algunas rutas pasan por lugares más bonitos
- **Como Google Maps**: familiar y fácil

---

## 📱 Stack Técnico

### Frontend
- **HTML5** + **CSS3** vanilla (sin frameworks)
- **JavaScript vanilla** (sin jQuery, React, Vue, etc.)
- **Leaflet.js** - mapas interactivos
- **OpenStreetMap** - tiles de mapa gratuitos

### APIs Externas (gratuitas)
- **OSRM** - cálculo de rutas y distancias
- **OpenStreetMap Nominatim** - geocodificación (nombre → coordenadas)
- **Overpass API** - búsqueda de incidentes de tráfico
- **OpenWeatherMap** - alertas meteorológicas

### Almacenamiento
- **LocalStorage** del navegador
- **JSON** para importar/exportar
- Sin servidor, 100% en el navegador

### Compatibilidad
- ✅ Escritorio (Chrome, Firefox, Safari, Edge)
- ✅ Móvil (iOS Safari, Chrome Mobile)
- ✅ Tablet (iPad, Android)
- ✅ Progressive Web App (funciona offline parcialmente)

---

## 💻 Instalación Local

### Opción 1: Servidor HTTP (Python)
```bash
cd roadtrip-italia
python -m http.server 8000
# Abre: http://localhost:8000
```

### Opción 2: Servidor HTTP (Node.js)
```bash
cd roadtrip-italia
npx http-server -p 8000
# Abre: http://localhost:8000
```

### Opción 3: Abrir directo
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

**Nota**: Algunas APIs requieren HTTPS en producción. Para desarrollo local usa HTTP.

---

## 🌍 Viajes Predefinidos

### 🇮🇹 Italia · 20 días (por defecto)
**Ruta**: Zaragoza → Girona → Niza → Turín → Milán → Verona → Venecia → Bolonia → Florencia → Siena → Pisa → Cinque Terre → Roma → Nápoles/Pompeya → Sorrento → Ferry → Barcelona → Zaragoza

**Características**:
- 19 paradas
- ~4.200 km de conducción
- Ferry Civitavecchia → Barcelona (20h)
- Campings y áreas verificadas
- Alertas de ZTL y Costa Amalfitana

**Crear nuevos viajes**:
- Botón **"＋ Viaje"** en la barra superior
- Introduce nombre y ciudad de salida
- La app geocodifica automáticamente
- Comienza con 1 parada, añade más

---

## 🔗 APIs Utilizadas

| API | Uso | Límite Gratuito |
|-----|-----|-----------------|
| **OSRM** | Rutas y distancias | Ilimitado |
| **Nominatim** | Geocodificación | 1 req/seg |
| **Overpass** | Incidentes de tráfico | 1 req/3seg |
| **OpenWeatherMap** | Clima en paradas | 1.000 req/día |
| **Leaflet + OSM** | Mapa | Ilimitado |

---

## ⚙️ Configuración

### En la pestaña "⚙️ Ajustes"

```
Consumo autocaravana (L/100 km): 12 (editable)
Precio medio combustible (€/L):  1.75 (editable)
Coste ferry (€):                  520 (editable)

Mostrar gasolineras:    ✓ (toggle)
Incluir peajes:         ✓ (toggle)
Mostrar paradas opcionales: ✓ (toggle)
```

### Precios de combustible por zona (editable)
| Zona | Precio |
|------|--------|
| España (fuera autopista) | €1.52 |
| Francia (hipermercado) | €1.72 |
| Francia (autoroute) | €1.92 |
| Italia · fai da te | €1.72 |
| Italia · servito | €1.90 |
| Italia · autostrada | €1.95 |

---

## 💡 Consejos de Uso

### ZTL (Zona Tráfico Limitado) en Italia
⚠️ Los centros históricos están CERRADOS para vehículos  
✅ Aparca SIEMPRE en las afueras (área/camping)  
✅ Usa transporte público o a pie  
❌ Entrar con camper = multa automática por cámara

### Costa Amalfitana (SS163)
❌ PROHIBIDA para autocaravanas de 7,5m  
✅ Aparca en Sorrento (camping)  
✅ Visita Positano/Amalfi en **bus SITA** o **ferry**

### Peajes en Italia
💳 Lleva **efectivo** y **tarjeta**  
🛣️ Considera un **Telepass** si haces muchos km  
🚐 Autocaravana = clase B/2 (más cara que coche)

### Repostaje en Italia
🍃 **"Fai da te"** (autoservicio) = más barato  
❌ **"Servito"** (con empleado) = evitar  
❌ Dentro de **autostrada** = caro  
✅ Gasolineras en **poblaciones** = mejor precio

### Pernocta
📱 Verifica en **[park4night.com](https://park4night.com)** (reseñas reales)  
📱 Verifica en **[CamperContact](https://www.campercontact.com)** (comunidad)  
🅿️ "Area di sosta" = área de servicio para autocaravanas

---

## 📞 Contacto / Soporte

- **GitHub**: [github.com/Nallibe/Rutas-Autocaravana](https://github.com/Nallibe/Rutas-Autocaravana)
- **Issues**: [Reporta bugs o sugiere mejoras](https://github.com/Nallibe/Rutas-Autocaravana/issues)
- **Email**: jnalliberg@gmail.com

---

## 📄 Licencia

Este proyecto es de **código abierto** bajo licencia MIT.

Puedes:
- ✅ Usar libremente
- ✅ Modificar y personalizar
- ✅ Compartir con amigos
- ✅ Crear tu propia versión

Solo pide crédito si lo compartes públicamente.

---

## 🙌 Créditos

**Autor**: Nallibe Rivera Grisale  
**Versión**: 1.1  
**Última actualización**: Julio 2025

### Librerias y Servicios
- 🗺️ [Leaflet.js](https://leafletjs.com/) - mapas
- 🌍 [OpenStreetMap](https://www.openstreetmap.org/) - tiles
- 🛣️ [OSRM](http://project-osrm.org/) - rutas
- 🔍 [Nominatim](https://nominatim.org/) - geocodificación
- 🚨 [Overpass API](https://overpass-api.de/) - incidentes
- 🌤️ [OpenWeatherMap](https://openweathermap.org/) - clima

---

## 🚀 Roadmap Futuro

- [ ] Importar rutas de Google Maps
- [ ] Histórico de viajes (estadísticas)
- [ ] Modo offline completo
- [ ] Integración con Booking/CamperContact
- [ ] Aplicación nativa (React Native)
- [ ] Compartir rutas en redes sociales
- [ ] Geocercas (alertas cuando llegas a paradas)

---

**¡Buen viaje! 🚐✨**

> "Viajar no es solo llegar al destino, es disfrutar del camino"
