# Filtrar y manipular data frames
#### > _especies <- data.frame(especie = c("Ajolote", "Rana", "Serpiente", "Tortuga"), habitat = c("Lago", "Río", "Bosque", "Lago"),tamano = c(30, 10, 150, 50),peso = c(150, 25, 1000, 500) )_
## Filtrar todas las especies que viven en un lago.
#### ""r > _habitad_lago <- especies[especies$habitat == "Lago", ]""
#### > _habitad_lago_

> ![image](https://github.com/user-attachments/assets/65f70586-d862-4d3c-a87d-6e6a87de3445)
## Ordenar los resultados por tamaño (de mayor a menor).
> _Tamaño <-especies[order(-especies$tamano), ]_
> _Tamaño_


