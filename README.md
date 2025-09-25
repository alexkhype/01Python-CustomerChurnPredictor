# Predictor de pérdida de clientes

## Tabla de Contenidos
- [Descripción](#Descripción)
- [Datos](#Datos)
- [Análisis](#Análisis)
- [Tecnologías y herramientas](#Tecnologías-y-herramientas)
- [Resultados](#Resultados)
- [Contribuciones](#Contribuciones)
- [Licencia](#Licencia)
- [Contacto](#Contacto)

## Descripción
El proyecto construye un modelo de aprendizaje automático para pronosticar la tasa de cancelación de usuarios en Interconnet, un operador de telecomunicaciones. Se utilizan datos personales, planes y contratos para anticipar la cancelación y permitir acciones de retención con ofertas personalizadas.

## Datos
Se utilizaron 4 conjuntos de datos principales:  
- **contract.csv**: Datos de contratos de 7,043 clientes con fechas, tipo, pago y cargos mensuales y totales.
- **personal.csv**: Información demográfica y estado civil de 7,043 clientes, incluyendo género y dependientes.
- **internet.csv**: Servicios de internet contratados por 5,517 clientes, con detalles de seguridad, backup y streaming.
- **phone.csv**: Datos de línea telefónica para 6,361 clientes, indicando si tienen múltiples líneas contratadas.

## Análisis
El enfoque incluyó:  
- Integración y limpieza de 4 bases de datos con 7,043 registros.
- Definición de variable objetivo binaria basada en fecha de finalización de contrato.
- Exploración univariada y bivariada para identificar variables clave como tipo de contrato y antigüedad.
- Aplicación de técnicas de imputación, codificación y creación de variables derivadas para modelado.
- Entrenamiento y evaluación de modelos de clasificación con validación que incluye métricas como ROC AUC.
 
## Tecnologías y herramientas
- Python 3.9 para desarrollo general
- Pandas, NumPy para manipulación y análisis de datos
- Seaborn, Matplotlib para visualización gráfica
- Scikit-learn para modelado predictivo y evaluación
- LightGBM, CatBoost, XGBoost para modelos avanzados de boosting
- Jupyter Notebook para desarrollo interactivo y documentación
 
## Resultados
- Modelos basados en boosting (LightGBM, CatBoost, XGBoost) lograron ROC AUC entre 0.93 y 0.94.
- CatBoost destacó con mejor equilibrio entre precisión (0.89), sensibilidad (0.71) y estabilidad del modelo.
- Se identificó desequilibrio de clases (26.5% cancelación), priorizando precisión para retención eficiente.
- Se detectó anomalía en cancelaciones históricas que requiere revisión para evitar sesgos en análisis futuros.

## Contribuciones
Bienvenidas sugerencias, correcciones y nuevas visualizaciones. Por favor, abre un issue o pull request para colaborar.

## Licencia
Este proyecto está bajo la licencia MIT.

## Contacto
Nombre: Alejandro M. García  
Email: [alexkhype@gmail.com](mailto:alexkhype@gmail.com)  
LinkedIn: [linkedin.com/in/amggl](https://linkedin.com/in/amggl)
