# Test Oposición Osakidetza — Conductor/a de Vehículos de Emergencias (OPE)

Aplicación web progresiva (**PWA**) para practicar la batería de oposiciones de Osakidetza (**300 preguntas de Temario Común** + **200 preguntas de Conductor/a de Emergencias**) y realizar simulacros cronometrados de **90 minutos** compuestos por **100 preguntas ordinarias + 10 preguntas de reserva**.

## Para qué sirve esta aplicación

- **Entrenamiento por temario y lotes:** Practica por bloques (*Temario Común*, *Conductor/a Emergencias* o mezclados), en modo secuencial por rangos/lotes o en modo aleatorio, eligiendo entre **Modo Estudio** (comprobación inmediata con explicación) y **Modo Examen**.
- **Simulacros oficiales (Modelos A y B · 90 minutos):** Cada modelo consta de **100 preguntas ordinarias + 10 preguntas de reserva** siguiendo el orden del examen a partir de las 300 + 200 preguntas.
- **Cómputo de 100 preguntas y reservas separadas:** La calificación sobre 10 y el porcentaje se calculan sobre las **100 preguntas ordinarias**. Las **10 preguntas de reserva** se contabilizan **aparte** y **no** sustituyen a ninguna ordinaria salvo que exista anulación de preguntas de las 100 (hasta un máximo de 10), en cuyo caso cada anulada se sustituye en orden por la reserva correspondiente.
- **Corrección de plantillas `.json` e historial:** Importa y comprueba plantillas de respuestas separadas en formato `.json`, revisa tus fallos o todas las respuestas, guarda tu historial de intentos en el navegador y exporta resultados.
- **Gestión protegida en Ajustes:** Zona protegida con código `112` para buscar, editar o restablecer preguntas y cargar baterías `.json` desde la carpeta `baterias/`.

## Contenido del repositorio

- `index.html`: Aplicación web progresiva completa con la lógica de estudio, simulacros de 100 preguntas + 10 reservas, corrección de plantillas, historial, exportación y zona protegida **Ajustes** (código `112`).
- `baterias/`: Carpeta con las baterías y recursos en `.json`:
  - `preguntas_temario_comun_001_300_completo.json`: 300 preguntas de *Temario Común*.
  - `CVE.json`: 200 preguntas de *Conductor/a de Emergencias*.
  - `osakidetza_modelo_a_preguntas.json` y `osakidetza_modelo_b_preguntas.json`: Preguntas de los Modelos A y B (100 ordinarias + 10 de reserva cada uno).
  - `plantilla_oficial_modelo_a.json`, `plantilla_oficial_modelo_b.json` y `plantilla_scan_118929.json`: Plantillas de respuestas en formato `.json`.
  - `manifest.json`: Configuración de baterías disponibles en la carpeta.

## Uso y despliegue

- Abre `index.html` directamente en el navegador o publícalo con **GitHub Pages** desde la rama `main`.
- En Android (Chrome), ábrelo mediante **GitHub Pages** o un servidor HTTP/HTTPS local (`npx serve`) y pulsa **Añadir a pantalla de inicio** para instalarlo como PWA.
