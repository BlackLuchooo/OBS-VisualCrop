OBS Visual Crop - ESPAÑOL
Esta es una herramienta web interactiva diseñada para gestionar el recorte y zoom de fuentes en OBS Studio de forma visual y precisa. VisualCrop.html actúa como una interfaz externa que elimina la necesidad de ajustar valores numéricos manualmente en los filtros de OBS.

Funciones Principales
Manipulación Visual Directa: Control mediante un rectángulo interactivo sobre una previsualización en tiempo real para definir el área de interés.

Zoom con Bloqueo de Aspecto: Sistema de acercamiento que mantiene la proporción original de la fuente, recalculando la escala de OBS automáticamente para mantener el tamaño en el lienzo.

Límites de Seguridad Dinámicos: Algoritmo de detección de bordes que impide recortes negativos o desbordamientos de parámetros que puedan romper la transformación.

Interfaz Adaptable: Área de trabajo ajustable verticalmente (resize) que permite ampliar el monitor de previsualización para realizar ajustes de alta precisión.

Persistencia de Datos: Almacenamiento local de credenciales (IP y contraseña) para permitir la conexión automática en futuras sesiones.

Guía de Inicio Rápido
Configuración en OBS:

Dirígete a Herramientas -> Ajustes de servidor WebSocket.

Habilita el servidor y anota la IP (127.0.0.1) y la contraseña.

Conexión:

Abre VisualCrop.html en cualquier navegador moderno.

Ingresa los datos de conexión y presiona Conectar.

Selecciona cualquier fuente dentro de tu escena de OBS haciendo clic sobre ella.

Ajustes:

Arrastra el recuadro verde para posicionar el recorte o utiliza los controles deslizantes para aplicar zoom relativo.

Notas de Desarrollo
Proyecto desarrollado por BlackLuchooo. Implementado con:

HTML5 / CSS3 (Sistema de UI adaptable).

JavaScript Vanilla.

OBS-WebSocket JS (Protocolo v5.x).

______________________________________________________________________________

OBS Visual Crop (English)
An interactive web tool designed to visually manage source cropping and zooming in OBS Studio. VisualCrop.html serves as an external interface that eliminates manual pixel entry in OBS filters.

Key Features
Direct Visual Control: Use an interactive bounding box over a real-time preview to define the crop area.

Aspect-Ratio Locked Zoom: Zooming system that preserves original source proportions by automatically recalculating the OBS scale.

Dynamic Safety Boundaries: Edge-detection algorithm that prevents negative values or parameter overflows from breaking the OBS transform.

Resizable Workspace: Vertically resizable preview area, allowing for high-precision adjustments by expanding the monitor.

Data Persistence: LocalStorage integration for credentials, enabling instant automatic reconnection in future sessions.

Quick Start Guide
OBS Setup:

Go to Tools -> WebSocket Server Settings.

Enable the server and note your IP (127.0.0.1) and password.

Connection:

Open VisualCrop.html in your web browser.

Enter your credentials and click Connect.

Click on any source inside your OBS scene to select it.

Adjustments:

Drag the green box to position the crop or use the sliders for relative zooming.

Tech Stack
Developed by Blackluchooo. Built using:

HTML5 / CSS3 (Adaptive UI system).

Vanilla JavaScript.


OBS-WebSocket JS (v5.x Protocol).
