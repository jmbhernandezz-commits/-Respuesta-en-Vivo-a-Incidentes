# 🛡️ Proyecto Final: Live Incident Response - 4Geeks Academy

Repositorio oficial del proyecto final del Bootcamp de Ciberseguridad, enfocado en la respuesta a incidentes en servidores activos (*Live Incident Response*), análisis forense de sistemas y remediación de amenazas.

## 📋 Descripción del Escenario
Se detectaron comportamientos anómalos en un servidor crítico de producción de 4Geeks Academy[cite: 1]. Bajo restricciones de alta disponibilidad (sin posibilidad de apagar el sistema), se asumió el rol de Analista de Ciberseguridad para inspeccionar, contener, erradicar y restaurar la integridad del servidor[cite: 1].

## 🛠️ Fases del Proyecto
1. **Reconocimiento y Recolección de Evidencias (Live Forensics):** Detección de cuentas de usuario no estándar (`hacker`), auditoría de puertos activos (FTP/21) y descubrimiento de un mecanismo de persistencia oculto en una tarea programada (`cron`) que exfiltraba información mediante `curl`.
2. **Remediación y Restauración:** Neutralización del cronjob malicioso, eliminación del script de exfiltración de credenciales (`/etc/passwd`) y remoción de la cuenta de usuario no autorizada.
3. **Informe Técnico Final:** Documentación detallada de los hallazgos, vulnerabilidades, acciones correctivas aplicadas y recomendaciones de endurecimiento (*hardening*).

## 📂 Contenido del Repositorio
* `INFORME TÉCNICO FINAL.pdf`: Documento completo con el desarrollo del caso y evidencias visuales.
