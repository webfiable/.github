# Changelog

Historial de cambios relevantes en Webfiable. Este registro cubre tanto el servicio de análisis como la aplicación web ([app.webfiable.com](https://app.webfiable.com)). Para cambios específicos del plugin, consulta el [changelog en WordPress.org](https://wordpress.org/plugins/webfiable-info/#developers).

---

## Marzo 2026

> Nuevas capacidades de análisis de seguridad y limpieza de arquitectura.

- 🆕 **Análisis de encabezados HTTP de seguridad.** Nueva evaluación que verifica la presencia y configuración de headers de seguridad en el sitio analizado.
- 🆕 **Análisis de conexión TLS/SSL.** Nueva evaluación que inspecciona el certificado, protocolo y configuración TLS del sitio.
- ✨ **Mejoras en la promoción del plugin.** La evaluación rápida ahora incluye información sobre el plugin antes y después del análisis para facilitar su adopción.
- 🧹 **Eliminación de proyectos legacy.** Limpieza de componentes obsoletos de la solución.

## Febrero 2026

> Rediseño de reportes, migración de plataforma y mejor detección de enlaces.

- 🆕 **Migración a .NET 10.** Actualización de toda la plataforma al framework más reciente.
- 🆕 **Nuevo sistema de reportes por correo.** Rediseño completo del reporte semanal con mejor estructura visual, badges de severidad e información más clara sobre el estado de cada verificación.
- 🆕 **Flujo de correo para plugin no detectado.** Cuando el endpoint del plugin no responde, el sistema envía un correo con instrucciones para instalar, activar o configurar Webfiable Info.
- ✨ **Detección de enlaces mejorada.** La auditoría de enlaces rotos y contenido mixto ahora se ejecuta desde el servidor con verificación real de cada URL, reemplazando la detección anterior basada solo en HTML.
- 🔧 **Correcciones de codificación en correos.** Soporte completo de caracteres especiales del español en los reportes por correo.

## Enero 2026

> Mejoras visuales en reportes.

- ✨ **Mejoras en el reporte.** Mensaje de plugin desactualizado y mejoras visuales en el formato del correo.

## Diciembre 2025

> Reorganización de la arquitectura interna para soportar las nuevas evaluaciones.

- 🆕 **Nuevo modelo de datos para análisis.** Reorganización en grupos (DNS, hosting, HTTP, TLS, headers, WordPress) para soportar las nuevas evaluaciones de forma extensible.
- 🆕 **Herramienta de reintento de registros.** Utilidad para reintentar automáticamente el registro de sitios que quedaron pendientes de verificación, con notificación por correo al administrador.
- ✨ **Lógica robusta de comparación de versiones de plugins.** Soporte para versionado semántico, pre-releases y formatos no estándar comunes en WordPress.
- ✨ **Separación de registro y validación.** El proceso de registro del plugin ya no bloquea la respuesta del API; la validación se ejecuta de forma asíncrona.

## Noviembre 2025

> Lanzamiento de la nueva aplicación web y sistema de clientes.

- 🆕 **Nueva aplicación web (app.webfiable.com).** Interfaz completamente rediseñada con Tailwind CSS, soporte para modo claro/oscuro y diseño responsive.
- 🆕 **Barra de progreso en tiempo real.** El análisis muestra el avance mientras se ejecuta, con soporte para múltiples análisis simultáneos en distintas pestañas.
- 🆕 **Detección de plugins en la evaluación rápida.** La evaluación por HTML ahora identifica plugins instalados y evalúa sus versiones.
- 🆕 **Ciclo de vida de clientes.** Sistema de estados para el registro de sitios (pendiente, activo, etc.) con verificación automática.
- ✨ **Despliegue multiplataforma.** La aplicación ahora se ejecuta en entornos Linux y Windows.

## Octubre 2025

> Integración con el plugin 2.0 y servicios centralizados.

- 🆕 **Soporte para Webfiable Info 2.0.** Integración con el nuevo esquema de registro automático del plugin.
- 🆕 **Servicio de envío de correos.** Nuevo componente centralizado para el envío de reportes y notificaciones.
- ✨ **Comparación de versiones mejorada.** Soporte para formatos como "3.7.1-beta.1".

---

<details>
<summary><strong>2025 (enero - marzo)</strong></summary>

### Marzo 2025

> Integración del plugin en los reportes semanales.

- 🆕 **Análisis con plugin en la suscripción.** Los reportes semanales ahora aprovechan la información del plugin cuando está disponible, con un mensaje en la evaluación rápida indicando la diferencia.
- 🔧 **Mejoras en la gestión de caché.** Solución de errores de memoria y timeouts al limpiar el caché de respuestas HTTP.

### Febrero 2025

> Primera integración funcional con el plugin Webfiable Info.

- 🆕 **Integración del plugin Webfiable Info.** Primera versión funcional de la lectura de datos desde el endpoint cifrado del plugin.
- ✨ **Publicación de llave pública.** La llave RSA para el cifrado se publica como archivo estático en lugar de estar embebida en el código del plugin.

### Enero 2025

> Nuevo branding y limpieza de código.

- ✨ **Nuevo branding.** Adaptación visual de la aplicación a la identidad de Webfiable.
- 🔧 **Mejor detección de directorios expuestos.** Verificación de que la URL final corresponde al directorio consultado antes de reportarlo como accesible.
- 🔧 **Mejor detección de login expuesto.** Reducción de falsos positivos al verificar la protección del acceso a wp-login.php.
- 🧹 **Eliminación de código legacy.** Limpieza de procedimientos obsoletos de conexión a sitios web.

</details>

<details>
<summary><strong>2024</strong></summary>

> Migración tecnológica, caché y modernización.

- ✨ **Migración a .NET 8.** Actualización del API, la interfaz web y los reportes al framework actual.
- 🆕 **Sistema de caché HTTP.** Las consultas a sitios web se almacenan temporalmente para mejorar rendimiento y reducir solicitudes repetidas.
- 🆕 **Reporte automático de errores.** Los errores de la plataforma se reportan automáticamente para diagnóstico centralizado.
- 🧹 **Modernización de controladores.** Adopción de características de C# 12 en toda la base de código.

</details>

<details>
<summary><strong>2023</strong></summary>

> Lanzamiento inicial de Webfiable.

- 🚀 **Lanzamiento inicial.** Primera versión pública de Webfiable con evaluación rápida por HTML.
- 🆕 **Análisis multi-página.** El escaneo revisa múltiples páginas de cada sitio en lugar de solo la página principal, con actualización en tiempo real.
- 🆕 **Reportes por correo (MVP).** Primera versión de los reportes semanales enviados automáticamente por correo electrónico.
- 🆕 **Detección de plugins por HTML.** Identificación de plugins instalados a partir del análisis del código fuente de las páginas.
- 🆕 **Detección de enlaces rotos y contenido mixto.** Identificación de enlaces que no funcionan y recursos cargados de forma insegura.
- 🆕 **Verificaciones de seguridad.** Evaluación de listado de directorios, seguridad de archivos y protección del login.

</details>

---

🆕 Nueva funcionalidad · ✨ Mejora · 🔧 Corrección · 🧹 Mantenimiento · 🚀 Hito
