
<h1 align="center">TELCOMs ANALYSIS IN ARGENTINA 2014 - 2022 </h1>

![telecom industry](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/ce533937-0ab5-452f-b79a-c8a00ef0f7b7)

 
This project is about analysing TELCOM sector in Argentina. The argentinian TELCOM market is a relatively well developed market with more than 62.12 million internet connections and it has evolved notably in accessibility since 2014.

I will go through two preprocessing parts and a reporting part:

    I. I had 11 datasets(from Enacom) in ETL and merged them into 5 meaningful tables from my point of view.
       See ETLs.ipynb file.
   
    II. I will explore the data and write some insights about the findings.
        See EDAs.ipynb file.
   
    III. I am going to do a dashboard which will be explained in more detail with the help of EDA.

This project will try to cope the following aspects (targets) analysing the data:

      1. Internet access in Argentina.
      2. Quality of the service.
      3. Profitability of the market.
      4. Which connectivity tecnologies are available in Argentina.

## Part I: ETL

I grouped the datasets as follows: 

TABLA 1: ACCESO A INTERNET POR VELOCIDAD DE BAJADA Y USO DE BANDA ANCHA O ANGOSTA TRIMESTRAL EN PROVINCIAS ARGENTINAS 2014 - 2022. 

  1. Número de accesos al servicio de Internet fijo por cada 100 hogares por provincia.
  2. Número de accesos al servicio de Internet fijo por velocidad de bajada en cada provincia (trimestral).
  3. Número de accesos al servicio de Internet fijo por banda ancha y banda angosta en cada provincia (trimestral).

TABLA 2: INGRESOS Y ACCESO A INTERNET POR TIPO DE TECNOLOGIA EN BANDA ANCHA O ANGOSTA TRIMESTRAL EN ARGENTINA 2014 - 2022

  1. Número total de accesos al servicio de Internet fijo por banda ancha y banda angosta (trimestral).
  2. Número de accesos al servicio de Internet fijo por tipo de tecnología. Total nacional (trimestral).
  3. Serie histórica de la velocidad media de descarga de Internet nacional (trimestral).
  4. Ingresos trimestrales de los operadores por el servicio de Internet fijo
 
TABLA 3:CONECTIVIDAD A INTERNET POR TIPO DE CONEXION EN LAS PROVINCIAS ARGENTINAS 2014 - 2022

  1. Listado de localidades con conectividad a internet, con detalle por tipo de conexión.

TABLA 4: TECNOLOGIAS DISPONIBLES POR PROVINCIA(PARTIDO Y LOCALIDAD) PARA ACCEDER AL SERVICIO DE INTERNET FIJO Y MOVIL 2014 -2022

  1. Consulta las tecnologías disponibles en tu localidad para acceder al servicio de Internet fijo y móvil

TABLA 5: NUMERO DE ACCESOS AL SERVICIO DE INTERNET FIJO POR VELOCIDAD DE BAJADA EN CADA LOCALIDAD DECLARADA

  1. Número de accesos al servicio de Internet fijo por velocidad de bajada en cada localidad declarada.

## Part II: EDA

These steps will lead the dashboard mainly:

  1. Graph 1 : Quarterly Trend of the Average Internet Access by Total Velocidad Bajada.
  2. Graph 2: Internet access for every 100 Household by argentinian province.
  3. Graph 4: Quarterly trend of the average download speed (ranges).
  4. Table 1.2: Quarterly rate growth by dowload speed (ranges).
  5. Table 2.2: Participacion of each access internet technology type (over Total_acceso_Tipotecnologia).
  6. Graph 9: Revenue trend by technology.
  7. Graph 11: Quarterly growth rate MBPS.
  8. Graph 14: Internet access percentages by technology.
  9. Table 4.1: Available internet technologies by aregentinian province.

## Part III: Dashboard

   #### Dashboard A:Accessibility vs Quality
   
![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/0975353e-3cb9-407d-a7c2-49fb5484db2d)

### III.1 Internet access in Argentina.

The internet access by every 100 household has increased since 2014, when it was 37 on average. It reached 67 on average(2022) in just 9 years.

![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/f6fc7981-df3f-4bf7-8ae3-67288c806290)

Capital Federal, Tierra del Fuego and La Pampa are the 3 provincies with more access by every 100 households and they are in the third percentile. 

Capital Federal, Tierra del Fuego, La Pampa, Cordoba, Chubut, San Luis, La Rioja, Neuquen, Santa Fe, Buenos Aires, Rio Negro, Catamarca, Entre Rios, Tucuman, Jujuy, Salta, Santiago del Estero, Misiones, Mendoza and San Juan have access above the average.

Corrientes, Chaco, Formosa y Santa Cruz have internet access under the average.

Average: 49.06574 C/100 Household.

If we set a KPI target of a internet access of 80 households out of 100 on average, Argentina would be close to get the goal.

An other way to see the access to internet is with variable Total velocidad bajada by Province, this shows something interesting about internet access in Argentina.

![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/2a389cd4-dc1d-414a-9b28-9e1e3a72609e)

Setting as Benchmark the average of "Total de velocidad de bajada(como proxy de acceso a internet)".
4 provinces out of 24 have internet access above the benchmark. These provinces are Buenos Aires, Capital Federal, Cordoba and Santa Fe. This doesnt only show inequalities in internet access, but in quality. 
 
The other 20 provinces might mean a good opportunity for potential markets analysing the reasons or why they do not have a good internet access in terms of quantity and quality.

### III.2 Quality of the service.

The KPIs Promedio de Acceso a internet por velocidad de bajada and Tasa de crecimiento de MBPS are both in red show that untill 2021 the internet access has increased steadily from 2014 but growth rate of MBPS did not increase. In fact, the MBPS growth rate decreased from 15 % in 2019 to 6% in 2022(in nominal terms the mbps is around 60 mbps) while the internet access by Velocidad bajada increased untill 2021.
![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/a22b5dc5-3ac4-4e67-bdd3-0d53841d0fd6)

![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/cad56f49-06d8-4b9a-924d-809e5df13ad6)


### III.3 Profitability of the market.

The amount of users or internet access measured by Promedio de acceso a internet por velocidad bajada might have a negative trend but revenues by type of technology used to provide internet have increased. The KPI Forecast ingresos shows a revenue of 183M by 2022 (with a goal of 200M) and the trend Evolucion Ingresos strengthens the first statementon this section. 

 #### Dashboard B: Revenues trend and revenues by technology

![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/f1aafd48-8a0e-403c-ad37-6fe4cefae141)

The most profitable technology is Cablemodem with 101M(miles de pesos). The second is fiber optic with 44M and third ADSL with 25M. Most of the profits come from provinces like Buenos Aires(1st), Capital Federal(2nd), Cordoba(3rd) and Santa Fe(4th). 

Until 2017 the download speed increased (see dashboard A), but the use of CABLEMODEM in the provision of the service began to skyrocket, fiber optics continued without being used intensively and since 2017 ADSL gradually ceased to be used.

Internet access has increased faster than the implementation of technologies that can cover or face a new demand for internet services. If we talk about fiber optic speed, internet can reach speeds of between 250 and 1000 Mbps, both upload and download. This makes fiber optic 5 times faster than a best cable connection.

### III.4 Which connectivity technologies are available in Argentina.

#### Dashboard C: Access to connectivity technologies

  ![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/edee1835-8a15-4fac-bc96-4765b95e7137)

Internet users connect to internet using technologies like: 

   1. 4G.
   2. Wireless.
   3. Telefoniafija.
   4. 3G.
   5. Satelital.
   6. Fibraoptica
   7. ADSL.
   8. Cablemodem.

As the list shows those technologies that are powerful in terms of speed of download and upload like fiber optic, ADSL and Cablemodem are at the bottom what means each time a new internet access is created, it might have problems like streaming in HD in platforms like youtube, Netflix or work from home. Although fiber optic, ADSL and Cablemodem can be found in the main cities from where the profits come importantly, they might have problems in terms of quality (mbps) according to the analysis above.

![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/b5c2196a-3950-45be-bc3c-9e97cb910631)

![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/d6272114-156e-4124-9372-9e66b7ba9b3a)

![image](https://github.com/MaxJv1/IndividualProject2DataAnalysis/assets/138952349/a0a64162-1131-49cc-b1a9-6d48eae7d902)


## IV. Conclusions

Accessibility to the service increased between 2014 and 2022 but its quality shows a negative trend. The volume of users(Velocidad descarga) shows a downward trend as well.

Cablemoden has skyrocketed since 2017 while there was no much invesment in fiber optic network and the accessibility to internet increased steadily until 2021.

The revenue has still increased which clearly shows that profits are led by prices more than new internet users.

The downward trend in quality may be a direct consequence of the lack of digital infraestructure (see profits by technology ) like fiber optic, the no optimization of existent digital infraestructure or both.

# Tools:

<div style="display:flex; align-items:center;">
  <div style="width:50%; padding-right:20px;">
    <h2>Herramientas Utilizadas</h2>
    <ul style="text-align: justify;">
      <li><b>🐍Python.</li>
      <li><b>📈Power BI.</li>
      <li><b>💻Numpy.</li>
      <li>🐼Pandas.<b></li>
      <li><b>📈Matplotlib.</li>
      <li><b>📈Seaborn.</li>
    </ul>
  </div>
 


# Author

Max Jeffer Cuellar Vizcarra

Correo electrónico: max_83_14@hotmail.com

LinkedIn: [Perfil de LinkedIn](https://www.linkedin.com/in/max-jeffer-cuellar-vizcarra-25197433/)

