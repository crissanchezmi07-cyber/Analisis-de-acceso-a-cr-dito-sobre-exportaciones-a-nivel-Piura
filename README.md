## Analisis de crédito al sector privado y exportaciones en Piura

# Pregunta guía 

¿En qué medida el crédito directo del sistema financiero al sector privado en Piura impacta en el nivel de exportaciones del departamento?

# Descripción General

Exploramos la relación entre el crédito directo al sector privado en Piura y las exportaciones, incorporando el Índice Costero El Niño (ICEN) como proxy de choques climáticos. Usamos datos mensuales 2005–2022 para construir un panel limpio y alineado, visualizar distribuciones, comparar dinámicas Piura vs. Perú y evaluar co-movimientos (correlaciones) y regularidades empíricas.

# Fuentes de datos (mensual)

Fuente principal: API del Banco Central de Reserva del Perú (BCRP)

Servicio oficial que entrega series macroeconómicas en formato JSON; garantiza trazabilidad, periodicidad mensual y metadatos consistentes.

Series 

- Crédito total nacional: Stock agregado de crédito al sector privado en todo el país; sirve como referencia para comparar el ciclo crediticio de Piura con la dinámica nacional.

- Crédito directo al sector privado a nivel de Piura (moneda nacional, moneda extranjera): Stock de préstamos del sistema financiero a empresas y hogares en Piura, desagregado en moneda nacional (MN) y moneda extranjera (ME); indica profundidad financiera regional y composición cambiaria.

- Exportaciones de Piura (FOB, US$): Valor mensual de ventas externas originadas en Piura a precios FOB en dólares; capta el desempeño exportador regional.

- Exportaciones nacionales (FOB, US$): Valor total de exportaciones del Perú; permite contextualizar a Piura dentro del patrón exportador agregado y su exposición a ciclos globales.

- Tipo de cambio promedio (S/ por US$): Cotización mensual promedio del sol frente al dólar; se usa para convertir exportaciones de US$ a S/ y para análisis de precios relativos. 

Fuente Índice Costero del Niño (ICEN): API del Instituto Geofísico del Perú (IGP)

Índice mensual del calentamiento/enfriamiento costero (Niño/Niña). Valores positivos sugieren Niño; negativos, Niña. Se utiliza como proxy de choques climáticos sobre la producción/exportación.

# Procedimiento

- Obtención de datos (BCRP)
- Limpieza macro y estandarización temporal
- Carga, limpieza y filtrado del ICEN
- Homologación de fechas y unión de variables macroeconómicas e Índice Costero del Niño
- Gráficos
  - Distribución Normal
  - Mapas  de calor
  - Boxplot
  - Series de tiempo
    
# Conclusión

- Existe una correlación casi perfecta entre el crédito regional y el nacional, lo que muestra que el sistema financiero de Piura está altamente integrado al ciclo macroeconómico del Perú. Los shocks nacionales o internacionales, como la pandemia del 2020, se transmiten con fuerza al ámbito regional.
- Aunque las exportaciones de Piura muestran una relación positiva con las nacionales, son mucho más volátiles. Esto se debe a que su canasta está concentrada en productos agroexportadores y pesqueros, muy sensibles a la variabilidad climática y a los precios internacionales, a diferencia del Perú en su conjunto que cuenta con una diversificación minera y productiva.
- El Índice Costero El Niño (ICEN) confirma que los eventos climáticos extremos son un factor de riesgo recurrente. Aunque sus correlaciones con exportaciones son débiles en magnitud, la evidencia visual es clara: episodios como el Niño 2017 coinciden con caídas severas en las exportaciones regionales, subrayando la vulnerabilidad de Piura frente al clima.
- Las distribuciones revelan que el crédito (tanto en Piura como en el país) sigue un crecimiento secular sostenido con sesgo hacia valores altos. En contraste, las exportaciones de Piura presentan altos picos y caídas, con valores atípicos marcados. El ICEN, en tanto, oscila alrededor de cero con colas extremas que reflejan los episodios Niño/Niña.
- Si bien el crédito y las exportaciones tienen una relación positiva, no se trata de un vínculo estrictamente causal. El crédito refleja condiciones financieras agregadas que evolucionan de manera estable, mientras que las exportaciones responden más rápido y con mayor intensidad a choques externos como el clima o los precios internacionales. Para validar impacto causal sería necesario aplicar modelos econométricos avanzados. 




  




