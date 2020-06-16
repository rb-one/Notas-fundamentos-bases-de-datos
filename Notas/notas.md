# Fundamentos de Bases de Datos

## Modulo 1. Bienvenida conceptos básicos y contexto histórico de las Bases de Datos

### Clase 1Expert Session: resuelve tus dudas sobre las bases de datos

### Clase 2 Bienvenida conceptos básicos y contexto histórico de las Bases de Datos

Tu profesor será Israel Vázquez, senior web developer en San Francisco, seminarista de bases de datos y entusiasta data engineering.
El almacenamiento en la nube tiene un gran pro comparada con los otros métodos de almacenamiento ya que es accesible desde cualquier parte del mundo. Además es centralizada y puede ser usada por varias personas al mismo tiempo.

Las bases de datos entran cuando hacemos la transición a medios digitales.

#### Tipos de bases de datos

**Relacionales:** En la industria hay varias compañías dedicadas a ser manejadoras de bases de datos relacionales como SQL Server, Oracle, **MariaDB**, entre otras.
**No relacionales**: Todavía están avanzando y existen ejemplos muy distintos como cassandra, elasticsearch, neo4j, MongoDB, entre otras.

#### Servicios

**Auto administrados:** Es la base de datos que instalas tú y te encargas de actualizaciones, mantenimiento, etc.
**Administrados:** Servicios que ofrecen las nubes modernas como Azure y no debes preocuparte por mantenimiento o actualizaciones.

## Modulo 2. Introducción a las bases de datos relacionales

### Clase 3 Historia de las RDB (relational data bases)

Las bases de datos surgen de la necesidad de conservar la información más allá de lo que existe en la memoria RAM.

Las bases de datos basadas en archivos eran datos guardados en texto plano, fáciles de guardar pero muy difíciles de consultar y por la necesidad de mejorar esto nacen las bases de datos relacionales. **Su inventor Edgar Codd** dejó ciertas reglas para asegurarse de que toda la filosofía de las bases de datos no se perdiera, estandarizando el proceso, **Codd invento el algebra relacional**

(Contenido adicional)
Bases de datos relacionales (RBD)

Es importante que sea fácil de guardar y extraer, anteriormente se usaban bases de datos basadas en archivos, el cuál era texto plano fácil de guardar, pero difícil de extraer, por esto se inventaron las bases de datos relacionales. En 1990 Codd se preocupó porque los sistemas de gestión de bases de datos (SGBD) que decían ser relacionales, no lo eran. En la práctica es difícil cumplir las 12 pero, un SGBD es más relacional cuantas más reglas cumpla

Las Reglas y mandamientos de Edgar Frank Ted Codd

**Regla 0:** Regla de fundación.
a) Cualquier sistema que se proclame como relacional, debe ser capaz de gestionar sus bases de datos enteramente mediante sus capacidades relacionales.

**Regla 1:** Regla de la información.
a) Todos los datos deben estar almacenados en las tablas
b) Esas tablas deben cumplir las premisas del modelo relacional
c) No puede haber información a la que accedemos por otra vía

**Regla 2:** Regla del acceso garantizado.
a) Cualquier dato es accesible sabiendo la clave de su fila y el nombre de su columna o atributo
b) Si a un dato no podemos acceder de esta forma, no estamos usando un modelo relacional

**Regla 3:** Regla del tratamiento sistemático de valores nulos.
a) Esos valores pueden dar significado a la columna que los contiene
b) El SGBD debe tener la capacidad de manejar valores nulos
c) El SGBD reconocerá este valor diferenciándolo de cualquier otro
d) El SGBD deberá aplicársele la lógica apropiada
e) Es un valor independiente del tipo de datos de la columna

**Regla 4:** Catálogo dinámico en línea basado en el modelo relacional.
a) El catálogo en línea es el diccionario de datos
b) El diccionario de datos se debe de poder consultar usando las mismas técnicas que para los datos
c) Los metadatos, por tanto, se organizan también en tablas relacionales
d) Si SELECT es una instrucción que consulta datos, también será la que consulta los metadatos

**Regla 5:** Regla comprensiva del sublenguaje de los datos completo.
a) Al menos tiene que existir un lenguaje capaz de hacer todas las funciones del SGBD
b) No puede haber funciones fuera de ese lenguaje
c) Puede haber otros lenguajes en el SGBD para hacer ciertas tareas
d) Pero esas tareas también se deben poder hacer con el “lenguaje completo”

**Regla 6:** Regla de actualización de vistas.
a) Las vistas tienen que mostrar información actualizada
b) No puede haber diferencias entre los datos de las vistas y los datos de las tablas base

**Regla 7:** Alto nivel de inserción, actualización, y cancelación.
a) La idea es que el lenguaje que maneja la base de datos sea muy humano
b) Eso implica que las operaciones del lenguaje de manipulación de los datos (DML) trabajen con conjuntos de filas a la vez
c) Para modificar, eliminar o añadir datos, no hará falta programar de la forma en la que lo hacen los lenguajes de tercera generación como C o Java

**Regla 8:** Independencia física de los datos.
a) Cambios en la física de la BD no afecta a las aplicaciones ni a los esquemas lógicos
b) El acceso a las tablas (elemento lógico) no cambia porque la física de la base de datos cambie

**Regla 9:** Independencias lógicas de los datos.
a) Cambios en el esquema lógico (tablas) de la BD no afectan al resto de esquemas
b) Si cambiamos nombres de tabla, o de columna o modificamos información de las filas, las aplicaciones (esquema externo) no se ven afectadas
c) Es más difícil de conseguir

**Regla 10:** Independencia de la integridad.
a) Las reglas de integridad (restricciones) deben de ser gestionadas y almacenadas por el SGBD

**Regla 11:** Independencia de la distribución.
a) Que la base de datos se almacene o gestione de forma distribuida en varios servidores, no afecta al uso de esta ni a la programación de las aplicaciones de usuario
b) El esquema lógico es el mismo independientemente de si la BD es distribuida o no

**Regla 12:** La regla de la no subversión.
a) La base de datos no permitirá que exista un lenguaje o forma de acceso, que permita saltarse las reglas anteriores.

### Clase 4 Entidades y atributos

Una **entidad** es algo similar a un objeto (programación orientada a objetos) y representa algo en el mundo real, incluso algo abstracto. Tienen atributos que son las cosas que los hacen ser una entidad, se diagraman dentro de cuadrados  y **por convención se ponen en plural**.

#### Atributos

Los atributos se representan con óvalos, los que tienen multiples valores llevan dobles óvalos, también existen atributos compuestos, los atributos especiales son óvalos con linea punteada.

Los **atributos compuestos** son aquellos que tienen atributos ellos mismos.

Los **atributos llave** son aquellos que identifican a la entidad y no pueden ser repetidos, se diagraman con underline. Existen:

- Naturales: Son inherentes al objeto como el número de serie
- Clave artificial: No es inherente al objeto y se asigna de manera arbitraria

![src/Atributos-rdb.png](src/Atributos-rdb.png)

#### Entidades

**Entidad Fuerte:** No depende de ninguna entidad para existir

**Entidades débiles:** No pueden existir sin una entidad fuerte y se representan con un cuadrado con doble línea.

- Identidades débiles por identidad: No se diferencian entre sí más que por la clave de su identidad fuerte.
- Identidades débiles por existencia: Se les asigna una clave propia.

![src/entidades_debiles.png](src/entidades_debiles.png)

![src/entidades_debiles_2.png](src/entidades_debiles_2.png)

Las entidades debiles pueden serlo por dos motivos:

**Por identidad:** No se diferencian entre si mas que por la clave de su entidad fuerte (clave isbn).

**Por existencia:** Usando llave asignada por nosotros (un id).

#### Clase 5 Entidades de Platzi Blog

Nuestro proyecto será un manejador de Blogpost. Es un contexto familiar y nos representará retos muy interesantes.

- Primer paso: Identificar las entidades (abstracciones del mundo real).

![src/entidades_platziblog.png](src/entidades_platziblog.png)

- Segundo paso: Pensar en los atributos.

![src/entidades_platziblog_2.png](src/entidades_platziblog_2.png)

![src/entidades_platziblog_3.png](src/entidades_platziblog_3.png)

### Clase 6 Relaciones

Las **relaciones** nos permiten ligar o unir nuestras diferentes entidades y se representan con rombos. Por convención se definen a través de verbos.

![src/relaciones.png](src/relaciones.png)

Las relaciones tienen una propiedad llamada **cardinalidad** y tiene que ver con números. Cuántos de un lado pertenecen a cuántos del otro lado:

Cardinalidad: 1 a 1
Cardinalidad: 0 a 1
Cardinalidad: 1 a N
Cardinalidad: 0 a N

#### Cardinalidad: 1 a 1

![src/cardinalidad_1_1.png](src/cardinalidad_1_1.png)

1 persona - tiene - 1 dato_contacto
1 dato_contacto - tiene - 1 persona.

#### Cardinalidad: 0 a 1

Algunos autores la denominan 1 a 1 opcional.
En el ejemplo una sesión tiene un usuario, pero no necesariamente esta loggeado todo  el tiempo

![src/cardinalidad_0_1.png](src/cardinalidad_0_1.png)

#### Cardinalidad: 1 a N (1 a muchos)

Un automóvil tiene N automóviles, pero 1 automóvil solo tiene 1 dueño.

![src/cardinalidad_1_N.png](src/cardinalidad_1_N.png)

#### Cardinalidad: 0 a N

![src/33333333333333333333333333333333333333333333333333333333333333333333.png](src/cardinalidad_0_N.png)

### Clase 7 Multiples muchos

Este tipo de cardinalidad es muy interesante por ello su clase aparte,se vera cuando veamos los campos clave.

Cardinalidad: N a N

### Clase 8 Diagrama ER

Un diagrama es como un mapa y nos ayuda a entender cuáles son las entidades con las que vamos a trabajar, cuáles son sus relaciones y qué papel van a jugar en las aplicaciones de la base de datos.

![src/diagrama_ER.png](src/diagrama_ER.png)

### Clase 9 Diagrama Físico: tipos de datos y constraints

Para llevar a la práctica un diagrama debemos ir más allá y darle detalle con parámetros como:

#### Tipos de dato

**- Texto:** CHAR(n), VARCHAR(n), TEXT
**- Números:** INTEGER, BIGINT, SMALLINT, DECIMAL(n,s), NUMERIC(n,s)
**- Fecha/hora:** DATE, TIME, DATETIME, TIMESTAMP
**- Lógicos:** BOOLEAN

Nota:

Char(8) reserva 8 espacios en memoria de forma fija, Varchar(8) hace lo mismo pero crece (1,2,3...8) de manera dinámica conforme los requieres.

#### Constraints (Restricciones)

**- NOT NULL:** Se asegura que la columna no tenga valores nulos
**- UNIQUE:** Se asegura que cada valor en la columna no se repita
**- PRIMARY KEY:** Es una combinación de NOT NULL y UNIQUE
**- FOREIGN KEY:** Identifica de manera única una tupla en otra tabla
**- CHECK:** Se asegura que el valor en la columna cumpla una condición dada
**- DEFAULT:** Coloca un valor por defecto cuando no hay un valor especificado
**- INDEX:** Se crea por columna para permitir búsquedas más rápidas, tiene la desventaja de que tiene que reindexar los registros cada vez, lo que vuelve muy lenta la operación de la bd.

### Clase 10 Diagrama Físico: normalizacion

La normalización como su nombre lo indica nos ayuda a dejar todo de una forma normal. Esto obedece a las 12 reglas de Codd y nos permiten separar componentes en la base de datos:

**Primera forma normal (1FN):** Atributos atómicos (Sin campos repetidos)
**Segunda forma normal (2FN):** Cumple 1FN y cada campo de la tabla debe depender de una clave única.
**Tercera forma normal (3FN):** Cumple 1FN y 2FN y los campos que NO son clave, NO deben tener dependencias.
**Cuarta forma normal (4FN):** Cumple 1FN, 2FN, 3FN y los campos multivaluados se identifican por una clave única.

![src/diagrama_fisico_sin_normalizar.png](src/diagrama_fisico_sin_normalizar.png)

**Primera forma normal (1FN):** Atributos atómicos (Sin campos repetidos)

![src/diagrama_fisico_1N.png](src/diagrama_fisico_1N.png)

**Segunda forma normal (2FN):** Cumple 1FN y cada campo de la tabla debe depender de una clave única.

![src/diagrama_fisico_2N.png](src/diagrama_fisico_2N.png)

**Tercera forma normal (3FN):** Cumple 1FN y 2FN y los campos que NO son clave, NO deben tener dependencias.

![src/diagrama_fisico_3N.png](src/diagrama_fisico_3N.png)

**Cuarta forma normal (4FN):** Cumple 1FN, 2FN, 3FN y los campos multivaluados se identifican por una clave única.

![src/diagrama_fisico_4N.png](src/diagrama_fisico_4N.png)

### Clase 11 Diagrama Físico: normalizando Platziblog

#### Diagram Entidad Relacion

![src/diagrama_ER.png](src/diagrama_ER.png)

#### Diagrama fisico Paso 1

Generar los campos básicos de cada entidad

![src/Diagrama_Fisico_paso_1.png](src/Diagrama_Fisico_paso_1.png)

#### Diagrama fisico Paso 2

Genera las relaciones entre cada entidad y asigna PK y FK.

![src/diagrama_fisico_paso_2.png](src/diagrama_fisico_paso_2.png)

#### Diagrama fisico Paso 3

![src/diagrama_fisico_paso_2_N_N.png](src/diagrama_fisico_paso_2_N_N.png)

Para manejar las relaciones muchos a muchos, es necesario generar una tabla intermedia de esta manera.

![src/diagrama_fisico_paso_3_N_N.png](src/diagrama_fisico_paso_3_N_N.png)

Observa que post_id y etiqueta_id usan llaves compuestas para hacer combinaciones únicas, o podemos generar también la forma anterior con un id

### Clase 12 Formas normales en DB relacionales

La normalización en las bases de datos relacionales es uno de esos temas que, por un lado es sumamente importante y por el otro suena algo esotérico. Vamos a tratar de entender las formas normales (FN) de una manera simple para que puedas aplicarlas en tus proyectos profesionales.

#### Primera Forma Normal (1FN)

Esta FN nos ayuda a eliminar los valores repetidos y no atómicos dentro de una base de datos.

Formalmente, una tabla está en primera forma normal si:

- Todos los atributos son atómicos. Un atributo es atómico si los elementos del dominio son simples e indivisibles.
- No debe existir variación en el número de columnas.
- Los campos no clave deben identificarse por la clave (dependencia funcional).
- Debe existir una independencia del orden tanto de las filas como de las columnas; es decir, si los datos cambian de orden no deben cambiar sus significados.

Se traduce básicamente a que si tenemos campos compuestos como por ejemplo “nombre_completo” que en realidad contiene varios datos distintos, en este caso podría ser “nombre”, “apellido_paterno”, “apellido_materno”, etc.

Se traduce básicamente a que si tenemos campos compuestos como por ejemplo “nombre_completo” que en realidad contiene varios datos distintos, en este caso podría ser “nombre”, “apellido_paterno”, “apellido_materno”, etc.

Los campos deben ser tales que si reordenamos los registros o reordenamos las columnas, cada dato no pierda el significado.

#### Segunda Forma Normal (2FN)

Esta FN nos ayuda a diferenciar los datos en diversas entidades.

Formalmente, una tabla está en segunda forma normal si:

- Está en 1FN
- Sí los atributos que no forman parte de ninguna clave dependen de forma completa de la clave principal. Es decir, que no existen dependencias parciales.
- Todos los atributos que no son clave principal deben depender únicamente de la clave principal.

Lo anterior quiere decir que sí tenemos datos que pertenecen a diversas entidades, cada entidad debe tener un campo clave separado. Por ejemplo:

![diagrama_fisico_1N.png](src/diagrama_fisico_1N.png)

En la tabla anterior tenemos por lo menos dos entidades que debemos separar para que cada uno dependa de manera única de su campo llave o ID. En este caso las entidades son alumnos por un lado y materias por el otro, ya que una materia. En el ejemplo anterior, quedaría de la siguiente manera:

![diagrama_fisico_2N.png](src/diagrama_fisico_2N.png)

#### Tercera Forma Normal (3FN)

Esta FN nos ayuda a separar conceptualmente las entidades que no son dependientes.

Formalmente, una tabla está en tercera forma normal si:

Se encuentra en 2FN
No existe ninguna dependencia funcional transitiva en los atributos que no son clave

Esta FN se traduce en que aquellos datos que no pertenecen a la entidad deben tener una independencia de las demás y debe tener un campo clave propio. Continuando con el ejemplo anterior, al aplicar la 3FN separamos la tabla alumnos ya que contiene datos de los cursos en ella quedando de la siguiente manera.

![diagrama_fisico_3N.png](src/diagrama_fisico_3N.png)

#### Cuarta Forma Normal (4FN)

Esta FN nos **trata de atomizar los datos multivaluados** de manera que no tengamos datos repetidos entre rows.

Formalmente, una tabla está en cuarta forma normal si:

- Se encuentra en 3FN
- Los campos multivaluados se identifican por una clave única

Esta FN trata de eliminar registros duplicados en una entidad, es decir que cada registro tenga un contenido único y de necesitar repetir la data en los resultados se realiza a través de claves foráneas.

Aplicado al ejemplo anterior la tabla materia se independiza y se relaciona con el alumno a través de una tabla transitiva o pivote, de tal manera que si cambiamos el nombre de la materia solamente hay que cambiarla una vez y se propagara a cualquier referencia que haya de ella.

![diagrama_fisico_4N](src/diagrama_fisico_4N.png)

De esta manera, aunque parezca que la información se multiplicó, en realidad la descompusimos o normalizamos de manera que a un sistema le sea fácil de reconocer y mantener la consistencia de los datos.

Algunos autores precisan una 5FN que hace referencia a que después de realizar esta normalización a través de uniones (JOIN) permita regresar a la data original de la cual partió.
