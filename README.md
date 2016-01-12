# Ecoinformatica
Repositorio de prueba que hemos hecho en Ecoinformatica
**Vamos a hacer una regresión**
Creamos una secuencia de números
```{r}
numeros <- seq(1,100, by=1)
```
De las que cogemos dos muestras al azar (x,y)
```{r}
x <- sample(numeros,50)
y <- sample(numeros,50)
```
Y las utilizamos para hacer una regresión
```{r}
reg1 <- lm(x~y)
```
Y la resumimos
```{r}
summary(reg1)
```
Y, por ultimo, representarla en una gráfica
```{r}
plot(x~y)
```