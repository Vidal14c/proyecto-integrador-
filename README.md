# proyecto-integrador-
Vocare - Asistente de Voz para Medicación

Proyecto Integrador | Tecnologías Emergentes en Interfaces de Usuario - ISPADE

Descripción General

"Vocare" es una aplicación web y móvil de un Asistente de Voz (Voice User Interface - VUI) diseñada específicamente para adultos mayores. El sistema permite gestionar los horarios de medicación mediante comandos de voz naturales, mitigando las barreras de accesibilidad visual y motriz (letras pequeñas y teclados complejos) comunes en este grupo demográfico.

Tecnologías Utilizadas

Frontend: HTML5, CSS3, JavaScript (Vanilla).

Estilos: Tailwind CSS (vía CDN) para un diseño de alto contraste y componentes accesibles.

Íconos: FontAwesome.

Tecnología Emergente (VUI):

Web Speech API (SpeechRecognition): Para convertir la voz del usuario en texto (Speech-to-Text).

Web Speech API (SpeechSynthesis): Para generar las respuestas habladas del sistema (Text-to-Speech).

Requisitos de Ejecución

Este prototipo ha sido diseñado para ejecutarse completamente en el lado del cliente (Navegador) sin requerir instalación de servidores complejos.

Navegador compatible: Google Chrome, Microsoft Edge, o Safari (Actualizados). Nota: Firefox no soporta nativamente Web Speech API sin configuraciones adicionales.

Hardware: Micrófono funcional y altavoces/auriculares.

Conexión a internet: Requerida, ya que las APIs de reconocimiento de voz del navegador a menudo utilizan servicios en la nube (ej. Google Cloud) por detrás.

Instalación y Uso

Clona o descarga este repositorio.

Abre el archivo vocare_app.html directamente en tu navegador (doble clic).

El navegador te pedirá permisos para usar el micrófono. Haz clic en "Permitir".

Toca el botón gigante del micrófono en el centro de la pantalla.

Escucha el "bip" e intenta decir: "¿Qué pastilla me toca?".

Estructura del Código

El proyecto sigue el principio de "Single-File Application" (para esta entrega de prototipo), dividiendo el archivo vocare_app.html en tres capas:

<head> y <style>: Importación de librerías (Tailwind) y animaciones personalizadas CSS (@keyframes pulse-ring).

<body> (UI):

view-home: Interfaz principal con el botón del micrófono y estado del texto.

view-history: Lista visual de medicamentos basada en heurísticas de usabilidad.

delete-modal: Capa de prevención de errores (Heurística).

<script> (Lógica VUI):

Gestión de eventos de reconocimiento de voz (recognition.onresult).

Función processVoiceCommand(text): Actúa como el procesador de lenguaje natural (NLP) simulado.

Función speak(text): Invoca la síntesis de voz.

Consideraciones de Accesibilidad (UX Implementada)

Basado en las evaluaciones heurísticas realizadas durante la asignatura:

Feedback visual y sonoro: El micrófono cambia de color (rojo pulsante) y emite un "bip" para indicar que está escuchando.

Botones XXL: Diseñados para usuarios con temblores o presbicia.

Altos contrastes: Uso de textos oscuros sobre fondos blancos y amarillos claros (Cumplimiento WCAG AA).

Recuperación de errores: Modal de advertencia antes de borrar un medicamento.

Limitaciones Conocidas

El procesamiento de lenguaje natural (NLP) en este prototipo está simulado con condicionales simples (if/else). En un entorno de producción, requeriría integración con servicios como Dialogflow o AWS Lex.

La lista de medicamentos está estática en el frontend. La versión final conectaría con Firebase Firestore.
