# Mi Tracker — 90 Días

Tracker de fitness personal en una sola página HTML (sin backend, sin instalación). Registra comidas, cardio, entrenamientos de gym, peso corporal, medidas y consulta asesoría basada en literatura científica — todo desde el navegador.

## Cómo usarlo

Descarga o clona el repo y abre `index.html` directamente en tu navegador (celular o computadora). No requiere servidor ni conexión a internet para funcionar (salvo la tipografía de Google Fonts).

```
git clone https://github.com/josecruzadi/Cambio.git
```

Luego abre `Cambio/index.html` con doble clic o arrastrándolo al navegador.

## Pestañas

- **🍗 Comidas** — menú del plan con cantidades exactas, extras rápidos y registro de comidas personalizadas (kcal/proteína/carbos).
- **🔥 Cardio** — atajos de cardio del plan, registro personalizado y contador de pasos diarios.
- **🏋️ Gym** — rutina semanal (Torso A/B, Pierna A/B), marca tus entrenamientos como completados y visualiza tu semana.
- **📏 Cuerpo** — gráfica de evolución de peso, historial y medidas corporales (cintura, brazos, piernas, etc.) cada 2 semanas.
- **📊 Resumen** — adherencia semanal, kcal promedio, proteína promedio, cardio total y exportación/importación de datos (JSON/CSV).
- **📚 Coach** — asesoría basada en evidencia científica actual sobre hipertrofia, pérdida de grasa y suplementos, con una calculadora personalizada (proteína, creatina, cafeína) según tu peso registrado. Cada recomendación está citada a su estudio de origen (Schoenfeld, Pelland, Nunes, Morton, Helms, Kreider, Guest, Jäger, Grgic, Trexler).

## Datos y privacidad

Todo se guarda **localmente en tu navegador** (`localStorage`, con respaldo en cookie) — nada se envía a ningún servidor. Esto significa que:

- Tus datos son privados por diseño.
- Si cambias de navegador o dispositivo, tus datos no viajan automáticamente — usa **⬇️ Descargar mis datos (JSON)** en la pestaña Resumen para respaldarlos, y **📤 Importar respaldo** para restaurarlos en otro lugar.
- Si reemplazas el archivo `index.html` por una versión nueva (por ejemplo tras actualizar el repo), tus datos se conservan siempre que sea el mismo navegador y la misma ubicación de archivo.

## Aviso

El contenido de la pestaña Coach es información educativa general basada en revisiones y meta-análisis científicos, no un reemplazo de asesoría médica o nutricional individualizada. Consulta a un profesional de salud antes de suplementar o hacer cambios grandes de dieta o entrenamiento.
