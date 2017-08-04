# regresion-17-
#Genaro Garduño Ruiz 
Practica #1
a<-4
b<-3
suma <- a+b
suma 
#operaciones de comparacion
a > b
a >= b
a <= b 
a == b
a < b
a != b # ¿ es diferente que b?
##################
## concepto de funci 
x <- abs(-2.5)
##abs es  la funcion del valor absoluto
x
help(abs)
# para asignar valores a variables en R se usa una <- 
x<- "hola "## variable tipo caracter
z <- 6 # el igual solo funciona en una sola direccion
### en este curso loa objetos o variables que se utilizan son de 
#caracter y na 
ciudad <- "toluca"   #una entrada
nombres <- c("Karla","Rodrigo","Miguel","Samuel")
# caracter de 4 entradas
edad <- c(28,17,49,31)  #numerico de 4 entradas
#se utiliza la funcion class para preguntarle a r que tipo de variable o clase es
class(nombres)
class(edad)


base1 <- data.frame (nombres,edad)

View(base1)


ls (base1) # ver lista de variables
base1$edad = base1$edad1
base1$edad  ## conocer los datos de la variable edad de la base 1

### ejercicio crear una variable de nombre sexo con 4 entradas
#donde hombre es 1 y mujer es el valor 2,  la primera entrada
## es mujer y las otras 3 son hombres
#despues de crear variable generen una nueva base
##de nombre base 2 con 3 variables, nombre , edad  y sexo


sexo <- c(2,1,1,1)

base2<- data.frame(nombres,edad, sexo)
base2
View(base2)
table(base2$sexo)
table(base2$edad)


palumnos <- c(40,120,60,80) ## alumnos facultad de economia
etiq <- c("actua","eco","ri","neg")

help("pie")

pie (palumnos)
pie (palumnos,etiq)
pie (palumnos, etiq, main=
       "Gráfica de pie de la facultad de economía"
       ,sub=("Fuente:Facultad de economía")
     , col= c("blue","red","pink","yellow")
     , radius = 1.0, clockwise = TRUE,lty = 15
       )



