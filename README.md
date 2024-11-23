# Caso Monopoly Bank

* Dataset 📁 [Dormammu-Bank](https://docs.google.com/spreadsheets/d/103uUUCE4gn83UYqC7z3yv2Kymc7LSCL0/edit?usp=sharing&ouid=113786428185283411378&rtpof=true&sd=true)

## Objetivo 🎯💡
Identificar patrones de consumo entre hombres y mujeres clientes de Dormammu, analizando hábitos como promedio de renta, cupo de tarjeta, montos de facturación, cantidad de transacciones y pagos de deudas en compras nacionales e internacionales. Además, se buscará evaluar la propensión de los clientes a continuar o abandonar los servicios del banco, utilizando el target del dataset como variable objetivo, previa exploración para entender su comportamiento.

## Contexto 📝
El banco Monopoly lleva muchos años atendiendo a sus clientes en Chile y recientemente ha sido adquierido por un Banco con capitales extranjeros llamado "Dormammu". Dormammu ha encargado a sus ingenieros hacer estudios sobre los clientes del banco Monopoly, para conocer su comportamiento detectar patrones. Además, debe analñizar cómo será su estrategia para abordar estos nuevos clientes dado el uso que ellos hacen de sus productos financieros. Los ingenieros del área informática del banco Monopoly han extraído una base de datos segúnuna solicitud recibida por el nuevo dueño del banco y la han compartido con los ingenieros de Dormammu que están en la sede de New York. La base contiene una muestra de clientes con 12 meses de información almacenada en variables que sirvan para alguna interpretación y entregar la mayor información posible a los dueños de este banco para que puedan conocer a los clientes, preparar una estrategia abordar a este nuevo mercado. La base de datos tiene variables asociadas a información del cliente variables mensuales, es decir una por cada mes, el cliente no se repite las variables asociadas se van agregando como una colmna más.

## Conclusiones 📋

* Al realizar un estudio al DataSet del Banco Monopoly/Dormammu, podemos encontrar que existen pocas variables categoricas, en la que destaca la 'Sexo', con la cual podimos ver el comportamiento de los clientes Masculinos como Femeninos en sus movimientos bancarios, ya sea en los cupos que poseen en las tarjetas de creditos, los montos facturados, los montos pagados de sus deudas y las transacciones realizadas en el año de estudio, cuantas cuentas poseen, entre otras.
* Ahora, las variables númericas proporcionadas en el DataSet, son muy dispersas, las cuales no poseen en su mayoria una moda, lo cual dificultad un estudio a travez de graficos, por ende, se utiliza estadistica basica para conocer su comportamiento a travez de los meses.

* Al tener un DataSet con muchas observaciones y caracteristicas, hay un gran procesamiento de datos, por lo que conlleva a tener lentitud en la carga de los datos, por lo que en muchas ocaciones, no se pueden realizar estudios con un alto procesamiento de los valores de las caracteristicas.

* Con respecto al aprendizaje supervisado, el mejor modelo es el de regresión logistica por su alta precisión en compración a los otros modelos de regresión, seguida por el modelo de clasificación K-NN

* Por ultimo, para el aprendizaje no supervisado se presenta como mejor algortmo el cluster jeraquico, ya que se identifica claramente los dos comportamientos de los clientes del banco

## Tecnologías y Librerías 💻

- **Python** 🐍: Lenguaje de programación de alto nivel, ampliamente utilizado en análisis de datos.
- **Numpy** 🔢: Librería para cálculos numéricos y operaciones con matrices.
- **Pandas** 🐼: Librería para la manipulación y análisis de datos en estructuras de datos como DataFrames.
- **Seaborn** 📊: Librería para visualización de datos basada en Matplotlib, ideal para gráficos estadísticos.
- **Matplotlib - pyplot** 📈: Herramienta de visualización de gráficos, ampliamente utilizada para crear gráficos estáticos.
- **Google Colab** ☁️: Entorno de desarrollo interactivo basado en la web, ideal para ejecutar Python en la nube.

## Procedimientos 🛠️  
1. 📊 **Análisis Exploratorio de Datos (EDA):**  
   - Exploración inicial para identificar patrones, relaciones y valores atípicos.  

2. 🧹 **Preprocesamiento de Datos:**  
   - Limpieza de datos, manejo de valores faltantes y creación de nuevas características.  

3. 🤖 **Construcción de Modelos:**  
   - **Aprendizaje Supervisado:** Modelos de clasificación y predicción basados en datos etiquetados.  
   - **Aprendizaje No Supervisado:** Detección de patrones y agrupaciones en datos no etiquetados.

## Diccionario de Variables 🏷️

| **Variable**       | **Descripción**                                                                 |
|--------------------|---------------------------------------------------------------------------------|
| **CORRELATIVO**     | Identificador cliente                                                           |
| **Region**          | Región de Residencia                                                            |
| **Renta**           | Renta del cliente                                                                |
| **Sexo**            | Sexo                                                                            |
| **Subsegmento**     | Subsegmento                                                                     |
| **Edad**            | Edad                                                                             |
| **Adicional**       | Indicador de Tenencia de TC adicionales                                         |
| **Antiguedad**      | Antigüedad del cliente (meses)                                                  |
| **CambioPin**       | Indicador del cambio de clave secreta de la tarjeta                             |
| **Consumo**         | Indicador de Crédito de Consumo                                                 |
| **Debito**          | Indicador de Tenencia de TD                                                      |
| **Ctacte**          | Indicador de Cuenta Corriente                                                   |
| **Cuentas**         | Número de cuentas que tiene el cliente                                          |
| **Hipotecario**     | Indicador de Crédito Hipotecario                                                |
| **Internauta**      | Indicador de cliente Internauta que usa la web Monopoly                         |
| **Monoproducto**    | Indicador de si el cliente es solo poseedor de una TC                           |
| **TC**              | Número de TC que tiene el cliente                                               |
| **Dualidad**        | Indicador de Dualidad (Cliente es dual si tiene 2 o más TC)                     |
| **CUPO_L1**         | Cupo de la tarjeta crédito para compras nacionales                              |
| **CUPO_MX**         | Cupo de la tarjeta crédito para compras internacionales                         |
| **CUPO_L2**         | Cupo de la tarjeta crédito para avances en cuotas                               |
| **Col_T12**         | Colocación del cliente en TC en el mes X                                         |
| **ColL1TE_T12**     | Revolving del cliente en TC en el mes X                                          |
| **EeccInt_T12**     | Monto internacional exigido en el estado de cuenta del cliente en el mes X       |
| **EeccNac_T12**     | Monto nacional exigido en el estado de cuenta del cliente en el mes X            |
| **Fac_T12**         | Monto facturado por el cliente en TC en el mes X                                 |
| **FacAI_T12**       | Monto facturado en avances internacionales por el cliente en TC en el mes X      |
| **FacAN_T12**       | Monto facturado en avances nacionales por el cliente en TC en el mes X           |
| **FacCCOT_T12**     | Monto facturado en compras en cuotas con tasa por el cliente en TC en el mes X   |
| **FacCCPC_T12**     | Monto facturado en compras en cuotas precio contado por el cliente en TC en el mes X |
| **FacCI_T12**       | Monto facturado en compras internacionales por el cliente en TC en el mes X     |
| **FacCN_T12**       | Monto facturado en compras nacionales por el cliente en TC en el mes X           |
| **FacCOL_T12**      | Monto facturado en avances en cuotas por el cliente en TC en el mes X            |
| **FacDebAtm_T12**   | Monto facturado en avances por el cliente en TD en el mes X                      |
| **FacDebCom_T12**   | Monto facturado en compras por el cliente en TD en el mes X                      |
| **FacPAT_T12**      | Monto facturado en PAT por el cliente en TC en el mes X                          |
| **FlgAct_T12**      | Indicador de actividad en el mes X en la TC                                      |
| **FlgActAI_T12**    | Indicador de actividad en avances internacionales en el mes X en la TC          |
| **FlgActAN_T12**    | Indicador de actividad en avances nacionales en el mes X en la TC               |
| **FlgActCCOT_T12**  | Indicador de actividad en compras nacionales en cuotas con tasa en el mes X en la TC |
| **FlgActCCPC_T12**  | Indicador de actividad en compras nacionales en cuotas precio contado en el mes X en la TC |
| **FlgActCI_T12**    | Indicador de actividad en compras internacionales en el mes X en la TC          |
| **FlgActCN_T12**    | Indicador de actividad en compras nacionales en el mes X en la TC               |
| **FlgActCOL_T12**   | Indicador de actividad en avances en cuotas con tasa en el mes X en la TC        |
| **FlgActPAT_T12**   | Indicador de actividad en PAT en el mes X en la TC                               |
| **PagoInt_T12**     | Monto de pagos de deuda internacional del cliente en el mes X                    |
| **PagoNac_T12**     | Monto de pagos de deuda nacional del cliente en el mes X                         |
| **Txs_T12**         | Número de transacciones realizadas por el cliente en TC en el mes X             |
| **TxsAI_T12**       | Número de transacciones en avances internacionales realizados por el cliente en TC en el mes X |
| **TxsAN_T12**       | Número de transacciones en avances nacionales realizados por el cliente en TC en el mes X |
| **TxsCCOT_T12**     | Número de transacciones en compras en cuotas con tasa realizados por el cliente en TC en el mes X |
| **TxsCCPC_T12**     | Número de transacciones en compras en cuotas precio contado realizados por el cliente en TC en el mes X |
| **TxsCI_T12**       | Número de transacciones en compras internacionales realizados por el cliente en TC en el mes X |
| **TxsCN_T12**       | Número de transacciones en compras nacionales realizados por el cliente en TC en el mes X |
| **TxsCOL_T12**      | Número de transacciones en avances en cuotas por el cliente en TC en el mes X    |
| **TxsDebAtm_T12**   | Número de transacciones en avances realizados por el cliente en TD en el mes X  |
| **TxsDebCom_T12**   | Número de transacciones en compras realizados por el cliente en TD en el mes X  |
| **TxsPAT_T12**      | Número de transacciones en PAT realizados por el cliente en TC en el mes X      |
| **UsoL1_T12**       | Monto de deuda en la línea de compras en la TC en el mes X                       |
| **UsoL2_T12**       | Monto de deuda en la línea de avances en cuotas en la TC en el mes X             |
| **UsoLI_T12**       | Monto de deuda en la línea de compras internacionales en la TC en el mes X       |


## Creditos 🙌
* David Valenzuela
* Mauricio Donato
* Víctor Vargas
