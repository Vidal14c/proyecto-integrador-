Vocare 💊🗣️

Asistente Médico Inteligente por Voz (Voice-First SPA)
Proyecto Integrador | Tecnologías Emergentes en Interfaces de Usuario
Estudiante: Arturo Contreras | Institución: ISPADE

🌟 Descripción del Proyecto

Vocare es una aplicación web interactiva desarrollada bajo el paradigma Voice-First (Primero la voz), orientada a resolver las barreras de accesibilidad digital (visuales, motrices y cognitivas) a las que se enfrentan los adultos mayores al gestionar sus tratamientos médicos.

Las interfaces médicas tradicionales dependen de textos pequeños, calendarios y menús complejos. Vocare elimina estas barreras sustituyendo los menús por una interfaz basada en reconocimiento de voz bidireccional, un diseño de alto contraste (Amarillo/Negro) y botones sobredimensionados.

🚀 Tecnologías Emergentes Implementadas

Web Speech API (VUI):

Speech-to-Text (STT): Captura y transcribe la voz natural del usuario mediante SpeechRecognition.

Text-to-Speech (TTS): Genera respuestas vocales humanizadas y pausadas para guiar al adulto mayor utilizando speechSynthesis.

Web Audio API: Generación de un oscilador de audio de 800Hz que emite un tono acústico (Bip) de confirmación antes de iniciar la escucha, resolviendo problemas de feedback sensorial detectados en pruebas UX.

Tailwind CSS: Maquetación responsiva (Mobile-First y soporte estricto de F12 para emulación móvil) y de muy alto contraste para superar problemas de presbicia y cataratas.

🛠️ Arquitectura y Tecnologías del Sistema

Frontend: Single Page Application (SPA) en Vanilla JavaScript (ES6+), HTML5 semántico y Tailwind CSS.

Backend (Arquitectura proyectada/servidor local): Servidor API REST desarrollado en Node.js con Express.

Base de Datos: Motor relacional MySQL para el almacenamiento seguro de recetas, diagnósticos y perfiles de pacientes.

📱 Demostración y Despliegue

Enlace a la Aplicación (Netlify): https://proyectointegradorac.netlify.app/

Prototipo local en código único: Ver archivo prototipo.html en este repositorio.

⚙️ Instrucciones de Instalación y Ejecución Local

Puedes probar el prototipo de dos formas:

Opción A: Ejecución Directa del Prototipo

Clona el repositorio o descarga el archivo prototipo.html.

Ábrelo directamente en tu navegador web (Google Chrome o Microsoft Edge recomendado).

Concede los permisos del micrófono cuando el navegador lo solicite.

Opción B: Ejecución con Servidor Local (VS Code)

Abre el proyecto en Visual Studio Code.

Instala la extensión Live Server.

Haz clic derecho sobre el archivo HTML y selecciona "Open with Live Server".

📋 Funcionalidades Clave

Panel Clínico Interactivo: Permite al cuidador registrar el nombre del paciente, su diagnóstico y añadir medicamentos de forma múltiple.

Asistente de IA Local (Reglas NLP): Botón inteligente que sugiere medicamentos automáticamente según la enfermedad ingresada (ej. Diabetes -> Metformina).

Feedback Multimodal: El sistema responde mediante voz sintetizada y simultáneamente escribe la respuesta en pantalla con tipografía gigante.
