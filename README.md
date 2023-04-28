# Estimación de mortalidad por COVID-19: Modelo matemático de vacunación e intervenciones no farmacológicas para Colombia

El objetivo de este repositorio es proporcionar a los interesados, la documentación del modelo matemático tipo SEIR, que permita, verificar y reproducir los resultados de la tesis de maestria, denominada "Estimación de mortalidad por COVID-19: Modelo matemático de vacunación e intervenciones no farmacológicas para Colombia". Asimismo, aquellos investigadores que quieran implementar el modelo a otros contextos o modificar el modelo, se deja disponible todo el proyecto y la documentación.

## Descripción:

**NOTA:** Este proyecto fue realizado en Wolfram Mathematica 12.3.

**Archivos:**


1.  [código del modelo](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis/blob/main/Cod_modelo_final.nb)

2. [Matrices de contacto para Colombia](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis/blob/main/MatricesCol.xlsx)

3. [Distribución de retraso](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis/blob/main/daysFisToDeath.csv)

4. [Mortalidad Colombia](https://github.com/IgnacioMendozaC/MortalidadCOVID-19tesis/blob/main/fallecidos_pos_mar2.csv)

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

* [Oscar Ignacio Mendoza Cardozo](https://orcid.org/0000-0002-3881-6430)
* :email: oscar.mendoza1@udea.edu.co



## Agradecimientos:
 
 Maestría en Epidemiología, Facultad Nacional de Salud Pública “Héctor Abad Gómez”, Universidad de Antioquia.


    Notas:
    
     `exexution.py` 
    
    
    
   




