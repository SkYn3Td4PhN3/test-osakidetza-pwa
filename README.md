# Test Oposición Osakidetza — Conductor/a de Vehículos de Emergencias (OPE)

Aplicación web progresiva (**PWA**) en un único archivo (`index.html`) para practicar el banco de **500 preguntas** (**300 de Temario Común** + **200 de Conductor/a de Emergencias**) y realizar simulacros cronometrados de **90 minutos** (**100 preguntas ordinarias + 10 de reserva**, Modelos A y B).

## Contenido del repositorio

- `index.html`: Aplicación completa (`v2.0.2`) con modos de estudio y examen, cronómetro de 90 minutos, selección de preguntas para examen, historial de intentos y zona protegida **Ajustes** (código `112`) para gestionar preguntas e importar baterías `.json`.
- `preguntas_temario_comun_001_300_completo.json`: Batería de 300 preguntas de Temario Común.
- `CVE.json`: Batería de 200 preguntas específicas de Conductor/a de Emergencias.
- `baterias/`: Carpeta con la batería completa (`banco_500.json`), baterías separadas, preguntas de los modelos A y B, plantillas oficiales y `manifest.json`.

## Uso y despliegue

- Puedes abrir `index.html` directamente en el navegador o publicarlo mediante **GitHub Pages** desde la rama `main`.
- Para instalarlo como aplicación en Android desde Chrome, ábrelo mediante **GitHub Pages** o un servidor local HTTP/HTTPS (`npx serve`) y selecciona **Añadir a pantalla de inicio**.
