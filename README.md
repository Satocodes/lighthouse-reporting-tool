📌 1. Nombre del Repositorio

multihouse-reporting-tool

📄 2. Descripción breve (para GitHub)

Automated auditing tool for bulk analysis of URLs using PageSpeed Insights and Lighthouse, with CSV reporting. Includes CLI and optional frontend input.

📘 3. README.md

# Multihouse Reporting Tool

Multihouse es una herramienta diseñada para auditar en masa URLs mediante la API de PageSpeed Insights de Google, generando reportes CSV con métricas clave y sugerencias de optimización. Está pensada para uso interno en proyectos como Profuturo, con posibilidad de extenderse a otros dominios.

## 🚀 Características

- Carga masiva de URLs desde `urls.json`
- Soporte para análisis de:
  - PageSpeed (mobile y desktop)
  - Lighthouse (performance, accesibilidad, SEO, best practices)
- Generación de archivos `.csv` listos para presentar
- Modo CLI
- Posible integración con frontend web

## 📂 Estructura del Proyecto

.├── index.js # Script principal que corre Lighthouse
├── input.csv # Lista de URLs a auditar
├── output.csv # Archivo de salida con resultados
├── error-log.txt # Errores de ejecución
├── package.json # Dependencias del proyecto


## 🛠️ Instalación

```bash
git clone https://github.com/tuusuario/lighthouse-bulk-reporter.git
cd lighthouse-bulk-reporter
npm install

✏️ Cómo usar

    Abre el archivo input.csv y carga tus URLs en el siguiente formato:

Name,Page type,URL
Example,Home,https://example.com

    Corre el script:

node index.js

    Revisa el archivo output.csv con los resultados.

✅ Ejemplo de salida

Name,Page type,URL,Performance,Accessibility,Best practices,SEO
Example,Home,https://example.com,92,88,100,100

💡 Ideas futuras

    Agregar soporte para Web Vitals.

    Interfaz frontend para subir URLs y ver los resultados en tiempo real.

    Exportar en formatos adicionales (JSON, HTML).