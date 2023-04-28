# Estimación de mortalidad por COVID-19: Modelo matemático de vacunación e intervenciones no farmacológicas para Colombia

El objetivo de este repositorio es proporcionar a los interesados, la documentación que permitan verificar, reproducir o implementar el modelo SEIR de vacunación e intervenciones no farmacológicas, propuesto para la tesis "Estimación de mortalidad por COVID-19: Modelo matemático de vacunación e intervenciones no farmacológicas para Colombia" para optar por título de MSc en Epidemiología, de la Facultad Nacional de Salud Pública “Héctor Abad Gómez”, Universidad de Antioquia.

## Descripción:

**NOTA:** Este proyecto fue realizado en Wolfram Mathematica 12.3.

**Archivos:**


1.  [Código del modelo](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis/blob/main/Cod_modelo_final.nb):

2. [Matrices de contacto para Colombia](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis/blob/main/MatricesCol.xlsx)

4. Use the `exexution.py` to run the code and set the receiver mails and other attributes

## Ejecución del modelo

Para reproducir o implementar este modelo matematico, deberá:

1. Descargar cada uno de los archivos incluidos en el [proyecto](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis)
2. Debe crear un (carpeta) en su ordenador con un proyecto en donde aloje los archivos que descargo anteriormente.
3. Abrir el archivo [Código del modelo](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis/blob/main/Cod_modelo_final.nb) y modificar el directorio con la dirección de la carpeta en donde alojó la documentación previamente descargada. 
   
 ```sh 
   SetDirectory["D:\\Oscar\Mendoza\\Documents\\UINIVERSIDAD\\MAESTRIA\\UNIVERSIDAD DE ANTIOQUIA\\II\\Proyecto\\Documento\\FINAL"]
 ```
 4. Modificar el dirección de la ubicación de las matrices de contacto, cargando el archivo **MatricesCol.xlsx** 
 
   ```sh 
  Bold = Import["D:\\Oscar \Mendoza\\Documents\\UINIVERSIDAD\\MAESTRIA\\UNIVERSIDAD DEANTIOQUIA\\II\\Proyecto\\Documento\\FINAL\\Bases de      datos\\MatricesCol.xlsx", "Data"]
   ```
  5. Modificar la dirección de la ubicación de la distribución de retraso, cargando el archivo **daysFisToDeath.csv**
 
 ```sh 
 dF2D = Import["D:\\Oscar \Mendoza\\Documents\\UINIVERSIDAD\\MAESTRIA\\UNIVERSIDAD DE \ANTIOQUIA\\II\\Proyecto\\Documento\\FINAL\\Bases de \datos\\daysFisToDeath.csv"] // Flatten;
  ```
  
  6. Modificar la dirección de la ubicación del archivo asociado a las muertes en Colombia por COVID-19 una vez ínicia el plan de vacunación. 
  
   ```sh 
dEmp = Import["D:\\Oscar Mendoza\\Documents\\UINIVERSIDAD\\MAESTRIA\\UNIVERSIDAD \DE ANTIOQUIA\\II\\Proyecto\\Documento\\FINAL\\Bases de \datos\\Casos_COVID\\Casos_COVID\\fallecidos_pos_mar2.csv"]
  ```

## Contribuciones



## Contacto

* [Oscar Ignacio Mendoza Cardozo](https://orcid.org/0000-0002-3881-6430) - oscar.mendoza1@udea.edu.co

## Agradecimientos:


    
    
    
    
   




