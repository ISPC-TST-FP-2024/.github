# Bienvenido a la Formación Profesional: Desarrollador de Dispositivos IoT

Esta organización forma parte del dictado de la FP "Desarrollador de Dispositivos IoT" en el ISPC (Instituto Superior Politécnico de Córdoba), bajo la Dirección General de Educación Técnica y Formación Profesional del Ministerio de Educación de Córdoba.

## La Formación Profesional

El trayecto formativo de "Desarrollador de Dispositivos IoT" busca formar técnicos capacitados para desempeñarse en todas las capas del Internet de las Cosas (IoT), desarrollando, administrando y manteniendo proyectos de IoT. Esto implica:

- Desarrollo de dispositivos para el IoT
- Configuración y administración de redes IoT
- Integración y gestión de datos en sistemas IoT
- Implementación de medidas de seguridad en dispositivos y redes IoT

## Proyecto Central: Gestión y Monitoreo de Recursos Hídricos Locales

**Objetivo del Proyecto:**
Desarrollar un sistema de control y monitoreo distribuido para optimizar el uso y gestión del agua en diferentes entornos. Este controlador tipo célula es capaz de abarcar el control general y amplio de jardines, plazas, huertas urbanas, así como grandes plantaciones agrícolas en campos rurales. El sistema se enfoca en la eficiencia y sostenibilidad del riego mediante la gestión y monitoreo inteligente de los recursos hídricos locales.

**Componentes del Proyecto:**

**Hardware:**
- **Microcontroladores:** ESP32
- **Módulos de Comunicación:** LoRa
- **Sensores:** Humedad del suelo, pH, lluvia, temperatura, etc.
- **Actuadores:** Bombas, sistemas de iluminación, motores de posicionamiento

**Software:**
- **IDE y Herramientas de Desarrollo:** VSCode, PlatformIO, Git, GitHub
- **Lenguajes de Programación:** C++, Arduino framework
- **Metodologías:** ABP (Aprendizaje Basado en Proyectos), Kanban, Scrum, Agile

**Protocolos de Comunicación:**
- **UART, SPI, I2C:** Comunicación entre sensores y microcontroladores
- **WiFi/Bluetooth:** Conectividad para ESP32
- **MQTT:** Protocolo de comunicación para IoT
- **HTTP/HTTPS:** Integración con servidores web y APIs REST
- **TCP, UDP, IPv6, OpenThread, Matter, Thread, Zigbee, LoRa**

**Visualización:**
- **Interfaces de Usuario:** Paneles de control basados en web utilizando herramientas como Node-RED, otros tipo HMI (LCD, OLED, etc)
- **Visualización de Datos:** Opciones provistas por docentes desde el cloud

## Funcionamiento del Sistema

**Recolección de Datos:**
- **Sensores:** Los sensores instalados recolectan datos sobre variables ambientales críticas como humedad del suelo, niveles de pH, precipitaciones y temperatura.
- **Microcontroladores ESP32:** Los microcontroladores ESP32 reciben datos de los sensores a través de interfaces de comunicación como UART, SPI e I2C.

**Transmisión de Datos:**
- **Módulos LoRa:** Utilizando módulos de comunicación LoRa, los microcontroladores ESP32 transmiten los datos recolectados a una estación base o a un servidor central.
- **WiFi/Bluetooth:** Alternativamente, la comunicación puede realizarse mediante WiFi o Bluetooth, dependiendo de la infraestructura y el alcance requerido.

**Procesamiento de Datos:**
- **Servidor Central/Estación Base:** Un servidor central procesa los datos recibidos, analizando las condiciones ambientales y generando informes en tiempo real.
- **MQTT y HTTP/HTTPS:** Los datos son enviados y recibidos mediante protocolos MQTT para asegurar una comunicación eficiente y segura. Las integraciones con APIs REST permiten la interoperabilidad con otras plataformas y servicios.

**Toma de Decisiones y Actuación:**
- **Algoritmos de Control:** Basados en los datos procesados, los algoritmos de control toman decisiones para optimizar el riego.
- **Actuadores:** Los microcontroladores ESP32 envían comandos a los actuadores (bombas, sistemas de iluminación, motores de posicionamiento) para ejecutar las acciones necesarias, como activar el riego o ajustar la iluminación.

**Visualización y Monitoreo:**
- **Paneles de Control Web:** Los usuarios pueden monitorear y controlar el sistema a través de interfaces de usuario web, utilizando herramientas como Node-RED.
- **Visualización en Cloud:** Los datos también pueden ser visualizados en plataformas cloud, proporcionando accesibilidad remota y almacenamiento seguro de los datos históricos.

## Adaptabilidad del Sistema

**1. Zonas Urbanas:**
- **Inmótica:** Implementación en edificios, plazas, parques, galerías, peatonales, etc. Controlando el riego y mantenimiento de áreas verdes urbanas.
- **Domótica:** Aplicación en casas y departamentos, gestionando huertas interiores, macetas y jardines interiores para mantener un riego óptimo y automatizado.

**2. Zonas Rurales:**
- **Huertas y Quintas:** Para proyectos personales y productivos, gestionando pequeños cultivos y asegurando un uso eficiente del agua.
- **Fincas:** Implementación en grandes proyectos productivos de cultivos, optimizando el riego y mantenimiento de las plantaciones.

**3. Gestión de Plagas:**
- **Sensores de Movimiento:** Para detectar la presencia de aves y otros animales.
- **Sensores de Sonido:** Para detectar sonidos de plagas.
- **Cámaras de Vigilancia:** Para monitoreo visual.
- **Dispositivos Ultrasónicos y Rociadores de Agua:** Para disuadir plagas.
- **Luces Estroboscópicas y Barreras Físicas:** Para proteger áreas sensibles.

## Ejemplos de Implementaciones

**1. Maceta en un Departamento:**
- **Sensores:** Humedad del suelo, luz, temperatura
- **Actuadores:** Bombas pequeñas para riego, luces LED
- **Conectividad:** WiFi/Bluetooth
- **Uso:** Automatización de riego y control de luz para plantas de interior.

**2. Huerta Urbana:**
- **Sensores:** Humedad del suelo, pH, temperatura, lluvia
- **Actuadores:** Bombas de agua medianas, válvulas de riego, luces LED
- **Conectividad:** WiFi, LoRa
- **Uso:** Gestión eficiente de riego y monitoreo de condiciones del suelo en huertas comunitarias.

**3. Jardinería de una Peatonal:**
- **Sensores:** Humedad del suelo, temperatura, luz, movimiento (para gestión de plagas)
- **Actuadores:** Bombas de alta capacidad, sistemas de iluminación, rociadores de agua
- **Conectividad:** LoRa, WiFi
- **Uso:** Automatización del riego y mantenimiento de áreas verdes en peatonales, además de sistemas para repeler plagas como aves.

**4. Finca:**
- **Sensores:** Humedad del suelo, pH, temperatura, lluvia, radiación solar, viento, nutrientes en el suelo
- **Actuadores:** Bombas de alta capacidad, válvulas de riego industriales, sistemas de fertilización, sistemas de climatización
- **Conectividad:** LoRa
- **Uso:** Gestión avanzada del riego, fertilización y monitoreo de condiciones climáticas para optimizar la producción agrícola.

## Sprints del Proyecto

**Sprint 1: Planificación y Configuración Inicial (Semanas 1-3)**
- **Objetivos:** Definir la arquitectura de red, planificar la comunicación inicial, identificar variables a sensorizar y actuar, seleccionar y evaluar tecnologías de sensores y actuadores, instalar y probar los sensores y actuadores seleccionados.
- **Actividades:** Reunión inicial, investigación de métodos y protocolos de comunicación, listado de variables a sensorizar y actuar, instalación y configuración de dispositivos y librerías en ESP32, pruebas iniciales de funcionamiento.

**Sprint 2: Integración y Desarrollo de Software (Semanas 4-7)**
- **Objetivos:** Desarrollar software básico para la integración de sensores, realizar simulaciones y pruebas con ESP32, configurar protocolos de comunicación en red, implementar la alimentación y pruebas de sensores y actuadores, realizar pruebas de red y seguridad inicial.
- **Actividades:** Desarrollo del código de lectura de sensores, configuración de módulos de comunicación, pruebas iniciales de comunicación, configuración del sistema de alimentación, documentación de resultados de pruebas iniciales.

**Sprint 3: Configuración Avanzada y Optimización (Semanas 8-11)**
- **Objetivos:** Configurar comunicaciones inalámbricas (WiFi, Bluetooth), implementar servicios de red (MQTT, HTTP, DNS) y seguridad, realizar pruebas de seguridad y estabilidad, optimizar la comunicación y preprocesamiento de datos.
- **Actividades:** Configuración de módulos WiFi y Bluetooth en ESP32, pruebas iniciales de comunicación inalámbrica, configuración de servicios de red y medidas de seguridad avanzadas, pruebas de seguridad y estabilidad del sistema, optimización de la configuración del sistema según resultados de pruebas.

**Sprint 4: Pruebas Finales, Documentación y Presentación (Semanas 12-15)**
- **Objetivos:** Realizar pruebas finales del sistema, ajustar y corregir errores, revisar el proyecto completo y obtener retroalimentación final, preparar y entregar la documentación final del proyecto, defender el proyecto ante los evaluadores.
- **Actividades:** Realización de pruebas finales de funcionamiento, verificación de la integración completa de todos los componentes, implementación de mejoras basadas en la retroalimentación, preparación y entrega de la documentación final, presentación y defensa del proyecto final.

## Conclusión

Este programa estructurado y coordinado permitirá a los estudiantes adquirir y aplicar conocimientos prácticos y teóricos en el desarrollo de un sistema IoT completo y funcional para la gestión y monitoreo de recursos hídricos locales, preparándolos para enfrentar los desafíos del campo del IoT en el ámbito profesional.

---

**ISPC - Instituto Superior Politécnico de Córdoba**
