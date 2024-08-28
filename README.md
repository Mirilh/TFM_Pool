# Proyecto de Fin de Máster: Modelo Predictivo de pH en Piscinas

Este proyecto de fin de máster realizado por el alumno Miriam Lopez Hernandez se centra en el desarrollo de modelos predictivos para el control del pH en piscinas, utilizando datos recolectados de diversos dispositivos instalados en diferentes piscinas. El objetivo principal es mejorar la precisión en la predicción de pH mediante el uso de técnicas de Machine Learning, con el fin de optimizar el mantenimiento de las piscinas y garantizar la calidad del agua.

## Estructura del Proyecto

### 1. **DATA**
   - **Processed_Data**: Contiene los conjuntos de datos que han sido preprocesados y limpiados, listos para ser utilizados en la construcción de los modelos predictivos.
     - `datos_limpios_Device06.csv`
     - `datos_limpios_Device07.csv`
     - `DatosProcesados.csv`
   - **Raw_Data**: Incluye los datos originales y no procesados, así como documentación técnica relevante para los dispositivos utilizados en la recolección de datos.
     - `Chl_ChloroMaticLifeguard_Datasheet_AU.pdf`
     - `Chl_ChloroMaticLifeguard_IOI.pdf`
     - `Data_Pool.csv`
     - `setpoint.csv`

### 2. **Notebook**
   - **F2_AnalisisExploratorio.ipynb**: Contiene el análisis exploratorio inicial de los datos. En este notebook se realizan visualizaciones y estadísticas descriptivas para comprender mejor la naturaleza de los datos y detectar posibles problemas antes del preprocesamiento.
   - **F3_1_ModeloPredictivo_Device01.ipynb**: Notebook en el que se desarrolla y ajusta el modelo predictivo para el dispositivo 01. Incluye la selección de variables, construcción del modelo y ajuste de hiperparámetros.
   - **F3_2_ModeloPredictivo_Device07.ipynb**: Similar al anterior, pero centrado en el dispositivo 07. Este notebook también incluye el desarrollo del modelo y el ajuste fino para maximizar el rendimiento.
   - **F4_IntegracionModelo_Device03.ipynb**: Este notebook documenta el proceso de integración y prueba del modelo desarrollado en el dispositivo 07, aplicado a los datos del dispositivo 03. También se evalúa la eficacia de este modelo en un dispositivo diferente.
   - **F4_IntegracionModelo_Device06.ipynb**: En este notebook, se integran los modelos entrenados en los dispositivos 01 y 07 para evaluar su desempeño en el dispositivo 06. Este análisis es crucial para entender la capacidad de generalización de los modelos desarrollados.

### 3. **Otros Archivos**
   - **requirements.txt**: Lista de dependencias y paquetes necesarios para ejecutar los notebooks. Asegura que el entorno de desarrollo esté configurado correctamente.
   - **TFM_MiriamLopez_ModeloPredictivoPH.docx**: Documento final del proyecto, donde se detallan todas las fases del trabajo, los resultados obtenidos y las conclusiones.
   - **README.md**: El archivo actual, que proporciona una visión general del proyecto y la estructura de los archivos.

## Configuración del Entorno

Para ejecutar los notebooks, es necesario tener un entorno Python configurado con las dependencias indicadas en `requirements.txt`. Se recomienda el uso de un entorno virtual para aislar las dependencias del proyecto:

```bash
python -m venv env
source env/bin/activate  # En Windows: env\Scripts\activate
pip install -r requirements.txt

