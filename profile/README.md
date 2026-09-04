<p align="center">
  <img src="https://avatars.githubusercontent.com/u/131711383" alt="Webfiable" width="60">
</p>
<h1 align="center">WEBFIABLE</h1>

<p align="center">
  <strong>Seguridad y salud para WordPress, impulsado por investigación en IA aplicada a negocio</strong>
</p>

<p align="center">
  <a href="https://webfiable.com">Web</a> · <a href="https://app.webfiable.com">Evaluación rápida</a> · <a href="https://wordpress.org/plugins/webfiable-info/">Plugin en WordPress.org</a>
</p>

---

## Qué es Webfiable

Webfiable es un servicio que analiza la configuración y seguridad de sitios WordPress. Detecta vulnerabilidades, configuraciones problemáticas y versiones desactualizadas, y entrega recomendaciones concretas para corregirlas.

Funciona a través de dos vías complementarias:

- **Evaluación rápida:** Ingresa la URL de tu sitio en [app.webfiable.com](https://app.webfiable.com) y obtén un diagnóstico inmediato basado en el análisis del HTML público: enlaces rotos, contenido mixto, directorios expuestos, protección del login y estado de plugins. Sin instalar nada. Es un buen punto de partida; para resultados con precisión completa, [instala el plugin](https://wordpress.org/plugins/webfiable-info/).

- **Plugin para WordPress:** Instala [Webfiable Info](https://wordpress.org/plugins/webfiable-info/) y recibe informes semanales por correo con detección precisa basada en los datos reales de tu entorno, no en inferencia por HTML.

  ![Versión](https://img.shields.io/wordpress/plugin/v/webfiable-info?label=versi%C3%B3n&color=blue) ![Probado hasta WordPress](https://img.shields.io/wordpress/plugin/tested/webfiable-info?label=probado%20hasta%20WP&color=green) ![Licencia](https://img.shields.io/badge/licencia-GPL%20v3-blue)

El proyecto está en fase beta pública. No hay costo, ni suscripción, ni transacciones comerciales.

## Por qué existe

Webfiable es un proyecto de investigación personal. Mi objetivo es entender de forma práctica cómo la inteligencia artificial puede acelerar, y en algunos casos transformar, los modelos de negocio digital.

La pregunta que me interesa es concreta: si hoy una persona puede apoyarse en IA para cubrir desarrollo de software, infraestructura, marketing, operaciones y atención al usuario, ¿qué cambia en la forma de evaluar, construir y escalar una iniciativa digital?

Webfiable es el laboratorio donde pruebo esas ideas. Un servicio funcional, con usuarios reales, que me obliga a resolver problemas de extremo a extremo: desde la arquitectura técnica hasta la comunicación con el usuario final. Cada decisión en este proyecto alimenta una visión más informada sobre qué es viable, qué acelera la IA y dónde siguen siendo indispensables el criterio y la experiencia humana.

## Sobre mí

He construido mi carrera en la intersección entre tecnología y negocio, con experiencia en Latinoamérica y Europa. He pasado por roles técnicos, consultoría, ventas enterprise y dirección general en hyperscalers globales, Big Four, consultoras de TI y de ciberseguridad, y una startup SaaS que cofundé como CTO. Hoy lidero Customer Success para EMEA en un fabricante de software de gestión de TI y ciberseguridad.

El hilo que conecta todo eso es el mismo: entender qué puede hacer la tecnología por un negocio y tomar decisiones con criterio sobre ello. Mantengo capacidades de desarrollo activas porque esa cercanía al detalle técnico es lo que me permite investigar las nuevas tendencias y sus potenciales efectos en modelos de negocio. Webfiable es donde convergen esa curiosidad técnica y la visión ejecutiva.

Puedes encontrarme en [LinkedIn](https://www.linkedin.com/in/fcovecino/).

## Estado actual y roadmap

Hoy Webfiable ofrece evaluación rápida por HTML desde [app.webfiable.com](https://app.webfiable.com) y reportes semanales detallados a través del [plugin instalable](https://wordpress.org/plugins/webfiable-info/), cubriendo enlaces rotos, contenido mixto, directorios expuestos, protección de login, estado de plugins y versión de WordPress, análisis de conexión TLS/SSL y encabezados HTTP de seguridad.

**Próximamente:** evaluación de versión PHP · evaluación de temas instalados · retroalimentación integrada en reportes.

📋 [Changelog completo](CHANGELOG.md)

## Seguridad y privacidad

Webfiable está diseñado para que no tengas que confiar a ciegas:

- **El plugin es ligero y transparente:** código abierto bajo GPL v3, revisado y publicado en el directorio oficial de WordPress.org. Su única función es exponer un endpoint cifrado con el inventario de software de tu sitio. No ejecuta análisis, no corre procesos en segundo plano y no afecta el rendimiento.
- **El análisis ocurre fuera de tu sitio:** un proceso en los servidores de Webfiable consulta el endpoint, ejecuta las evaluaciones y te envía el reporte. No se requiere acceso al panel de administración ni credenciales.
- **Consentimiento explícito:** el endpoint está deshabilitado por defecto y solo se activa con tu autorización.
- **Recopilación mínima:** solo inventario de software (versiones de WordPress, plugins y temas). No se accede a credenciales, contenido ni datos de usuarios.
- **Cifrado en cada transmisión:** AES-256-CBC + RSA-2048 con IV único por respuesta. Solo Webfiable puede descifrar la información.

## Enlaces

🌐 [webfiable.com](https://webfiable.com) · 🔍 [Evaluación rápida](https://app.webfiable.com) · 🔌 [Plugin en WordPress.org](https://wordpress.org/plugins/webfiable-info/) · 📬 [soporte@webfiable.com](mailto:soporte@webfiable.com)

---

<p align="center"><sub>Proyecto personal en fase beta · No comercial · Hecho con curiosidad y café</sub></p>
