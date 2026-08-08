

# Alertas de Prácticas Profesionales de LinkedIn (n8n)

Monitoree las publicaciones de las páginas de empresas en LinkedIn a través de feeds RSS y reciba alertas por correo electrónico cuando una publicación coincida con:
- Palabras clave de prácticas (intern/internship/تدريب…)
- Palabras clave del área (AI/ML/Data + variantes en árabe)

## Contenido
- `workflows/linkedin_internship_alerts.json` — importar en n8n
- `sheets/companies_template.csv` — plantilla de Google Sheets
- `docs/` — configuración + solución de problemas + palabras clave

## Inicio rápido
1. Crea una hoja de Google Sheets usando `sheets/companies_template.csv`
2. Rellena la columna `rss_link` (RSSHub u otro generador de RSS)
3. Importa el JSON del flujo de trabajo a n8n
4. Configura las credenciales de Google Sheets y Gmail
5. Edita las palabras clave en el nodo **Code**
6. Activa el flujo de trabajo

## Notas sobre la estabilidad del RSS
Las instancias públicas/comunitarias de RSSHub a menudo devuelven errores 503. Para mayor fiabilidad:
- aloja RSSHub en tu propio dominio/VPS, o
- utiliza un proveedor de pago estable de RSS “página-a-RSS”.
