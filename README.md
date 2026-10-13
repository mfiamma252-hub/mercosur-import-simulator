# mercosur-import-simulator
Calculadora web de costos de importación y aranceles para países del Mercosur.

# ImportCalc · Cross-Border Trade & Cost Simulator

**ImportCalc** es una herramienta web interactiva diseñada para calcular el costo real de importar productos desde plataformas internacionales (como Amazon, Temu o Shein) hacia países del Mercosur (Argentina, Brasil y México), incorporando normativas aduaneras, franquicias y tasas vigentes.

Este proyecto nació con un enfoque práctico para resolver un problema real de optimización de costos en compras internacionales, uniendo el análisis de comercio exterior con el desarrollo frontend.

## Funcionalidades Principales
* **Calculadora de Costos de Importación:** Permite ingresar múltiples productos en USD, sumar costos de envío y calcular automáticamente el precio final en la moneda local de destino con los impuestos y aranceles estimados.
* **Comparador de Tiendas (Importado vs. Mercado Local):** Evalúa si conviene comprar un producto en una tienda internacional o adquirirlo directamente en Mercado Libre, contrastando regímenes de courier, franquicias y costos logísticos.
* **Motor de Reglas Aduaneras por País:** Implementa la lógica de cálculo específica para:
  * **Argentina:** Régimen Courier (ARCA) y Correo Argentino (Puerta a Puerta).
  * **Brasil:** Remessa Conforme (Receita Federal).
  * **México:** Régimen simplificado de paquetería (SAT).
* **Tipos de Cambio en Tiempo Real:** Integración con la API de Frankfurter con un sistema de *fallback* para garantizar disponibilidad.

## Stack Tecnológico
* **HTML5 & CSS3:** Diseño moderno *responsive* con modo oscuro, tipografías cuidadas (*Syne* e *Instrument Sans*), uso avanzado de CSS Grid y Flexbox.
* **JavaScript (Vanilla):** Lógica de negocio, manipulación del DOM, gestión de estados y llamadas asíncronas (`fetch` API).
* **APIs externas:** Consumo de tasas de cambio internacionales en tiempo real.

## Estructura del Proyecto
El proyecto está diseñado como una aplicación ligera de archivo único (*single-file architecture*), lo que facilita su despliegue inmediato en plataformas estáticas como GitHub Pages:

```text
├── index.html         # Código fuente completo (Estructura, Estilos CSS y Lógica JS)
└── README.md          # Documentación del proyecto

Este proyecto esta desarrollado como una solución práctica para la toma de decisiones en comercio electrónico transfronterizo (B2C), combinando fundamentos de aranceles aduaneros y desarrollo web frontend.
