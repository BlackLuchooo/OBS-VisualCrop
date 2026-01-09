# OBS Visual Crop

Interfaz web interactiva diseñada para la gestión visual de recortes (cropping) y zoom de fuentes en **OBS Studio**. Esta herramienta permite realizar ajustes precisos mediante manipulación directa sobre una previsualización, eliminando la configuración manual de parámetros numéricos en los filtros de OBS.

---

## Funciones Principales

* **Manipulación Visual Directa**: Define el área de interés moviendo un rectángulo interactivo sobre una previsualización en tiempo real.
* **Zoom Inteligente con Bloqueo de Aspecto**: Sistema de zoom relativo que mantiene las proporciones originales de la fuente, compensando automáticamente la escala en el lienzo de OBS.
* **Límites Dinámicos de Seguridad**: Algoritmo de protección que detecta los bordes de la imagen original para evitar recortes negativos o desbordamientos técnicos.
* **Monitor Resizable**: Contenedor de previsualización ajustable verticalmente para permitir trabajos de alta precisión en áreas pequeñas.
* **Memoria de Conexión**: Persistencia de credenciales (IP y Contraseña) mediante LocalStorage para reconexión automática.

---

## Requisitos Técnicos

* **OBS Studio**: Versión 28.0 o superior.
* **Protocolo**: OBS WebSocket v5.x (habilitado en `Herramientas` > `Ajustes de servidor WebSocket`).
* **Archivo**: `VisualCrop.html` guardado localmente en su ordenador.

---

## Guía de Instalación e Integración en OBS

Para una mejor experiencia, se recomienda integrar esta herramienta como un panel interno de OBS:

1.  **Obtener la ruta del archivo**: 
    * Localiza el archivo `VisualCrop.html` en tu carpeta.
    * Haz clic derecho sobre el archivo y selecciona "Copiar como ruta" (o ábrelo en tu navegador y copia la dirección que aparece en la barra de URL, que empezará por `file:///...`).
2.  **Crear el Panel en OBS**:
    * En OBS Studio, ve al menú superior `Paneles` (Docks) > `Paneles de navegador personalizados...`.
    * En **Nombre del panel**, escribe: `Visual Crop`.
    * En **URL**, pega la ruta que copiaste en el paso 1.
    * Haz clic en `Aplicar` y cierra la ventana.
3.  **Configuración Final**:
    * Aparecerá una nueva ventana flotante. Puedes arrastrarla y acoplarla en cualquier lugar de la interfaz de OBS.
    * Ingresa la IP y contraseña de tu servidor WebSocket.
    * **Selecciona cualquier fuente** en tu escena de OBS; la herramienta la detectará y calibrará los controles automáticamente.

---

## Metodología de Desarrollo

La herramienta opera bajo una arquitectura de comunicación asíncrona de baja latencia. El motor principal utiliza una lógica de **compensación de escala inversa**: cuando el usuario reduce el área visible (zoom in), el script calcula el factor de escala necesario para que la fuente mantenga su tamaño percibido en la composición final.

### Tecnologías utilizadas:
* **Lenguajes**: HTML5, CSS3, JavaScript (Vanilla).
* **API**: OBS-WebSocket JS (v5.x).
* **Sincronización**: ResizeObserver API para la interfaz adaptable.

---

### Créditos
Desarrollado por Blackluchooo.
