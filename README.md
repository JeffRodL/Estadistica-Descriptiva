# Estadística descriptiva

# Estadística descriptiva vs inferencial

**Ejemplo: Estadística de un jugador:** 

- Descriptiva:
    - Resumir historial deportivo.
- Inferencial:
    - Predecir desempeño futuro del jugador.

**¿Puedes mentir con estadística?**

- Dependerá de la definición de quien es el mejor jugador de fútbol.
- No hay una definición objetiva.
- Los diferentes estadísticos descriptivos dan nociones diferentes sobre los mismos datos.

![Untitled.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled.png)

## ¿Por qué aprender estadística?

- Resumir grandes cantidades de información.
- Tomar mejores decisiones (¿o peores?)
- Responder preguntas con relevancia social.
- Reconocer patrones en los datos.
- Descubrir a quienes usan estas herramientas con fines nefastos.

# Flujo de trabajo en Data Science

![Untitled%201.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%201.png)

![Untitled%202.png(Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%202.png)

> según esta clase; la ingesta de datos y validación sí es una etapa del flujo de trabajo de un proyecto de Data Science donde interviene la estadística descriptiva.
> 

El flujo de trabajo en Data Science tiene 8 pasos:

1. Data ingestion.
2. Data visualization.
3. Data preparation.
4. Model training .
5. Model evaluation.
6. Model validation.
7. Model serving.
8. En user interface.

En algunos de estos se puede aplicar la estadística, por ejemplo, en los primeros cuatro la estadística descriptiva juega un rol importante.

# Plan del curso

Sabemos y tenemos bien claro que la estadística descriptiva es súper común, pero el diferenciador más grande de este curso es que estamos contextualizando la estadística descriptiva específicamente para Ciencia de Datos. No solo vamos a entender las fórmulas matemáticas si no el contexto de la estadística para descubrir todas las caras que tiene.

## **¿Cuáles serán los puntos específicos que vamos a tratar en este curso?**

### Primer bloque

![122623879-806e8b00-d063-11eb-9330-c007c4b68ce0.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/122623879-806e8b00-d063-11eb-9330-c007c4b68ce0.png)

Vamos abordar  cuales son los elementos de estadística descriptiva para la ingesta y el procesamiento de los datos. 

Estadíticos para análitica y exploración.

### Segundo bloque

![122623878-7ea4c780-d063-11eb-9fe7-9344df6f0569.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/122623878-7ea4c780-d063-11eb-9fe7-9344df6f0569.png)

Vamos a ver análisis exploratorio de los datos, identificar correlaciones de los datos, abordaremos si a partir de eso podemos reducir el conjunto de datos que necesitamos para un modelo, por ejemplo. Entonces, el objetivo es abordar los estadísticos para exploración y analítica.

# Tipos de datos

**Categóricos**

(género, categorías, métodos, etc)

- ordinal
- nominal

**Numéricos**

(edad, altura, temperatura, etc)

- discretos
- continuos

Los datos categóricos también conocidos como datos cualitativos, representan características como el género, el idioma, etc. de una persona. También pueden tomar valores numéricos, por ejemplo: 1 para mujeres y 0 para hombres. Hay que tener en cuenta que esos números no tienen significado matemático.Los tipos de datos estadísticos categóricos se clasifican en:.

- **Datos nominales:** Otros de los tipos de datos estadísticos son los que tienen valores nominales que representan unidades discretas y se usan para etiquetar variables que no tienen un valor cuantitativo.Estos datos no tienen un orden, aunque cambiara el orden de sus valores, no cambia su significado.
- **Datos ordinales:** Los datos ordinales representan unidades discretas y ordenadas. Por lo tanto, es casi lo mismo que los datos nominales, excepto que su orden es importante.Las escalas ordinales generalmente, se usan para medir características no numéricas como la felicidad, la satisfacción del cliente, etc.

.

### Datos numéricos

Estos tipos de datos estadísticos también se conocen como datos cuantitativos, y se refieren a una medida o recuento. Se clasifican de la siguiente manera:.

- **Datos discretos:** Los datos estadísticos son discretos cuando sus valores son distintos y separados. Es decir, cuando los datos sólo pueden tomar ciertos valores.Este tipo de datos no se puede medir, pero se pueden contar. Básicamente representan información que se puede clasificar.
- **Datos continuos:** Los datos continuos representan mediciones y, por lo tanto, sus valores. no se pueden contar, pero se pueden medir. A su vez, estos se clasifican de la siguiente manera:
    - **Datos de intervalo:** Los datos de intervalo representan unidades ordenadas que tienen la misma diferencia . Por lo tanto, hablamos de datos de intervalo cuando tenemos una variable que contiene valores numéricos que están ordenados y donde conocemos las diferencias exactas entre los valores.

El problema con los datos de valores de intervalo es que podemos sumar y restar, pero no podemos multiplicar, dividir o calcular razones. Debido a que no existe un cero verdadero, no se pueden aplicar muchas estadísticas descriptivas e inferenciales..

- **Datos de relación:** También son unidades ordenadas que tienen la misma diferencia. Los datos de relación son los mismos que los valores de intervalo, con la diferencia de que tienen un cero absoluto.

# Medidas de tendencia central

- Media (promedio)
    - Es el promedio de todos los datos, puede ser susceptible a valores atípicos
- Mediana (dato central)
    - Es el dato central, es decir que tiene la misma cantidad de datos a su izquierda y derecha, no es lo mismo que la mediana
- Moda (dato que más se repite)
    - Es el dato que se repite más, la moda no aplica para datos numéricos continuos.

## Diagramas de frecuencias

Es la representación gráfica asociada a la tabla de frecuencia, normalmente todos los estadísticos descriptivos se pueden representar en términos de esta distribución.

[Untitled (1)-6c9ab365-1d8c-4325-96ab-37f9687a2371.webp](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled_(1)-6c9ab365-1d8c-4325-96ab-37f9687a2371.webp)

> **Como dato curioso e interesante:**
> 
> 
> No solo existen esas 3 medidas de tendencias central, hay otras más poco conocidas, pero las abordaremos ahora mismo:.
> 
> - **Media ponderada:** es una medida de tendencia central, que es apropiada cuando en un conjunto de datos cada uno de ellos tiene una importancia relativa (o peso) respecto de los demás datos. Se obtiene multiplicando cada uno de los datos por su ponderación (peso) para luego sumarlos, obteniendo así una suma ponderada; después se divide esta entre la suma de los pesos, dando como resultado la media ponderada.
> - **Media armónica:** La media armónica es igual al número de elementos de un grupo de cifras entre la suma de los inversos de cada una de estas cifras.En otras palabras, la media armónica es una medida estadística recíproca a la media aritmética, que es la suma de un conjunto de valores entre el número de observaciones.
> - **Media geométrica:** es una cantidad arbitraria de números (por decir n números) es la raíz n-ésima del producto de todos los números; es recomendada para datos de progresión geométrica, para promediar razones, interés compuesto y números índice.

## ¿Cuando usar cuál?

La media es susceptible a valores atípicos.

La moda no aplica para datos numéricos continuos.

# Metáfora de Bill Gates en un bar

Se tiene un data set de la forma

$$
dataset=\{x_1,x_2,...,x_n\}
$$

La media es entonces

$$
media=\overline{x}=\frac{1}{N}(x_1+x_2+...+x_n)=\frac{1}{N}\sum_{i=1}^{N}x_i
$$

La mediana se define como:

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%203.png)

# Medidas de dispersión

Medidas de dispersión más utilizadas:

- Rango
    - El rango es el intervalo entre el valor máximo y el valor mínimo.
- Cuartiles
    - Los cuartiles son valores que dividen una muestra de datos en cuatro partes iguales.
        - 1er cuartil: (Q1) 25% de los datos es menor que o igual a este valor.
        - 2do cuartil: (Q2) La mediana. 50% de los datos es menor que o igual a este valor.
        - 3er cuartil: (Q3) 75% de los datos es menor que o igua a este valor.
        - Rango intercuartil: La distancia entre el primer cuartil y el tercero (Q3-Q1), de esta manera, abarca el 50% central de los datos
- Diagrama de caja o boxplot:
    - Representa gráficamente una serie de datos numéricos a través de sus cuartiles. De esta manera, el diagrama de caja muestra a simple vista la mediana y los cuartiles de los datos. También puede representar los valores atípicos de estos.

## Desviación estandar

Sea un conjunto de dataset 

$$
dataset=\{x_1,x_2,...,x_n\}
$$

y a media definida

$$
\bar{X}=\frac{1}{N}\sum_{i=1}^{N}x_i
$$

Si se toma como valor de referencia la media, para evitar valores negativos encontrados a la izquierda, se utiliza la varianza

$$
\sigma^2=\frac{1}{n}\sum_{i=1}^{n}(x_1-\bar{x})^2
$$

donde $\sigma$ es la llamada desviación estandar.

Si el conjunto con el que se trabaja no es la población, sino con un conjunto dento de la población llamada muestra se utiliza un factor de correción

$$
\sigma=\sqrt{\frac{1}{n-1}\sum_{i=1}^{n}(x_1-\bar{x})^2}
$$

### Distribución normal o distribución gaussiana

Para una distribución normal, la mitad es justamente la mediana la cua coincide con el cuartil 2 Q2

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%204.png)

Si se asume una distribución normal ideal, entonces $\sigma$ también mide desviaciones

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%205.png)

Si tomo los valores de tres veces la desviación estandar a derecha e izquierda de la mediana, obtengo la totalidad de los datos, un 99.72% en esa distribución.

Si los datos se encuentran en este rango:

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%206.png)

con IQR el rango intercuartil. Se consideran datos “normales”. No son atípicos ni outayers. 

Si la distribución no es simétrica, el criterio anterior no es válido.

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%207.png)

Para este caso se utiliza la mismas ecuaciones con la diferencia que ahora se utilizan dos funciones dependientes de los rangos intercuartiles.

# Exploración visual de los datos

[https://www.data-to-viz.com/](https://www.data-to-viz.com/)

[https://datavizproject.com/](https://datavizproject.com/)

# Pipelines de procesamiento para variables numéricas

Una  **pipeline** de datos es una construcción lógica que representa un proceso dividido en fases.

> La combinación de una base de datos transaccional, un lenguaje de programación, un motor de procesamiento y un almacén de datos da como resultado un pipeline. - Data Engineering with Python. Packtpub
> 

## Escalamiento lineal

**¿por qué usarlos?**

Modelos de Machine Learning eficientes en el rango de -1 a 1

**¿Hay diferentes tipos?**

max-min, clipping, z-score, Winsorizing, etc

**¿Cuándo usarlos?**

Data simétrica o uniformemente distribuida

## Normalización

La normalización es una técnica que a menudo se aplica como parte de la 
preparación de datos para el aprendizaje automático. El objetivo de la 
normalización es cambiar los valores de las columnas numéricas en el 
conjunto de datos para usar una escala común, sin distorsionar las 
diferencias en los rangos de valores ni perder información. La 
normalización también es necesaria para que algunos algoritmos modelen 
los datos correctamente.

Por ejemplo, suponga que su conjunto de datos de entrada contiene una 
columna con valores que van de 0 a 1 y otra columna con valores que van 
de 10,000 a 100,000. La gran diferencia en la escala de los números 
podría causar problemas al intentar combinar los valores como 
características durante el modelado.

La normalización evita estos problemas al crear nuevos valores que 
mantienen la distribución general y las proporciones en los datos de 
origen, mientras mantienen los valores dentro de una escala aplicada en 
todas las columnas numéricas utilizadas en el modelo.

**Tenemos varias opciones para transformar datos numéricos:**

- Cambiar todos los valores a una escala de 0 a 1 o transformar los
valores representándolos como rangos de percentiles en lugar de valores
absolutos.
- Aplicar la normalización a una sola columna o a varias columnas en el mismo conjunto de datos.
- Si necesita repetir el experimento o aplicar los mismos pasos de
normalización a otros datos, puede guardar los pasos como una
transformación de normalización y aplicarlos a otros conjuntos de datos
que tengan el mismo esquema.

> Nota importante: Algunos algoritmos requieren que los datos se 
normalicen antes de entrenar un modelo. Otros algoritmos realizan su 
propia normalización o escalado de datos.
> 

### Normalización lineal

**Algunos de los tipos:**

- **Zscore :** convierte todos los valores en una puntuación z. Los valores de la columna se transforman mediante la siguiente fórmula:

$$
z=\frac{\mathrm{x}-mean(x)}{stdev(x)}=\frac{x-\bar{x}}{\sigma}
$$

La media y la desviación estándar se calculan para cada columna por separado. Se utiliza la desviación estándar de la población.

- **MinMax :** el normalizador min-max cambia la escala
linealmente cada característica al intervalo [0,1]. El cambio de escala al intervalo [0,1] se realiza cambiando los valores de cada característica para que el valor mínimo sea 0, y luego dividiendo por el nuevo valor máximo (que es la diferencia entre los valores máximo y mínimo originales). Los valores de la columna se transforman mediante la siguiente fórmula:

$$
z=\frac{x-min(x)}{[max(x)-min(x)]}
$$

**¿Cuándo usar la normalización lineal?**

- En datos simétricos o en datos uniformemente distribuidos.

> el Zscore tambien te lo puedes topar como StandartScaler.
> 

### La formula general de normalización estadística

Anteriormente se presento la normalización para rangos de [0,1], pero si los rangos deseados son otros, entonces se suele recurrir a su forma más general de escalamiento min-max:

$$
X'=a+\frac{(X-X_{min})(b-a)}{X_{max}-X_{min}}
$$

donde el rango de valores se encuentra entre ***a y b.***

# Transformación no lineal

**¿Por qué usarlos?**

- En el caso donde haya datos fuertemente sesgados y no simétricos.

**¿Hay diferentes tipos?**

- Logaritmos, sigmoides, polinomiales, etc.

**¿Cuándo usarlos?**

- Antes de escalamientos lineales.

**Algunos tipos:**

- **Logística:** los valores de la columna se transforman mediante la siguiente fórmula:

$$
Z =\frac{1}{1+exp(-x)}
$$

- **LogNormal:** esta opción convierte todos los valores a una escala logarítmica normal. Los valores1 de la columna se
transforman mediante la siguiente fórmula:

$$
z= Ln.cdf(x;;\bar{x},\sigma)
$$

Aquí μ y σ son los parámetros de la distribución, 
calculados empíricamente a partir de los datos como estimaciones de 
máxima verosimilitud, para cada columna por separado.

- **TanH:** todos los valores se convierten a una
tangente hiperbólica. Los valores de la columna se transforman mediante
la siguiente fórmula:

$$
P(k|x;\theta)=\frac{[E(y|x)]^ke^{E(y|k)}}{k!}
$$

**¿Cuándo usarlos?**

Justo antes de aplicar el escalamiento lineal, las transformaciones 
no lineales solo son para que nuestros datos queden lineales para luego 
aplicar la normalización lineal. Siempre se debe aplicar la 
normalización lineal.

# Pipelines de procesamiento para variables categóricas

## Mapeos numéricos:

**Dummy:**

- Representación compacta.
- Mejor para inputs lineamente independientes. (No tiene grado de correlación significativo)

Realiza un mapeo de un valor categórico a un valor numérico.  Es mejor cuando sabemos que las categorías son diferentes entre si.

**One-hot**

- Permite describir categorías no incluidas inicialmente.

Permite representar todas las categorías de tal forma que cuando llegue una categoría desconocida, el one hot también lo pueda representar.

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%208.png)

# Correlaciones

La correlación es una medida estadística que expresa hasta qué punto dos variables están relacionadas linealmente (esto es, cambian conjuntamente a una tasa constante)

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%209.png)

La covarianza:

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%2010.png)

Coeficiente de correlación: (el p value)

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%2011.png)

## ¿Qué es la covarianza?

- Es un valor que indica el grado de variación conjunta de dos variables aleatorias respecto a sus medias.

### ¿Qué es el coeficiente de correlación?

- El coeficiente de correlación es la medida específica que cuantifica la intensidad de la relación lineal entre dos variables en un análisis de correlación.

![0AKQKBi.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/0AKQKBi.png)

# Matriz de covarianza

Una matriz de varianzas-covarianzas es una matriz cuadrada que contiene las varianzas y covarianzas asociadas con diferentes variables. Los elementos de la diagonal de la matriz contienen las varianzas de las variables, mientras que los elementos que se encuentran fuera de la diagonal contienen las covarianzas entre todos los pares posibles de variables.

![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%2012.png)

Cuando se tienen más de 2 variables se calculan todas las posibles covarianzas de las parejas de datos, esto se organiza en una matriz y se obtiene lo que se conoce como una matriz de covarianza.

Esta se representa con la letra sigma mayúscula Sigma.

- Los valores de la diagonal dan valores muy altos porque evidentemente cada variable está muy correlacionada consigo misma.
- Los elementos que se encuentran fuera de la diagonal contienen las covarianzas entre todos los pares posibles de variables.

.

**¿Qué hace el StandardScaler() de Scikit Learn?**

Normaliza los datos restando el promedio y dividiendo sobre la desviación estándar en cada variable (Z-Score).

Nota: para calcular la matriz de correlaciones hay que obtener la transpuesta del Array con los datos escalados.

.

**¿Cómo se calcula la matriz de covarianza con Python?**

Método cov() de Numpy: covariance_matrix = np.cov(scaled.T)

Método corr() de Pandas: corr_matrix = df.corr()

# Calculo de valores propios de una matriz

Cuando tenemos un conjunto de datos con muchas variables, la matriz de covarianza es el objeto matemático que permite identificcar cuáles variables están altamente relacionadas.

Cuando dos variables están altamente correlacionadas, quiere decir que aportan básicamente la misma información del problema y eso podría indicar que solo necesitariamos una sola de ellas. Esta técnica está basada en un concepto del álgebra de vectores y matrices, que llamamos el cálculo de los valores propios de una matriz y en esta lectura profundizaremos sobre qué significa ese procedimiento.

Las matrices son en general objetos matemáticos que tienen un cierto número de filas y columnas. Las matrices tienen una operación especial que llamamos transponer, la cual consiste en ubivar cada fila como columna en una nueva matriz, el resultado se denomina la matriz transpuesta 

![zEGhv9B.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/zEGhv9B.png)

Así también las matrices, entre las matrices podemos definir reglas de suma y resta de forma similar a como hacemos con los números naturales o decimales, con una condición especial: ambas matrices deben tener las mismas dimensiones y cuando las dimensiones de una matriz son iguales entre ellas decimos que es una matriz cuadrada.

Una matriz inversa se define tal que 

![kEiv8fB.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/kEiv8fB.png)

El cálculo de matriz inversa se hace rápido usando NumPy así:

```python
A = np.array([[2, 4], [-1, 2]])
Ainversa = np.linalg.inv(A)

```

Donde, el resultado de `Ainversa` en este caso particular sería:

```python
array([[ 0.25 , -0.5  ],
	[ 0.125,  0.25 ]])
```

Como caso particular adicional a la definición anterior, consideremos el producto de una matriz cuadrada por un vector (aquí entendemos un vector como una matriz de una sola columna, también se le denomina por eso vectores columna en muchos libros de álgebra lineal) cuya longitud es igual al número de filas de la matriz así

![1aFGNYg.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/1aFGNYg.png)

Donde definimos que el producto de una matriz por un vector resulta en otro vector de las mismas dimensiones (filas). Y la regla que consideramos para el caso de matrices cuadradas también aplica de manera que los elementos del vector resultante se obtendrían de multiplicar filas por columnas así:

![9vuSATV.png](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/9vuSATV.png)

También tenemos una operación entre vectores que denominamos el producto punto o producto interior. Normalmente al considerar esta definición se representa el primer vector como una sola fila y el segundo como una sola columna así (sigamos pensando con base en el ejemplo anterior de la matriz por el vector, pero ahora la matriz solo tiene una fila):

![https://i.imgur.com/596zIHK.png](https://i.imgur.com/596zIHK.png)

Y como ya te estás dando cuenta (teniendo en mente la misma definición de multiplicación de matrices) al solo haber una fila en la primera matriz y una columna en la segunda matriz, el resultado solo podrá tener un elemento y es por esto que el resultado de multiplicar dos vectores de esta manera es siempre un número:

![https://i.imgur.com/IGNqY7n.png](https://i.imgur.com/IGNqY7n.png)

Simplifiquemos la notación así:

![https://i.imgur.com/ONdFb8h.png](https://i.imgur.com/ONdFb8h.png)

Y esto nos recuerda la clásica regla de multiplicar vectores como *x por x más y por y*. Y si los vectores tienen más dimensiones, entonces *… más z por z* y así. Recuerda que la notación simplificada es porque ahora tenemos que la primera componente es el eje X del vector y la segunda componente el eje Y del vector cuando lo dibujamos en un plano cartesiano.

![https://i.imgur.com/bP7C40X.png](https://i.imgur.com/bP7C40X.png)

Ahora, cuando pensamos en multiplicar un vector por el mismo, la misma definición aplica:

![https://i.imgur.com/doQIHFe.png](https://i.imgur.com/doQIHFe.png)

Y nos damos cuenta de que esto se relaciona con el Teorema de Pitágoras al ver que el producto de un vector por el mismo nos da el cuadrado de la longitud de la flecha que representa al vector en el plano cartesiano:

![https://i.imgur.com/7441gI8.png](https://i.imgur.com/7441gI8.png)

![https://i.imgur.com/qzk7KN3.png](https://i.imgur.com/qzk7KN3.png)

Así vemos que la longitud de un vector, también conocida como norma del vector se calcula como:

![https://i.imgur.com/OUmWoRs.png](https://i.imgur.com/OUmWoRs.png)

Listo, con esto terminamos un repaso básico de lo mínimo de matrices y vectores para lo que viene.

## Vectores y Valores propios de una matriz

En álgebra lineal podemos tener ecuaciones donde la incógnita es un vector, supongamos la siguiente ecuación:

![https://i.imgur.com/mee9AMt.png](https://i.imgur.com/mee9AMt.png)

Aquí A es una matriz cuadrada NxN cuyos elementos conocemos perfectamente y X es un vector columna cuyas componentes desconocemos. Aquí recordemos que multiplicar un vector por un número es simplemente multiplicar cada componente del vector por dicho número.

Entonces lo que esta ecuación nos pregunta es:

¿Existen vectores X tales que al multiplicarlos por la matriz A eso es equivalente a simplemente multiplicarlos por un número?

Si tal vector existe y está asociado a un valor específico de , entonces decimos que el vector X es un **vector propio de la matriz A** y x es su **valor propio correspondiente**.

Consideremos esto para el caso de una matriz 2 x 2, como la siguiente:

![https://i.imgur.com/5AlP07v.png](https://i.imgur.com/5AlP07v.png)

Esto se traduce en el sistema de ecuaciones (haciendo el producto matriz por vector):

![https://i.imgur.com/LVyLKYe.png](https://i.imgur.com/LVyLKYe.png)

Aquí entonces debemos encontrar las combinaciones de x, y e que satisfacen el sistema de ecuaciones. En general, hacer esto requiere otros conceptos más detallados del álgebra de matrices como el cálculo de determinantes y resolver ecuaciones polinomiales cuya explicación solo puede dejarse a un [curso exclusivo de álgebra lineal](https://platzi.com/cursos/algebra-lineal/). Pero no te preocupes, ya que podemos hacer este cálculo de manera rápida con python así:

```
import numpyas np

A = np.array([[1, 2], [1, 0]])
values, vectors = np.linalg.eig(A)

```

Donde la **matriz A** contiene los elementos exactos de la matriz anterior y el comando `np.linalg.eig(A)` lo que hace es calcular directamente los valores y vectores propios, llamados **values y vectors** en el código, respectivamente.

Verás que esta matriz tiene dos valores propios:

```
array([ 2., -1.])

```

Con sus respectivos vectores propios asociados:

```
array([[ 0.89442719, -0.70710678 ],
	[ 0.4472136 , 0.70710678 ]])

```

Aquí es importante anotar que los vectores que entrega la función `np.linalg.eig(A)` son vectores columna de manera que los elementos de la primera columna de `vectors` corresponden con el primer valor de `values` y así sucesivamente. Entonces en nuestro lenguaje matemático usual, escribimos las dos soluciones como:

![https://i.imgur.com/7k3ZwIF.png](https://i.imgur.com/7k3ZwIF.png)

![https://i.imgur.com/ZsJ3LAt.png](https://i.imgur.com/ZsJ3LAt.png)

Puedes verificar que cada vector y su respectivo valor propio cumplen la ecuación original ejecutando cada parte así:

```
np.matmul(A, vectors.T[1])

```

Que te da como resultado:

```
array([ 0.70710678, -0.70710678])

```

Mientras que por otro lado calculando:

```
values[1]*vectors.T[1]

```

Resulta en lo mismo:

```
array([ 0.70710678, -0.70710678])

```

Donde hemos considerado el segundo vector y valor propio respectivamente tomando `λ = -1` y el vector incógnita `X` igual a `vectors.T[1]`.

Uno de los hechos más importantes de obtener los vectores y valores propios de una matriz es poder diagonalizarla. En general se define que una matriz A es diagonalizable si es posible escribirla como el producto de:

![https://i.imgur.com/yWyi48D.png](https://i.imgur.com/yWyi48D.png)

Donde D es una matriz diagonal (matriz donde todos los elementos por fuera de la diagonal son cero), un ejemplo de matriz diagonal sería:

![https://i.imgur.com/tRw3bAM.png](https://i.imgur.com/tRw3bAM.png)

Y aquí un resultado matemático bien conocido es que si una matriz es diagonalizable, la matriz D se construye colocando sus valores propios en la diagonal y la matriz P se construye colocando en cada columna el vector propio,siguiendo el mismo orden de valores propios correspondientes de la matriz D, así:

![https://i.imgur.com/NNiVLu3.png](https://i.imgur.com/NNiVLu3.png)

Lo importante de estudiar este procedimiento en nuestro curso, es que cuando aplicamos este cálculo de vectores y valores propios a una **matriz de covarianza**, los vectores representan las direcciones a lo largo de las cuales percibimos la mayor cantidad de varianza de ese conjunto de datos, donde la cantidad de varianza es proporcional al valor propio de cada vector propio.

Y es importante tener en cuenta que este procedimiento aplica para un conjunto de datos con N variables al que le corresponde una matriz de covarianza de tamaño NxN.

Ahora, el último factor importante de esta técnica es que para matrices de covarianza, sus vectores propios siempre son independientes unos de otros y esto es justamente lo que queremos en un proceso de reducción de variables, porque direcciones independientes implica que estos vectores representan nuevas variables cuya correlación es la más baja posible y así cada nueva variable es lo más representativa posible.

En álgebra lineal se dice más precisamente que los vectores propios de una matriz de covarianza son ortogonales y esto quiere decir que el producto interno de cualquier par de estos vectores siempre da como resultado cero:

![https://i.imgur.com/IygBQDo.png](https://i.imgur.com/IygBQDo.png)

Como consecuencia la matriz se denomina matriz ortogonal, y se sabe en matemáticas que la inversa de una matriz ortogonal es igual a la transpuesta, de manera que:

![https://i.imgur.com/20Iqk5V.png](https://i.imgur.com/20Iqk5V.png)


![Untitled](Estadi%CC%81stica%20descriptiva%201872ac93d43e4d45bbd44a85b2ab781a/Untitled%2013.png)
