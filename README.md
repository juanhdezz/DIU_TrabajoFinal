# Executive Summary

La página web de Salamanca Film Commission cumple adecuadamente con su función informativa, ofreciendo recursos valiosos para profesionales del sector audiovisual interesados en rodar en Salamanca. Sin embargo, presenta áreas de mejora en cuanto a **diseño visual**, **accesibilidad** y **experiencia de usuario**. La navegación es funcional, pero podría beneficiarse de una arquitectura de información más intuitiva y un diseño responsive optimizado. Se recomienda una revisión integral basada en principios de UX y accesibilidad para mejorar la eficacia y la satisfacción del usuario.

---

## Análisis Individual Profundo

### Diseño Visual y Coherencia Estética

El sitio utiliza una paleta de colores sobria y una tipografía legible, lo que facilita la lectura del contenido. Sin embargo, la estética general es algo anticuada, con un diseño que no refleja las tendencias actuales en diseño web. La coherencia visual entre las diferentes secciones es aceptable, aunque la inclusión de más elementos visuales, como imágenes de alta calidad y vídeos, podría enriquecer la experiencia del usuario.

### Usabilidad y Navegación Intuitiva

La estructura del menú principal es clara, con categorías bien definidas como "Localizaciones", "Rodar en Salamanca" y "Noticias". No obstante, la navegación podría mejorarse mediante la implementación de **breadcrumbs** y un **buscador interno** para facilitar el acceso a la información. Además, algunos enlaces requieren múltiples clics para acceder a la información deseada, lo que puede afectar la eficiencia de la navegación.

Para un análisis más profundo de la usabilidad, y siguiendo las directrices del "Tema 5 Usabilidad", se podrían aplicar diversas técnicas de evaluación. La usabilidad se enfoca en la facilidad con la que los usuarios pueden aprender a usar un sistema, su eficiencia al usarlo, la facilidad para recordar cómo usarlo, la propensión a errores y la satisfacción subjetiva.

Dada la necesidad de un análisis más exhaustivo, se proponen las siguientes técnicas que, por motivos de tiempo en esta revisión inicial, quedan pendientes de realización:

* **Evaluación heurística:** Como se menciona en el PDF (p. 26), esta técnica permite identificar problemas de usabilidad al comparar la interfaz con un conjunto de principios reconocidos (heurísticas). Podría ser realizada por expertos en usabilidad para detectar fallos de diseño que impactan directamente en la eficiencia y satisfacción del usuario. Se podrían aplicar heurísticas de Nielsen como la visibilidad del estado del sistema, el control y libertad del usuario, y la prevención de errores.
* **Test de usuarios (think-aloud protocol):** Aunque más consumidor de tiempo, la observación directa de usuarios reales interactuando con la página (como se describe en el PDF, p. 43) revelaría problemas de navegación y comprensión que no son evidentes para los desarrolladores o evaluadores expertos. Se les pediría a los participantes que piensen en voz alta mientras realizan tareas específicas en la web.
* **Encuestas de satisfacción (SUS - System Usability Scale):** Tras la interacción de los usuarios con la web, una encuesta estandarizada como el SUS (mencionado en el PDF, p. 57) proporcionaría una medida cuantitativa de la satisfacción subjetiva, permitiendo comparar la usabilidad percibida con benchmarks.

La implementación de estas técnicas permitiría obtener una visión más completa de los problemas de usabilidad, validando las observaciones iniciales y descubriendo otros aspectos críticos que podrían estar afectando la experiencia del usuario.

### Accesibilidad (WCAG Guidelines)

Según el análisis de la herramienta WAVE, la página presenta deficiencias en accesibilidad, a pesar de reportar un pase en WCAG AA y AAA.

**Errores de Contraste:**
* Se detecta **1 error de contraste muy bajo**, lo que dificulta la legibilidad para usuarios con baja visión. Es crucial revisar y ajustar la combinación de colores para asegurar un contraste adecuado entre el texto y el fondo.

**Alertas:**
* **No page regions (1):** Indica una falta de regiones de página (como `banner`, `main`, `navigation`, `contentinfo`), lo que puede dificultar la navegación para usuarios de lectores de pantalla.
* **Redundant link (8):** Se encontraron 8 enlaces redundantes. Esto puede generar confusión y frustración para los usuarios, especialmente aquellos que navegan con teclado o lectores de pantalla. Se recomienda consolidar o revisar estos enlaces.

**Características:**
* **Alternative text (12):** Aunque se identifican 12 textos alternativos, la presencia de errores de contraste y la falta de regiones de página sugieren que, si bien existen, su implementación podría no ser óptima o completa para todas las imágenes o elementos gráficos relevantes.
* **Linked image with alternative text (11):** Similar al punto anterior, se reconoce el uso de texto alternativo en imágenes con enlaces, lo cual es positivo, pero se debe verificar su precisión y utilidad para los usuarios de lectores de pantalla.
* **Language (1):** Se ha detectado la declaración del idioma, lo cual es una buena práctica de accesibilidad.
* **Heading level 1 (1):** La existencia de un encabezado de nivel 1 es fundamental para la estructura semántica de la página.

**ARIA:**
* **ARIA label (33):** Se utilizan 33 etiquetas ARIA, lo que es un buen indicativo de intentos de mejorar la accesibilidad para usuarios de lectores de pantalla. Sin embargo, la presencia de alertas como "No page regions" o "Redundant link" podría indicar que, a pesar de usar ARIA, su aplicación no resuelve completamente todos los problemas o que su uso no es siempre el más apropiado o eficiente. Es importante verificar que estas etiquetas sean precisas y útiles.
* **ARIA tabindex (15):** Se han implementado 15 `tabindex` ARIA. Esto puede ser útil para controlar el orden de tabulación, pero un uso excesivo o incorrecto puede generar problemas de navegación para los usuarios de teclado. Se debe asegurar que el orden de tabulación sea lógico y predecible.

En resumen, la página presenta deficiencias notables en contraste y estructura de regiones, así como redundancia en enlaces, a pesar de un esfuerzo en el uso de textos alternativos y atributos ARIA. Es fundamental abordar estas áreas para mejorar la experiencia de los usuarios con discapacidades visuales o que utilizan tecnologías de asistencia. Se recomienda una auditoría exhaustiva de la implementación de ARIA y una revisión del diseño para asegurar el cumplimiento total de las pautas WCAG.

### Responsive Design

El sitio es parcialmente responsive; se adapta a diferentes tamaños de pantalla, pero la experiencia en dispositivos móviles no está completamente optimizada. Algunos elementos, como menús desplegables y formularios, no funcionan adecuadamente en pantallas pequeñas, lo que puede frustrar a los usuarios móviles.

### Arquitectura de Información

La organización del contenido es lógica, pero podría beneficiarse de una jerarquía más clara y una mejor categorización. El sitemap del sitio, disponible en [https://octopus.do/wnknrzl2wo](https://octopus.do/wnknrzl2wo), clarifica la arquitectura de la información actual y ofrece una visión general de la estructura de la web.

Para optimizar y mejorar esta arquitectura, se podría aplicar la técnica de **Card Sorting**. Esta técnica (mencionada indirectamente en el PDF en el contexto de la organización de la información y categorización, aunque no con ese nombre explícito) permite a los usuarios organizar y agrupar el contenido de una manera que les resulte lógica e intuitiva. Por ejemplo, los usuarios podrían agrupar tarjetas que representen elementos como "Localizaciones", "Permisos de rodaje", "Noticias", "Contacto", etc., en categorías que ellos mismos definirían o que les serían preestablecidas. Esto ayudaría a validar o reestructurar las categorías existentes en la sección de "Localizaciones", subdividiéndolas en "Históricas", "Naturales" y "Urbanas" o en otras categorías que emerjan de la propia lógica del usuario.

Adicionalmente, el **Content Labeling** (etiquetado de contenido) es crucial. Esto implica asegurar que los nombres de las categorías y subcategorías sean claros, concisos y comprensibles para los usuarios. Un etiquetado efectivo facilita que los usuarios encuentren la información deseada sin ambigüedades. La combinación de un Card Sorting con una revisión de los Content Labeling puede generar una arquitectura de información más centrada en el usuario y, por ende, una navegación más intuitiva y eficiente. Por limitaciones de tiempo en esta fase, la realización de un estudio de Card Sorting y una revisión exhaustiva del Content Labeling quedan pendientes.

### Experiencia de Usuario (UX) ,Velocidad de Carga y Rendimiento

La experiencia de usuario es funcional pero carece de elementos interactivos que involucren al usuario. La implementación de funcionalidades como **mapas interactivos**, **recorridos virtuales** y **testimonios de producciones anteriores** podría mejorar significativamente la experiencia. Además, la inclusión de un **chatbot** o una sección de preguntas frecuentes más dinámica podría proporcionar asistencia inmediata a los usuarios.

La velocidad de carga es aceptable en conexiones de banda ancha, pero podría optimizarse significativamente. Para este análisis, se ha utilizado la herramienta **Google PageSpeed Insights**, que proporciona métricas detalladas y diagnósticos para mejorar el rendimiento web. Los resultados obtenidos (haciendo referencia a las imágenes `velocidad1.png` y `velocidad2.png` si estuvieran disponibles para una visualización más completa) revelan varias áreas de oportunidad:

**Diagnósticos Obtenidos:**

* **Evitar cambios de diseño importantes (15 cambios de diseño detectados):** Esto se refiere a "layout shifts" o cambios inesperados en el diseño de la página mientras se carga, lo que puede ser molesto para el usuario. Es crucial estabilizar los elementos durante la carga.
* **Habilita la compresión de texto (Ahorro potencial de 420 KiB):** La compresión GZIP o Brotli para archivos CSS, JavaScript y HTML puede reducir drásticamente el tamaño de los datos transferidos, mejorando la velocidad de carga.
* **Renderizado del mayor elemento con contenido (7000 ms):** Un tiempo de 7 segundos para que el elemento más grande de la página sea visible es considerable y puede generar una mala primera impresión en el usuario. Es fundamental optimizar la carga de este elemento crítico.
* **Reduce el contenido JavaScript que no se use (Ahorro potencial de 492 KiB):** Eliminar o aplazar la carga de código JavaScript que no es esencial para el contenido inicial reduce el tiempo de procesamiento y descarga.
* **Elimina los recursos que bloqueen el renderizado (Ahorro potencial de 1180 ms):** Archivos CSS y JavaScript que bloquean la renderización inicial deben ser optimizados para que no impidan que el contenido visible de la página se cargue rápidamente.
* **Minifica los recursos JavaScript (Ahorro potencial de 31 KiB):** Reducir el tamaño de los archivos JavaScript eliminando espacios en blanco y comentarios puede acelerar su descarga y parseo.
* **Publica imágenes con formatos de próxima generación (Ahorro potencial de 138 KiB):** Utilizar formatos de imagen modernos como WebP o AVIF en lugar de JPEG o PNG puede reducir el tamaño de los archivos sin sacrificar calidad.
* **Usa un tamaño adecuado para las imágenes (Ahorro potencial de 88 KiB):** Servir imágenes en las dimensiones exactas necesarias para el dispositivo del usuario evita la descarga de imágenes excesivamente grandes y luego escalarlas.
* **Reduce el contenido CSS que no se use (Ahorro potencial de 16 KiB):** Al igual que con JavaScript, eliminar CSS no utilizado puede reducir el tamaño de los archivos y mejorar el rendimiento.
* **No tiene una etiqueta `<meta name="viewport">` con width o initial-scale:** Esta etiqueta es crucial para asegurar que la página se adapte correctamente a diferentes tamaños de pantalla, especialmente en dispositivos móviles.
* **Precargar la imagen de renderizado del mayor elemento con contenido:** Indicar al navegador que priorice la carga de la imagen principal puede mejorar la velocidad de renderizado percibida.
* **Los elementos de imagen no tienen width y height explícitos:** Definir estas dimensiones ayuda a prevenir "layout shifts" y permite al navegador reservar espacio antes de que la imagen se cargue.
* **Minifica los archivos CSS (Ahorro potencial de 5 KiB):** Similar a JavaScript, minificar CSS reduce su tamaño.
* **Publica recursos estáticos con una política de caché eficaz (Se han encontrado 44 recursos):** Configurar políticas de caché adecuadas permite que los navegadores almacenen recursos estáticos localmente, evitando descargas repetidas.
* **Asegúrate de que el texto permanece visible mientras se carga la fuente web:** Evitar el "flash of unstyled text" (FOUT) o "flash of invisible text" (FOIT) mediante `font-display: swap` o técnicas similares.
* **No usa listeners pasivos para mejorar el desplazamiento:** Los "event listeners" pasivos pueden mejorar el rendimiento del desplazamiento, especialmente en dispositivos móviles.
* **Codifica las imágenes de forma eficaz (Ahorro potencial de 37 KiB):** Optimizar la calidad de compresión de las imágenes para encontrar un equilibrio entre tamaño de archivo y calidad visual.
* **Evitar document.write():** El uso de `document.write()` puede ralentizar el renderizado de la página.
* **Evita las animaciones no compuestas (2 elementos animados encontrados):** Las animaciones que no usan propiedades que pueden ser animadas directamente por el compositor del navegador pueden causar un rendimiento deficiente.
* **Evita encadenar solicitudes críticas (Se han encontrado 12 cadenas):** Reducir el número de recursos que deben cargarse secuencialmente para que la página sea interactiva.
* **Reducir el uso de código de terceros (El código de un tercero ha bloqueado el hilo principal durante 0 ms):** Aunque en este caso el bloqueo es de 0 ms, el diagnóstico resalta la importancia de monitorizar el impacto de scripts de terceros.
* **Evita tareas largas del hilo principal (1 tarea larga encontrada):** Tareas JavaScript largas pueden bloquear el hilo principal y hacer que la página no responda a la interacción del usuario.

La mejora de estas áreas de diagnóstico es crucial para optimizar la velocidad de carga y, por ende, la experiencia del usuario, especialmente en conexiones lentas o dispositivos móviles.

---

## Análisis Comparativo: Salamanca Film Commission vs. Film in Granada

### 1. Diseño Visual (Interfaz y Consistencia Estética)

| Criterio          | Salamanca Film Commission                                                                 | Film in Granada                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| :---------------- | :---------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Coherencia visual | Uso básico de colores planos y tipografías sin jerarquías marcadas. El diseño no transmite una narrativa visual clara. | Uso armónico de colores, tipografía consistente, buen contraste y elementos visuales alineados con el propósito cinematográfico.                                                                                                                                                                                                                                                                                                                                     |
| Identidad visual  | Escasa. El sitio se percibe como institucional sin rasgos diferenciales.                   | Fuerte identidad de marca. La estética comunica cultura visual y cine desde la portada.                                                                                                                                                                                                                                                                                                                                                                                          |
| Jerarquía visual  | Poco contrastada. No se distingue con claridad entre secciones principales y secundarias.   | Claramente estructurada. Las llamadas a la acción y títulos jerarquizados facilitan la lectura escaneada.                                                                                                                                                                                                                                                                                                                                                                        |

**Valoración general:**
→ Film in Granada está mejor diseñado visualmente. Aplica principios de diseño emocional y affordance visual (Law of Common Region y Fitts’ Law de Laws of UX) que mejoran la percepción y orientación del usuario.

### 2. Organización de Tareas

| Criterio                                | Salamanca Film Commission                                                                                     | Film in Granada                                                                                                                                       |
| :-------------------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Claridad en objetivos del sitio         | El propósito del sitio y los servicios no están explícitamente destacados; el usuario debe explorar para comprender. | El objetivo del sitio y su utilidad para productoras se entiende desde el primer vistazo gracias a textos directos e imágenes con contexto.            |
| Estrategia de llamadas a la acción      | Pocas llamadas visibles; enlaces textuales sin diseño prominente ni orientación a la acción.                  | Botones visuales prominentes con verbos orientados a tarea (“Solicita tu rodaje”, “Explora localizaciones”).                                         |
| Segmentación de perfiles de usuario     | No hay diferenciación clara entre usuarios como productores, técnicos o gestores institucionales.             | Presenta accesos diferenciados o información contextual para diferentes tipos de usuarios (guías, formularios, directorios específicos).             |

**Valoración general:**
→ Film in Granada presenta una organización de tareas más efectiva, guiando al usuario con intención clara. Aplica los principios de reconocimiento sobre memorización (heurística de Nielsen) y facilita la acción mediante un diseño proactivo.

### 3. Arquitectura de la Información

| Criterio                      | Salamanca Film Commission                                                                 | Film in Granada                                                                                                          |
| :---------------------------- | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------ |
| Estructura del menú principal | Menú simple pero poco jerárquico. Las categorías carecen de subniveles bien definidos.     | Menú con estructura lógica, jerarquía clara y agrupación semántica orientada a tareas frecuentes del usuario.             |
| Profundidad de navegación     | Contenidos clave requieren más de 3 clics. Algunos accesos están ocultos en subpáginas.    | La mayoría de tareas se pueden realizar en 2 clics. Buena accesibilidad desde la portada a secciones operativas clave.   |
| Etiquetado y nomenclatura     | Uso de términos genéricos (“Rodar en Salamanca”) sin indicaciones funcionales.             | Etiquetas claras, orientadas a objetivos (“Cómo rodar”, “Guía profesional”, “Rodado en Granada”) con lenguaje directo.   |

**Valoración general:**
→ Film in Granada cuenta con una arquitectura de información más clara, profunda y eficiente. Refuerza la orientación del usuario mediante rutas de acceso optimizadas y nomenclatura alineada a la lógica de tareas.

### 4. Flujo de Navegación

| Criterio                       | Salamanca Film Commission                                                                 | Film in Granada                                                                                                             |
| :----------------------------- | :---------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------- |
| Nivel de orientación           | No dispone de migas de pan (breadcrumbs); los retornos requieren uso del navegador.       | Incluye breadcrumbs y menús contextuales. Facilita saber en qué sección se encuentra el usuario y cómo volver.              |
| Fluidez del recorrido          | Navegación algo fragmentada; no siempre existe un recorrido continuo ni enlaces contextuales. | Flujo coherente, sin callejones sin salida. Todas las rutas tienen retornos claros y continuidad temática.                  |
| Compatibilidad y adaptación móvil | Adaptación parcial; algunos menús no son totalmente funcionales en dispositivos móviles.  | Responsive completo; navegación optimizada para móvil con menús colapsables y botones de tamaño adecuado para pulsación.     |

**Valoración general:**
→ Film in Granada proporciona un flujo de navegación más fluido, coherente y accesible en distintos dispositivos. Reduce la carga cognitiva (Hick’s Law) y mejora la orientación contextual del usuario mediante navegación guiada.

---
