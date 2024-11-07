# Filtrar y manipular data frames
#### > _especies <- data.frame(especie = c("Ajolote", "Rana", "Serpiente", "Tortuga"), habitat = c("Lago", "Río", "Bosque", "Lago"),tamano = c(30, 10, 150, 50),peso = c(150, 25, 1000, 500) )_
## Filtrar todas las especies que viven en un lago.
#### >_install.packages("dplyr")_
#### > _habitad_lago <- especies[especies$habitat == "Lago", ]
#### > _habitad_lago_

> ![image](https://github.com/user-attachments/assets/65f70586-d862-4d3c-a87d-6e6a87de3445)
## Ordenar los resultados por tamaño (de mayor a menor).
#### > _Tamaño <-especies[order(-especies$tamano), ]_
#### > _Tamaño_

![image](https://github.com/user-attachments/assets/93f47c69-cde9-49bd-a9c2-6d425151e509)

# Generación de gráficos
#### >_install.packages("tidyverse")_
#### > _ggplot(iris, aes(x = Sepal.Length, y = Sepal.Width, color = Species)) geom_point(size = 3) + labs(title = "Relación entre Largo y Ancho de Sépalo", x = "Largo del Sépalo", y = "Ancho del Sépalo") theme_minimal() scale_color_manual(values = c("setosa" = "blue", "versicolor" = "black", "virginica" = "purple"))_

![image](https://github.com/user-attachments/assets/c7ff104b-c45d-4c44-8cae-7e31d4165835)

#	Agrupar datos y realizar cálculos agregados
## Agrupar las calificaciones por estudiante y calcular el promedio de calificación por cada uno.
#### >_calificaciones <- data.frame(estudiante = c("Ana", "Carlos", "Lucía", "Jorge", "Ana", "Carlos", "Lucía", "Jorge"), asignatura = c("Matemáticas", "Matemáticas", "Matemáticas", "Matemáticas", "Historia", "Historia", "Historia", "Historia"),calificacion = c(95, 85, 92, 88, 78, 82, 85, 90))_

#### >_install.packages("dplyr")_
#### >_ install.packages("magrittr")_

![image](https://github.com/user-attachments/assets/1cc94579-c8eb-4cdc-8574-36230eb8b9e2)

# Transformación de datos y crear nuevas variables
#### >_alturas <- data.frame( nombre = c("Laura", "Pedro", "Sara", "Miguel"),altura_cm = c(160, 175, 150, 180))_
#### > _alturas$altura_metros <- alturas$altura_cm / 100_
#### > _alturas_

![image](https://github.com/user-attachments/assets/5fc6c884-57b7-4ceb-9a53-a7ee84efb56f)

# Generación de gráficos de barras
#### >_ventas <- data.frame(
  mes = c("Enero", "Febrero", "Marzo", "Abril", "Mayo", "Junio"),
  ventas = c(12000, 15000, 13000, 16000, 17500, 14000)
)_
#### >_ ggplot(ventas, aes(x = mes, y = ventas)) + geom_bar(stat = "identity", fill = "purple", color = "black") + labs(title = "Ventas Mensuales", x = "Mes", y = "Ventas") + theme_minimal()

![image](https://github.com/user-attachments/assets/3ee907f3-d31a-4aef-a9a0-1e5105513fa5)







