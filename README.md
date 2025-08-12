# DeepRead AI: Asistente de Lecto-comprensión

DeepRead AI es una aplicación web estática que convierte cualquier libro en formato EPUB en un entorno interactivo de lecto-comprensión potenciado por IA. Ofrece herramientas para explorar y estudiar el contenido de manera más eficiente.

## Características

- **Carga de EPUB**  
  Permite seleccionar y cargar un archivo `.epub` desde el navegador.  
- **Vista de Contenido**  
  Navega por el índice de capítulos y selecciona el capítulo que deseas estudiar.
- **Resumen Automático**  
  Genera un resumen conciso en español del texto seleccionado usando Google AI Studio (Gemini).
- **Extracción de Conceptos Clave**  
  Extrae de 3 a 5 ideas o conceptos principales del capítulo.
- **Cuestionario Interactivo**  
  Crea un cuestionario de 10 preguntas de opción múltiple con explicaciones para reforzar la comprensión.
- **Mapa Mental**  
  Presenta el índice del libro como un mapa mental interactivo (conceptual o estructural) con distintos niveles de profundidad.
- **Chat Inteligente**  
  Chat contextual basado en el texto del capítulo, con opción de extender la consulta a conocimiento general.
- **Persistencia en el Navegador**  
  Guarda la API key de Google AI Studio y los resultados de IA en `localStorage` para minimizar llamadas repetidas.

## Tecnologías

- **HTML5** y **Tailwind CSS**  
- **JavaScript**: 
  - [epub.js](https://github.com/futurepress/epub.js) para procesar archivos EPUB  
  - [jszip](https://stuk.github.io/jszip/) para descompresión interna  
  - [D3.js](https://d3js.org/) y [Markmap](https://markmap.js.org/) para visualizar mapas mentales  
- **Google Generative Language API** (Gemini) para generación de contenido y cuestionarios  
- **LocalStorage** para persistencia de clave API y cache de respuestas IA

## Uso

1. Clona el repositorio:
   ```sh
   git clone https://github.com/jlopezf8/Ebook-Assistant.git
   cd Ebook-Assistant
   ```
2. Abre https://jlopezf8.github.io/Ebook-Assistant/ en tu navegador preferido.
3. Ingresa tu API Key de Google AI Studio.
4. Carga un archivo `.epub` y comienza a explorar.

## API Key

1. Obtén una clave de Google AI Studio en:  
   https://aistudio.google.com/app/apikey  
2. Pégala en el campo de ingreso, se almacenará solo en tu navegador.

## Licencia

Proyecto de código abierto bajo la [MIT License](LICENSE).
