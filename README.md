Encontraran 4 archivos: 
1: Pdf con informe "Informe Tarea 1 ICD"
2: Script .python "Tarea1_icd_notebook"
3: Script .ipynb "Tarea1_icd_.ipynb"
4: Archivo README.md

Metodología
Se utilizó el lenguaje de programación Python en el entorno de desarrollo Jupyter Notebook, a través de Conda. Para el procesamiento, análisis y visualización de datos se utilizaron las siguientes librerías:

pandas
matplotlib
sqlalchemy
pymysql

Para la limpieza y el conteo de palabras se retiraron varios símbolos y signos de puntuación. Los análisis temporales de las obras consideraron el periodo 1588-1613, dividido en periodos de 5 años. La base de datos fue obtenida del Relational Dataset Repository.

Descripción de la base de datos y resultados obtenidos: 

Tabla works:
Columnas: id, Title, LongTitle, Date, GenreType

Tabla chapters:
Columnas: id, Act, Scene, Description, work_id

Tabla characters:
Columnas: id, CharName, Abbrev, Description

Tabla paragraphs:
Columnas: id, ParagraphNum, PlainText, character_id, chapter_id

Script de Análisis:
Para realizar el análisis y procesamiento de datos descrito en este informe, se ha creado un script en Python. Este script automatiza los pasos necesarios para:

Conectar a la base de datos y extraer los datos relevantes.
Realizar la limpieza de datos, incluyendo la eliminación de símbolos y signos de puntuación no deseados.
Generar análisis estadísticos y visualizaciones de los datos.
Identificar las palabras más frecuentes en las obras de Shakespeare.

Uso del Script
Para ejecutar el script, sigue estos pasos:
Clona el repositorio y navega al directorio del proyecto:

git clone https://github.com/HoracioDSS/Tarea-1-ICD/tree/main.git

Instala las dependencias necesarias utilizando Conda:

conda create --name shakespeare-analysis python=3.8
conda activate shakespeare-analysis
conda install pandas matplotlib sqlalchemy pymysql

Ejecuta el script en un entorno Jupyter Notebook:

jupyter notebook

En caso de no usar Conda: 

Crea un entorno virtual e instala las dependencias necesarias usando pip:

python -m venv env
source env/bin/activate   
pip install -r requirements.txt

Ejecuta el script en un entorno Jupyter Notebook:

pip install jupyter
jupyter notebook





