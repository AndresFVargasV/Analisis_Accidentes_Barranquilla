# Análisis de Accidentalidad en Barranquilla

Este repositorio contiene un análisis descriptivo y de geolocalización de la accidentalidad en Barranquilla. El análisis se ha realizado utilizando Python, Azure Maps y Google Maps API para generar gráficos y mapas informativos.

## Contenido

1. **Notebooks de Análisis:**
   - `Accidentalidad_Barranquilla.ipynb`: Jupyter Notebook que realiza un análisis descriptivo de la accidentalidad en Barranquilla, incluyendo gráficos informativos y estadísticas clave.
   - `accidentes_bquilla_2023_ubicacion_fulldataset.csv`: CSV que contiene todos los datos de los accidentes presentados en Barranquilla en el año 2023 junto con las coordenadas de estos mismos.
   - `coordenadas_accidentes_bquilla_azure.csv`: CSV que contiene solo las coordenadas de los accidentes en Barranquilla en 2023 obtenidos con la API de Azure Maps. Esto con el fin de reutilizar estos datos y no hacer mucho consumo de recursos al obtener nuevamente los datos.
   - `coordenadas_accidentes_bquilla_gmaps_api.csv`: CSV que contiene solo las coordenadas de los accidentes en Barranquilla en 2023 obtenidos con la API de Google Maps. Esto con el fin de reutilizar estos datos y no hacer mucho consumo de recursos al obtener nuevamente los datos.
   - `barranquilla_map.html`: Este archivo HTML contiene la vista desde el navegador del análisis geo-espacial de los accidentes en Barranquilla en 2023. Así como también, podemos ver la semaforización y cámaras de tránsito de la ciudad en diferentes capas del mapa. 

2. **Datos:**
   - [Dataset Accidentalidad Barranquilla - Alcaldía de Barranquilla](https://www.datos.gov.co/Transporte/Accidentalidad-en-Barranquilla/yb9r-2dsi/about_data): A través de este enlace, podrás ingresar al dataset público de accidentes en Barranquilla desde el año 2018 hasta 2023. Este conjunto de datos es suministrado por La Alcaldía Distrital de Barranquilla, Distrito Especial, Industrial y Portuario.
   - [Dataset Detención Electronica Barranquilla - Alcaldía de Barranquilla](https://www.datos.gov.co/Transporte/Mapa-de-Puntos-de-Detecci-n-electr-nica-de-Barranq/4jwj-za7t): A través de este enlance, podrás ingresar al dataset público de todas las cámaras de tránsito registradas en Barranquilla. Este conjunto de datos es suministrado por La Alcaldía Distrital de Barranquilla, Distrito Especial, Industrial y Portuario.
   - [Dataset Semaforización Barranquilla - Alcaldía de Barranquilla](https://www.datos.gov.co/Transporte/Mapa-de-Semaforizaci-n-Barranquilla/cq6s-q4gx): A través de este enlance, podrás ingresar al dataset público de todos los semaforos registrados en Barranquilla. Este conjunto de datos es suministrado por La Alcaldía Distrital de Barranquilla, Distrito Especial, Industrial y Portuario.

3. **Gráficos y Mapas:**
   - En el cuaderno de Jupyter `Accidentalidad_Barranquilla.ipynb` encontrarás gráfico y conclusiones generadas durante el análisis.

## Requisitos y Dependencias

- Python 3.x
- Bibliotecas de Python: pandas, matplotlib, seaborn, folium, etc. (En la primera celda del cuaderno `Accidentalidad_Barranquilla.ipynb` podrás encontrar todas las bibliotecas necesarias para este análisis y solo basta con ejecutar la celda).

## Cómo Ejecutar el Análisis

- Clona este repositorio:

    ```bash
    git clone https://github.com/AndresFVargasV/Analisis_Accidentes_Barranquilla.git
    cd Analisis_Accidentes_Barranquilla
    ```

## Nota Importante

Deber tener en cuenta lo siguiente si quieres ejecutar o realizar un nuevo análisis con la script de obtención de coordenadas de los accidentes en el cuaderno de Jupyter:

- Azure Maps: Es necesario tener una cuenta de Microsoft Azure y tener activo el servicio de Azure Maps para poder generar una API KEY que permita obtener datos de coordenadas de los accidentes.

## Contribuciones

¡Las contribuciones son bienvenidas! Si encuentras problemas o tienes ideas para mejorar el análisis, por favor, abre un problema o envía una solicitud de extracción.

## Licencia

Este proyecto está bajo la [Licencia MIT](LICENSE).
