# **Sunai**
## **Postulacion Sunai**


**Descripción del desafío**:

En esta oportunidad, se cuenta con 2 archivos (.xlsx), donde cada uno representa la generación de energía en una planta solar de 1 día completo, dividida por inversor. La relación entre inversor y planta es de muchos a uno, es decir, una planta está relacionada a 1 o más inversores.

El desafío es poder procesar los archivos tomando en cuenta que en la realidad pueden haber 1000 archivos a procesarse.

Para cada archivo, se solicita lo siguiente:

1) Generar un gráfico, un line chart donde el eje x sea la fecha y el eje y sea el active power para finalmente guardarlo.

2) Guardar en un (.txt) la suma por día del active power, el valor máximo y mínimo del active energy y por último, la ruta donde se encuentra el grafico generado en 1).

3) Imprimir en consola la suma total del active power por día, de todas las plantas.


## **Repositorio: Sunai**

En el repositorio antes mencionado, se encuentra el desarrollo del algoritmo en cuestión.

Primero, deben descargarse ambos archivos .xlsx en su computadora, y guardar la ruta donde se van a descargar. Luego, se descarga el algoritmo como tal (postulacion_sunai.ipynb) y sólo se debe indicar la carpeta o ruta donde están los archivos excel.

El algoritmo guardará las graficas de *active_power_im* por fecha, por archivo, y mostrara en pantalla la *suma de active power* de cada planta, para todos los inversores. Adicionalmente, se creará un archivo .txt con el resumen por cada inversor para la suma, máximo y mínimo de *active_power_im*, con su respectiva fecha, para cada inversor.


-----------------------------------------------------------------------------------------------------------------------

### *Extra*

1) En caso que se trabajen con más fechas (mismo archivo o más de 1), la opción es *pd.concat* y concatenar las fechas en una columna maestra, para luego hacer una separación/clasificación por *groupby* y *get_group*.

2) Si se desea crear una carpeta y guardar allí archivos, está un módulo ejemplo llamado *create_archive_drop_files.ipynb* (es referencial, no aplica con al algoritmo original, se debe modificar para tal motivo).
