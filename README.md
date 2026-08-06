# Mi Coach — Plan Personalizado

Coach de fitness individualizado en una sola página HTML (sin backend, sin instalación). Le das tu peso, talla, edad, sexo y objetivo, y te genera automáticamente un plan de **dieta, entrenamiento y suplementación** basado en literatura científica — luego lo sigues día a día desde el navegador.

## Cómo usarlo

Descarga o clona el repo y abre `index.html` directamente en tu navegador (celular o computadora). No requiere servidor ni conexión a internet para funcionar (salvo la tipografía de Google Fonts).

```
git clone https://github.com/josecruzadi/Cambio.git
```

Luego abre `Cambio/index.html` con doble clic o arrastrándolo al navegador, completa tu perfil en la primera pestaña y listo.

## Cómo genera tu plan

En la pestaña **🧑‍⚕️ Perfil** ingresas peso, talla, edad, sexo, nivel de actividad diaria, tu objetivo (perder grasa / ganar músculo / recomposición / mantener), días de entrenamiento por semana y preferencias alimenticias. Con eso la app calcula:

- **Calorías objetivo** — BMR con la fórmula de Mifflin-St Jeor × factor de actividad (TDEE), ajustado según tu objetivo (déficit ~15-25% para perder grasa, superávit ~10% para ganar músculo magro).
- **Macros** — proteína en g/kg escalada según objetivo (1.6-2.2 g/kg en mantenimiento/superávit, 2.3-3.1 g/kg en déficit para conservar músculo), grasas ~25% de las calorías (con piso mínimo por salud hormonal) y el resto en carbohidratos.
- **Rutina de entrenamiento** — genera un split según tus días disponibles: 3 días (Full Body), 4 días (Torso/Pierna A-B), 5-6 días (Push/Pull/Legs), repartido en la semana con descanso entre sesiones.
- **Suplementación sugerida** — dosis de creatina, cafeína y proteína en polvo calculadas con tu peso, más beta-alanina si tu objetivo o volumen de entrenamiento lo justifica.

Todas las fórmulas y rangos están citados a su estudio de origen en la pestaña **📚 Coach**.

## Pestañas

- **🧑‍⚕️ Perfil** — formulario inicial y resumen de tu plan generado (calorías, macros, rutina semanal, stack de suplementos). Se puede editar en cualquier momento.
- **🍗 Comidas** — tu meta diaria de macros, una calculadora de alimentos comunes (pollo, arroz, huevo, avena, atún, etc. con macros por 100g) para registrar cantidades exactas, y un formulario para comidas personalizadas.
- **🔥 Cardio** — atajos de cardio rápidos, registro personalizado y contador de pasos diarios.
- **🏋️ Gym** — tu rutina del día según el split generado, marca tus entrenamientos como completados y visualiza tu semana completa.
- **📏 Cuerpo** — gráfica de evolución de peso contra tu peso objetivo (si lo defines), historial y medidas corporales (cintura, brazos, piernas, etc.) cada 2 semanas.
- **📊 Resumen** — adherencia semanal contra tus metas personalizadas, kcal/proteína promedio, cardio total y exportación/importación de datos (JSON/CSV).
- **📚 Coach** — el porqué detrás de cada número: hipertrofia (volumen, frecuencia, RIR), pérdida de grasa (déficit, proteína, cardio), suplementos por nivel de evidencia y recuperación, cada punto citado a su paper (Schoenfeld, Pelland, Nunes, Morton, Helms, Kreider, Guest, Jäger, Grgic, Trexler).

## Datos y privacidad

Todo se guarda **localmente en tu navegador** (`localStorage`, con respaldo en cookie) — nada se envía a ningún servidor. Esto significa que:

- Tus datos, incluido tu perfil, son privados por diseño.
- Si cambias de navegador o dispositivo, tus datos no viajan automáticamente — usa **⬇️ Descargar mis datos (JSON)** en la pestaña Resumen para respaldarlos, y **📤 Importar respaldo** para restaurarlos en otro lugar.
- Si reemplazas el archivo `index.html` por una versión nueva (por ejemplo tras actualizar el repo), tus datos se conservan siempre que sea el mismo navegador y la misma ubicación de archivo.

## Aviso

El contenido de este coach es información educativa general basada en revisiones y meta-análisis científicos, no un reemplazo de asesoría médica o nutricional individualizada. Consulta a un profesional de salud antes de suplementar o hacer cambios grandes de dieta o entrenamiento.
