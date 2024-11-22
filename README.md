# 📊 Análisis de Campañas de Marketing por Email  
**Autor:** [Daniel Robles Aller](www.linkedin.com/in/danielroblesaller) 

**Tecnologías Utilizadas:** Power BI, DAX, Power Query  

---

## **Descripción del Proyecto**
Este proyecto analiza el rendimiento de una serie de campañas de marketing por email, con el objetivo de identificar patrones de comportamiento y oportunidades de optimización. Mediante Power BI, he transformado los datos brutos en insights claros y accionables, apoyándome en la creación de medidas DAX, visualizaciones interactivas y un modelo de datos optimizado. El repositorio incluye tanto el archivo `.pbix` como un informe detallado en PDF con los hallazgos clave.

---

## **Archivos en el Repositorio**

- **`EmailCampaignAnalysis.pbix`**: Archivo de Power BI con el modelo de datos, medidas DAX, visualizaciones y configuraciones de segmentación.
- **`Conclusiones_Análisis.pdf`**: Informe en PDF con un resumen detallado de los hallazgos y recomendaciones estratégicas para optimizar el rendimiento de las campañas.
- **`README.md`**: Documento de introducción y descripción del proyecto (este archivo).

---

## **Estructura del Análisis**

### 1. **Exploración y Transformación de los Datos**  
   - **Manejo de Valores Faltantes**: En la columna `Dispositivo`, los valores nulos se reemplazaron con "Desconocido" para asegurar que todos los registros se incluyeran en el análisis.
   - **Extracción de Información del Email**: Se creó una columna para extraer el dominio de cada correo, lo que permitió analizar las tasas de rebote y conversión por proveedor de correo electrónico.
   - **Estandarización de Fechas**: Se incluyó una **Dimensión de Fechas** para facilitar el análisis temporal con segmentaciones por mes, trimestre y año.

### 2. **Diseño del Modelo en Estrella**  
   - **Tabla de Hechos**: La tabla principal, `HechosInteracciones`, contiene los eventos de interacción en las campañas, incluyendo clics, aperturas, rebotes y conversiones.
   - **Tablas de Dimensiones**: Se crearon las siguientes dimensiones para optimizar el análisis:
     - **DimCampañas**: Incluye detalles sobre el nombre, tipo y objetivo de cada campaña.
     - **DimClientes**: Define el segmento del cliente (lead o cliente existente).
     - **DimGeografía**: Incluye información de ubicación por país, con latitud y longitud.
     - **DimDispositivos**: Clasifica los tipos de dispositivos, incluyendo la categoría "Desconocido".
     - **DimDominios**: Contiene información sobre el dominio del correo electrónico del cliente.
     - **DimCalendario**: Permite realizar segmentaciones temporales para el análisis histórico de las campañas.

### 3. **Creación de Medidas DAX**  
   Se desarrollaron varias medidas DAX para responder a preguntas específicas sobre el rendimiento de las campañas:
   - **Tasa de Clics, Tasa de Rebote, Tasa de Conversión y Tasa de Cancelación de Suscripción**: Métricas clave para evaluar la efectividad de las campañas.
   - **Medidas de Segmentación**: Totales de clics y conversiones divididos por segmentos de cliente y tipo de dispositivo.
   - **Filtros para Top N**: Configuración de filtros en visualizaciones para identificar los países y dominios con mejor y peor rendimiento en diversas métricas.

### 4. **Visualizaciones en Power BI**  
   Se configuraron visualizaciones específicas para responder a cada pregunta planteada. Estas visualizaciones incluyen:
   - **KPIs de Métricas Globales**: Tasa de Apertura, Tasa de Clics, Tasa de Conversión y Tasa de Rebote, ubicados en la parte superior para brindar una vista general.
   - **Gráficos de Barras, Líneas y Circulares**: Para análisis detallados de clics y conversiones por país, tipo de dispositivo, tipo de campaña y otros factores.
   - **Mapa Interactivo**: Representación geográfica de la Tasa de Apertura, mostrando el rendimiento de las campañas por país.
   - **Tooltip**: Que interactua con el mapa para visualizar el rendimeinto por Segmento, las Interacciones y las Conversiones en cada uno de los paises.
   - **Botones de Navegación**: Implementados para optimizar el espacio y permitir alternancia entre visualizaciones.

---

## **Cómo Visualizar el Proyecto**

Para ver el análisis en Power BI:
1. Descargue el archivo **EmailCampaignAnalysis.pbix**.
2. Ábralo en Power BI Desktop para explorar el modelo de datos, las visualizaciones y las medidas DAX.
3. Consulte el archivo **Conclusiones_Análisis.pdf** para una descripción detallada de los hallazgos clave y recomendaciones.

---

Este proyecto demuestra habilidades avanzadas en **análisis de datos**, **Power BI**, y **DAX**, así como capacidad para **documentar y estructurar proyectos** en GitHub. Cada paso del análisis fue diseñado para maximizar el valor de los datos y proporcionar insights estratégicos, siguiendo buenas prácticas en modelado de datos y visualización.

---
## Contacto


- **Email:** [danielroblesaller@gmail.com](mailto:danielroblesaller@gmail.com)
- **LinkedIn:** [Daniel Robles](https://www.linkedin.com/in/danielroblesaller)

---

**¡Gracias por visitar mi repositorio!**

---
