# nelsonmauri
# ARBOLES DE DESICION 
#PAQUETES DE DATOS TITANIC
#Paquete tidyverse
library(tidyverse)
library(titanic)
#cargar los datos 
data("titanic_train")
head(titanic_train)
#paquete rpart
#paquete rpart.plot
library(rpart)
library(rpart.plot)
library(rattle)
#modelo arbol de desicion 
Arbol<- rpart(
  formula = Survived ~ Sex + Age,
  data = titanic_train,
  method = "class"
)
library(bitops)
library(tibble)
library(rpart.plot)
rpart.plot(arbol)
rpart.plot(Arbol)
#predecir sobre el modelo 
predic_arbol <- predict(Arbol,type = 'class')
titanicpredic <- cbind(titanic_train,predic_arbol)
predict(object = Arbol,
        newdata = data.frame(Age = 4 ,
                             Sex ='male'),
            type = "class")
