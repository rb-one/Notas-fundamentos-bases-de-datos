
![badge](src/badge.webp)

# Fundamentos de Bases de Datos

## Indice

- [Fundamentos de Bases de Datos](#fundamentos-de-bases-de-datos)
  - [Indice](#indice)
  - [Modulo 1. Bienvenida conceptos básicos y contexto histórico de las Bases de Datos](#modulo-1-bienvenida-conceptos-básicos-y-contexto-histórico-de-las-bases-de-datos)
    - [Clase 1Expert Session: resuelve tus dudas sobre las bases de datos](#clase-1expert-session-resuelve-tus-dudas-sobre-las-bases-de-datos)
    - [Clase 2 Bienvenida conceptos básicos y contexto histórico de las Bases de Datos](#clase-2-bienvenida-conceptos-básicos-y-contexto-histórico-de-las-bases-de-datos)
      - [Tipos de bases de datos](#tipos-de-bases-de-datos)
      - [Servicios](#servicios)
  - [Modulo 2. Introducción a las bases de datos relacionales](#modulo-2-introducción-a-las-bases-de-datos-relacionales)
    - [Clase 3 Historia de las RDB (relational data bases)](#clase-3-historia-de-las-rdb-relational-data-bases)
    - [Clase 4 Entidades y atributos](#clase-4-entidades-y-atributos)
      - [Atributos](#atributos)
      - [Entidades](#entidades)
      - [Clase 5 Entidades de Platzi Blog](#clase-5-entidades-de-platzi-blog)
    - [Clase 6 Relaciones](#clase-6-relaciones)
      - [Cardinalidad: 1 a 1](#cardinalidad-1-a-1)
      - [Cardinalidad: 0 a 1](#cardinalidad-0-a-1)
      - [Cardinalidad: 1 a N (1 a muchos)](#cardinalidad-1-a-n-1-a-muchos)
      - [Cardinalidad: 0 a N](#cardinalidad-0-a-n)
    - [Clase 7 Multiples muchos](#clase-7-multiples-muchos)
    - [Clase 8 Diagrama ER](#clase-8-diagrama-er)
    - [Clase 9 Diagrama Físico: tipos de datos y constraints](#clase-9-diagrama-físico-tipos-de-datos-y-constraints)
      - [Tipos de dato](#tipos-de-dato)
      - [Constraints (Restricciones)](#constraints-restricciones)
    - [Clase 10 Diagrama Físico: normalizacion](#clase-10-diagrama-físico-normalizacion)
    - [Clase 11 Diagrama Físico: normalizando Platziblog](#clase-11-diagrama-físico-normalizando-platziblog)
      - [Diagram Entidad Relacion](#diagram-entidad-relacion)
      - [Diagrama fisico Paso 1](#diagrama-fisico-paso-1)
      - [Diagrama fisico Paso 2](#diagrama-fisico-paso-2)
      - [Diagrama fisico Paso 3](#diagrama-fisico-paso-3)
    - [Clase 12 Formas normales en DB relacionales](#clase-12-formas-normales-en-db-relacionales)
      - [Primera Forma Normal (1FN)](#primera-forma-normal-1fn)
      - [Segunda Forma Normal (2FN)](#segunda-forma-normal-2fn)
      - [Tercera Forma Normal (3FN)](#tercera-forma-normal-3fn)
      - [Cuarta Forma Normal (4FN)](#cuarta-forma-normal-4fn)
  - [Modulo 3 RDBMS (MySQL) o cómo hacer lo anterior de manera práctica](#modulo-3-rdbms-mysql-o-cómo-hacer-lo-anterior-de-manera-práctica)
    - [Clase 13 RDB Qué](#clase-13-rdb-qué)
    - [Clase 14 Instalación local de un RDBMS (Windows)](#clase-14-instalación-local-de-un-rdbms-windows)
    - [Clase 15  Instalación local de un RDBMS (Mac)](#clase-15-instalación-local-de-un-rdbms-mac)
    - [Clase 16 Instalación local de un RDBMS (Ubuntu)](#clase-16-instalación-local-de-un-rdbms-ubuntu)
    - [Clase 17 Clientes Graficos](#clase-17-clientes-graficos)
    - [Clase 18 Servicios administrados](#clase-18-servicios-administrados)
  - [Modulo 4 SQL hasta en la sopa](#modulo-4-sql-hasta-en-la-sopa)
    - [Clase 19 Historia de SQL](#clase-19-historia-de-sql)
    - [Clase 20 DDL create](#clase-20-ddl-create)
    - [Clase 21 CREATE VIEW y DDL ALTER](#clase-21-create-view-y-ddl-alter)
      - [Create view](#create-view)
      - [Alter Table](#alter-table)
      - [Drop Column Borrando una columna](#drop-column-borrando-una-columna)
    - [Clase 22 DDL drop](#clase-22-ddl-drop)
    - [Clase 23 DML](#clase-23-dml)
      - [Insert](#insert)
      - [Update](#update)
      - [Delete](#delete)
      - [Select](#select)
    - [Clase 24 Que tan standard es SQL](#clase-24-que-tan-standard-es-sql)
    - [Clase 25 Creando Platziblog: tablas independientes](#clase-25-creando-platziblog-tablas-independientes)
    - [Clase 26 Creando Platziblog: tablas transitivas](#clase-26-creando-platziblog-tablas-transitivas)
    - [Clase 27 Creando Platziblog: tablas transitivas](#clase-27-creando-platziblog-tablas-transitivas)
      - [Reverse Engineer](#reverse-engineer)
    - [Clase 28 Por qué las consultas son tan importantes](#clase-28-por-qué-las-consultas-son-tan-importantes)
    - [Clase 29 Estructura básica de un Query](#clase-29-estructura-básica-de-un-query)
      - [Primer Consulta](#primer-consulta)
    - [Clase 30 SELECT](#clase-30-select)
    - [Clase 31 FROM](#clase-31-from)
    - [Clase 32 Utilizando la sentencia FROM](#clase-32-utilizando-la-sentencia-from)
    - [Clase 33 WHERE](#clase-33-where)
    - [Clase 34 Utilizando la sentencia WHERE nulo y no nulo](#clase-34-utilizando-la-sentencia-where-nulo-y-no-nulo)
    - [Clase 35 GROUP BY](#clase-35-group-by)
    - [Clase 36 ORDER BY y HAVING](#clase-36-order-by-y-having)
    - [Clase 37 El interminable agujero de conejo (Nested queries)](#clase-37-el-interminable-agujero-de-conejo-nested-queries)
    - [Clase 38 Como convertir una pregunta en un query SQL](#clase-38-como-convertir-una-pregunta-en-un-query-sql)
      - [De pregunta a Query](#de-pregunta-a-query)
    - [Clase 39 Preguntandole a la base de datos](#clase-39-preguntandole-a-la-base-de-datos)
    - [Clase 40 Consultando PlatziBlog](#clase-40-consultando-platziblog)
  - [Modulo 4 Introduccion a la bases de datos NO relacionales](#modulo-4-introduccion-a-la-bases-de-datos-no-relacionales)
    - [Clase 41 Que son y cuales son los tipos de bases de datos no relacionales](#clase-41-que-son-y-cuales-son-los-tipos-de-bases-de-datos-no-relacionales)
      - [Tipos de bases de datos no relacionales:](#tipos-de-bases-de-datos-no-relacionales)
    - [Clase 42 Servicios administrados y jerarquía de datos](#clase-42-servicios-administrados-y-jerarquía-de-datos)
  - [Modulo 5 Manejo de modelos de datos en bases de datos no relacionales](#modulo-5-manejo-de-modelos-de-datos-en-bases-de-datos-no-relacionales)
    - [Clase 43 Top level collection con Firebase](#clase-43-top-level-collection-con-firebase)
    - [Clase 44 Creando y borrando documentos en Firestore](#clase-44-creando-y-borrando-documentos-en-firestore)
    - [Clase 45 Colecciones vs subcolecciones](#clase-45-colecciones-vs-subcolecciones)
    - [Clase 46 Recreando Platziblog](#clase-46-recreando-platziblog)
    - [Clase 47 Construyendo Platziblog en Firestore](#clase-47-construyendo-platziblog-en-firestore)
    - [Clase 48 Proyecto final: transformando tu proyecto en una db no relacional](#clase-48-proyecto-final-transformando-tu-proyecto-en-una-db-no-relacional)
      - [Regla 1. Piensa en la vista de tu aplicación](#regla-1-piensa-en-la-vista-de-tu-aplicación)
  - [Modulo 6 Bases de datos en la vida real](#modulo-6-bases-de-datos-en-la-vida-real)
    - [Clase 49 Bases de datos en la vida real](#clase-49-bases-de-datos-en-la-vida-real)
    - [Clase 50 Big Data](#clase-50-big-data)
    - [Clase 51 Data warehouse](#clase-51-data-warehouse)
    - [Clase 52 Data mining](#clase-52-data-mining)
    - [Clase 53 ETL](#clase-53-etl)
    - [Clase 54 Business intelligence](#clase-54-business-intelligence)
    - [Clase 55 Machine Learning](#clase-55-machine-learning)
    - [Clase 56 Data Science](#clase-56-data-science)
    - [Clase 57 Por que aprender bases de datos hoy](#clase-57-por-que-aprender-bases-de-datos-hoy)
  - [Bonus](#bonus)
    - [Clase 58 Bases de datos relacionales vs no relacionales](#clase-58-bases-de-datos-relacionales-vs-no-relacionales)

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

![image](https://user-images.githubusercontent.com/114417877/196577914-49c6a91d-2f7f-4d34-8aca-15ce078e458f.png)


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

Char(8) reserva 8 espacios en memoria de forma fija, Varchar(8) hace lo mismo pero crece (1,2,3...8) de manera dinámica conforme los requieres y tiene un limite general de 255 caracteres.

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

## Modulo 3 RDBMS (MySQL) o cómo hacer lo anterior de manera práctica

### Clase 13 RDB Qué

**RDBMS** significa Relational Database Management System o sistema manejador de bases de datos relacionales. Es un programa que se encarga de seguir las reglas de Codd y se puede utilizar de manera programática.

### Clase 14 Instalación local de un RDBMS (Windows)

Hay dos maneras de acceder a manejadores de bases de datos:

- Instalar en máquina local un administrador de bases relacional.
-Tener ambientes de desarrollo especiales o servicios cloud.

En este curso usaremos MySQL porque tiene un impacto histórico siendo muy utilizado y además es software libre y gratuito. La versión 5.6.43 es compatible con la mayoría de aplicaciones y frameworks.

- Root es el usuario principal que tendrá todos los permisos y por lo tanto en ambientes de producción hay que tener mucho cuidado al configurarlo.

Link
<https://dev.mysql.com/downloads/windows/installer/5.6.html>

Procedimiento:

- Descargamos e instalamos como es usual en windows
- En el instalador seleccionamos la opción custom
- Instalamos MySQL Server la version 64bts
- Instalamos MySQL Workbench (ignoramos lo demás)

![Instalador_mysql_1](src/Instalador_mysql_1.png)
![Instalador_mysql_2](src/Instalador_mysql_2.png)
![Instalador_mysql_3](src/Instalador_mysql_3.png)

### Clase 15  Instalación local de un RDBMS (Mac)

La instalación es similar al todos los instaladores en mac, descarga el archivo .dmg

<https://dev.mysql.com/downloads/workbench/>

Para macOS debes descargar workbench aparte.

<https://dev.mysql.com/downloads/mysql/5.7.html>

### Clase 16 Instalación local de un RDBMS (Ubuntu)

Visita la dirección de descarga de la versión de comunidad de MySql
<https://dev.mysql.com/downloads/mysql/5.7.html#downloads>

Dirígete a la sección de selección de descargas y selecciona tu distribución de Linux. En nuestro caso Ubuntu y selecciona posteriormente la versión que estás utilizando actualmente, en nuestro caso 18.04 de 64 bits.

Los pasos son similares a los otros sistemas, descarga el paquete .deb, también puedes instalar desde la consola

sudo apt-get install mysql-server

### Clase 17 Clientes Graficos

Observamos el preview y pasos para crear un schema en Mysql workbench

![worckbench_1](src/worckbench_1.png)

![worckbench_2](src/worckbench_2.png)

![worckbench_3](src/worckbench_3.png)

### Clase 18 Servicios administrados

Hoy en día muchas empresas ya no tienen instalados en sus servidores los RDBMS sino que los contratan a otras personas. Estos servicios administrados cloud te permiten concentrarte en la base de datos y no en su administración y actualización.

Introducción a google cloud, toma el curso para configurarlo.

## Modulo 4 SQL hasta en la sopa

### Clase 19 Historia de SQL

**SQL** significa Structured Query Language y tiene una estructura clara y fija. Su objetivo es hacer un solo lenguaje para consultar cualquier manejador de bases de datos volviéndose un gran estándar.

Ahora existe el **NOSQL** o Not Only Structured Query Language que significa que no sólo se utiliza SQLen las bases de datos no relacionales.

### Clase 20 DDL create

SQL tiene dos grandes sublenguajes:

**DDL o Data Definition Language** que nos ayuda a crear la estructura de una base de datos. Existen 3 grandes comandos:

**- Create**: Nos ayuda a crear bases de datos, tablas, vistas, índices, etc.

-**Alter**: Ayuda a alterar o modificar entidades.

**- Drop**: Nos ayuda a borrar. Hay que tener cuidado al utilizarlo.

**3 objetos que manipularemos con el lenguaje DDL:**

- Database o bases de datos
- Table o tablas. Son la traducción a SQL de las entidades
- View o vistas: Se ofrece la proyección de los datos de la base de datos de forma entendible.

![SQL_create_database](src/SQL_create.png)

![SQL_create](src/SQL_create_database.png)

Seleccionamos el schema  como default, de forma gráfica aunque con la terminal seria el use database.

![worckbench_default_schema.png](src/worckbench_default_schema.png)

El comando Create Table

![create_table_slide](src/create_table_slide.png)

El creamos con workbench la tabla anterior, definimos  cada uno de los campos de manera sencilla posterior damos apply

![worckbench_new_table_1.png](src/worckbench_new_table_1.png)

![worckbench_new_table_2_apply.png](src/worckbench_new_table_2_apply.png)

![worckbench_new_table_3.png](src/worckbench_new_table_3.png)

### Clase 21 CREATE VIEW y DDL ALTER

#### Create view

![workbench_create_view.png](src/workbench_create_view.png)

Para iniciar el ejercicio insertamos datos en la BD,  copiamos la sentencia
`SELECT * FROM platziblog.people;`, nos movemos a views y damos click derecho y create view.

Views ya cuenta con la parte inicial de la sentencia de create view, pegamos debajo el select y damos apply

```mysql
CREATE VIEW 'new_view' AS
SELECT * FROM platziblog.people;
```

![create_view1](src/create_view1.png)

![create_view2](src/create_view2.png)

![create_view3](src/create_view3.png)

![create_view4](src/create_view4.png)

Parece redundante la información, pero podemos estructurar las consultas junto con otras tablas, y estas vistas mantendrán la consulta sin necesidad de acer la de nuevo incrementando los  datos de forma automática.

#### Alter Table

!![alter_table_1](src/alter_table_1.png)

!![alter_table_2](src/alter_table_2.png)

!![alter_table_3](src/alter_table_3.png)

!![alter_table_4](src/alter_table_4.png)

!![alter_table_1](src/alter_table_1.png)

#### Drop Column Borrando una columna

Click derecho y deled selected

!![drop_column_1](src/drop_column_1.png)

!![drop_column_1](src/drop_column_2.png)

### Clase 22 DDL drop

Está puede ser la sentencia ¡más peligrosa! (????), sobre todo cuando somos principiantes. Básicamente borra o desaparece de nuestra base de datos algún elemento.

Pasos para borrar una tabla

![drop_table](src/drop_table.png)

![drop_table_1](src/drop_table_1.png)

![drop_table_2](src/drop_table_2.png)

![drop_table_3](src/drop_table_3.png)

Pasos para borrar la base de datos o schema

![drop_schema_1](src/drop_schema_1.png)

![drop_schema_2](src/drop_schema_2.png)

![drop_schema_3](src/drop_schema_3.png)

![drop_schema_4](src/drop_schema_4.png)

Nota: las herramientas del DDL se utilizan mayormente en la fase de construcción y mantenimiento de las bases de datos, la manipulación u operación se hace con DML.

### Clase 23 DML

**DML** trata del contenido de la base de datos. Son las siglas de Data Manipulation Language y sus comandos son:

**- Insert:** Inserta o agrega nuevos registros a la tabla.
**- Update:** Actualiza o modifica los datos que ya existen.
**- Delete:** Esta sentencia es riesgosa porque puede borrar el contenido de una tabla.
**- Select:** Trae información de la base de datos.

#### Insert

Crearemos este comando en una BD nueva llamada platzi_test con la con la estructura del ejercicio anterior

![insert_command.png](src/insert_command.png)

En la seccion de query realizamos el comando

```sql
INSERT INTO people(last_name, first_name, address, city)
VALUES ('Hernandez', 'Laura', 'Calle 21', 'Monterrey');
```

Insertamos los valores con el símbolo de rayo o con ctrl + enter

![insert_command_1.png](src/insert_command_1.png)

![insert_command_2.png](src/insert_command_2.png)

#### Update

![update_command.png](src/update_command.png)

comandos

```sql
UPDATE people SET last_name = 'Chavez', city = 'Merida'
WHERE person_id = 1;
```

![update_command_1.png](src/update_command_1.png)

![update_command_2.png](src/update_command_2.png)

#### Delete

```sql
DELETE FROM people WHERE person_id = 1;
```

![delete__command_1.png](src/delete__command_1.png)

#### Select

![select_command.png](src/select_command.png)

```sql
SELECT first_name, last_name FROM people;
```

![select_command_1.png](src/select_command_1.png)

### Clase 24 Que tan standard es SQL

La utilidad más grande de SQL fue unificar la forma en la que pensamos y hacemos preguntas a un repositorio de datos. Ahora que nacen nuevas bases de datos igualmente siguen tomando elementos de SQL.

Practicamos lo anterior como repaso.

```sql
CREATE TABLE people(
person_id int,
last_name VARCHAR(255),
first_name VARCHAR(255),
address VARCHAR(255),
city VARCHAR(255)
);

INSERT INTO people (last_name, first_name, address, city)
VALUES (‘Hernandez’, ‘Laura’, ‘Calle 21’, ‘Monterrey’);
.

SELECT first_name, last_name FROM people;


DROP TABLE people;
```

Realizamos  lo  mismo en una instancia de postgre gcloud

Tal cual pegamos crear tabla

```sql
CREATE TABLE people(
person_id int,
last_name VARCHAR(255),
first_name VARCHAR(255),
address VARCHAR(255),
city VARCHAR(255)
);
```

revisamos las tablas con

```sql
\dt
```

Hacemos las operaciones anteriores

```sql

INSERT INTO people (last_name, first_name, address, city)
VALUES (‘Hernandez’, ‘Laura’, ‘Calle 21’, ‘Monterrey’);
.

SELECT first_name, last_name FROM people;


DROP TABLE people;
```

El DDL y DML en ambos  motores de bases de datos es estandar, cambian solo funciones internas.

### Clase 25 Creando Platziblog: tablas independientes

- Una buena práctica es comenzar creando las entidades que no tienen una llave foránea.
- Generalmente en los nombres de bases de datos se evita usar eñes o acentos para evitar problemas en los manejadores de las bases de datos.

![diagrama_fisico_paso_2](src/diagrama_fisico_paso_2.png)

Creamos el schema `platziblog` y seleccionamos como default y creamos las siguientes tablas

- categorías
  
![platziblog_tabla_etiquetas_1](src/platziblog_tabla_caracteristicas_1.png)

![platziblog_tabla_caracteristicas_2](src/platziblog_tabla_caracteristicas_2.png)

Creamos de igual forma la tabla Etiquetas

![platziblog_tabla_etiquetas_1](src/platziblog_tabla_etiquetas_1.png)

![platziblog_tabla_etiquetas_2](src/platziblog_tabla_etiquetas_2.png)

Tabla Usuarios

![platziblog_tabla_usuarios_1.png](src/platziblog_tabla_usuarios_1.png)

![platziblog_tabla_usuarios_2.png](src/platziblog_tabla_usuarios_2.png)

### Clase 26 Creando Platziblog: tablas transitivas

Creando Platziblog: tablas dependientes
El comando **“cascade”** sirve para que cada que se haga un update en la tabla principal, se refleje también en la tabla en la que estamos creando la relación.

![platziblog_tabla_post_1.png](src/platziblog_tabla_post_1.png)

![platziblog_tabla_post_2.png](src/platziblog_tabla_post_2.png)

Vamos a la pestaña Foreign Key y asignamos las relaciones.

Asignamos la llave foranea del usuario_id

![platziblog_tabla_post_fk_usuario_id.png](src/platziblog_tabla_post_fk_usuario_id.png)

![platziblog_tabla_post_fk_categorias_id.png](src/platziblog_tabla_post_fk_categorias_id.png)

![platziblog_tabla_post_fk_categorias_id_1.png](src/platziblog_tabla_post_fk_categorias_id_1.png)

### Clase 27 Creando Platziblog: tablas transitivas

- Las tablas transitivas sirven como puente para unir dos tablas. No tienen contenido semántico.

- **Reverse Engineer** nos reproduce el esquema del cual nos basamos para crear nuestras tablas. Es útil cuando llegas a un nuevo trabajo y quieres entender cuál fue la mentalidad que tuvieron al momento de crear las bases de datos.

Creamos la tabla comentarios.

![platziblog_tabla_comentarios.png](src/platziblog_tabla_comentarios.png)

![platziblog_tabla_comentarios_1.png](src/platziblog_tabla_comentarios_1.png)

Creamos las llaves foráneas para los comentarios de los usuarios

![platziblog_tabla_comentarios_usuarios_fk_1.png](src/platziblog_tabla_comentarios_usuarios_fk_1.png)

![platziblog_tabla_comentarios_usuarios_fk_2.png](src/platziblog_tabla_comentarios_usuarios_fk_2.png)

Creamos las llaves foráneas para los comentarios de los posts

![platziblog_tabla_comentarios_usuarios_fk_1.png](src/platziblog_tabla_comentarios_usuarios_fk_1.png)

![platziblog_tabla_comentarios_usuarios_fk_2.png](src/platziblog_tabla_comentarios_usuarios_fk_2.png)

Ahora solo nos queda crear la tabla intermedia para romper la relacion muchos a muchos.

![diagrama_fisico_paso_3_N_N.png](src/diagrama_fisico_paso_3_N_N.png)

Para ello creamos la tabla intermedia post_etiquetas

![platziblog_tabla_post_etiquetas.png](src/platziblog_tabla_post_etiquetas.png)

![platziblog_tabla_post_etiquetas_1.png](src/platziblog_tabla_post_etiquetas_1.png)

Ligamos las llaves foráneas para post_id

![platziblog_tabla_post_etiquetas_fk_1.png](src/platziblog_tabla_post_etiquetas_fk_1.png)

![platziblog_tabla_post_etiquetas_fk_2.png](src/platziblog_tabla_post_etiquetas_fk_2.png)

Ligamos las llaves foráneas para etiquetas_id

![platziblog_tabla_post_etiquetas_etiquetas_fk_1.png](src/platziblog_tabla_post_etiquetas_etiquetas_fk_1.png)

![platziblog_tabla_post_etiquetas_etiquetas_fk_2.png](src/platziblog_tabla_post_etiquetas_etiquetas_fk_2.png)

#### Reverse Engineer

Seleccionamos la opción Database para acceder a reverse engineer
![reverse_engineer_1](src/reverse_engineer_1.png)

![reverse_engineer_2](src/reverse_engineer_2.png)

![reverse_engineer_3](src/reverse_engineer_3.png)

![reverse_engineer_4](src/reverse_engineer_4.png)

![reverse_engineer_5](src/reverse_engineer_5.png)

![reverse_engineer_6](src/reverse_engineer_6.png)

![reverse_engineer_7](src/reverse_engineer_7.png)

### Clase 28 Por qué las consultas son tan importantes

Las consultas o queries a una base de datos son una parte fundamental ya que esto podría salvar un negocio o empresa.
Alrededor de las consultas a las bases de datos se han creado varias especialidades como ETL o transformación de datos, business intelligence e incluso machine learning.

### Clase 29 Estructura básica de un Query

Los queries son la forma en la que estructuramos las preguntas que se harán a la base de datos. Transforma preguntas en sintaxis.

El query tiene básicamente 2 partes: SELECT y FROM y puede aparecer una tercera como WHERE.

La estrellita o asterisco (*) quiere decir que vamos a seleccionar todo sin filtrar campos.

Antes de iniciar la clase corre este script

```sql
Script de la base datos platziblog

--creamos la base datos :platziblog

-- nos ubicamos en la base datos  platziblog
use platziblog;

-- CREACIONES DE TABLAS
-- Eliminacion de tablas, va en ese orden por los FK
 drop table comentarios;
 drop table posts_etiquetas;
 drop table posts;
 drop table etiquetas;
 drop table usuarios;
 drop table categorias;


-- CREACIONES DE TABLAS
-- Creación de la tabla usuarios
CREATE TABLE `usuarios` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `login` varchar(30) NOT NULL,
  `password` varchar(32) NOT NULL,
  `nickname` varchar(40) NOT NULL,
  `email` varchar(40) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY`email_UNIQUE` (`email`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- Creación de la tabla categorias
CREATE TABLE `categorias` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `nombre_categoria`varchar(30) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- Creación de la tabla etiquetas
CREATE TABLE`etiquetas` (
  `id`int(11) NOT NULL AUTO_INCREMENT,
  `nombre_etiqueta`varchar(30) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- Creación de la tabla posts
CREATE TABLE `posts` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `titulo` varchar(130) NOT NULL,
  `fecha_publicacion` timestamp NULL DEFAULT NULL,
  `contenido` text NOT NULL,
  `estatus` char(8) DEFAULT 'activo',
  `usuario_id` int(11) DEFAULT NULL,
  `categoria_id` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`),
  KEY `posts_usuarios_idx` (`usuario_id`),
  KEY `posts_categorias_idx` (`categoria_id`),
  CONSTRAINT `posts_categorias` FOREIGN KEY (`categoria_id`) REFERENCES `categorias` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION,
  CONSTRAINT `posts_usuarios` FOREIGN KEY (`usuario_id`) REFERENCES `usuarios` (`id`) ON DELETE NO ACTION ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;

-- Creación de la tabla comentarios
CREATE TABLE `comentarios` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `cuerpo_comentario` text NOT NULL,
  `usuario_id` int(11) NOT NULL,
  `post_id` int(11) NOT NULL,
  PRIMARY KEY (`id`),
  KEY `comentarios_usuario_idx` (`usuario_id`),
  KEY `comentarios_post_idx` (`post_id`),
  CONSTRAINT `comentarios_post` FOREIGN KEY (`post_id`) REFERENCES `posts` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION,
  CONSTRAINT `comentarios_usuario` FOREIGN KEY (`usuario_id`) REFERENCES `usuarios` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION
) ENGINE=InnoDB DEFAULT CHARSET=utf8;


-- Creación de la tabla posts_etiquetas
CREATE TABLE `posts_etiquetas` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `post_id` int(11) NOT NULL,
  `etiqueta_id` int(11) NOT NULL,
  PRIMARY KEY (`id`),
  KEY `postsetiquetas_post_idx` (`post_id`),
  KEY `postsetiquetas_etiquetas_idx` (`etiqueta_id`),
  CONSTRAINT `postsetiquetas_etiquetas` FOREIGN KEY (`etiqueta_id`) REFERENCES `etiquetas` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION,
  CONSTRAINT `postsetiquetas_post` FOREIGN KEY (`post_id`) REFERENCES `posts` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- INSERCIÓN DE VALORES A LAS TABLAS
-- Insert  en la tabla usuarios
INSERT INTO usuarios (login,password,nickname,email) VALUES ('israel','1234','israel','israel@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('monica','1234','Moni','monica@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('laura','1234','Lau','laura@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('edgar','5678','Ed','edgar@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('perezoso','5678','Oso Pérez','perezoso@platziblog.com');

-- Insert  en la tabla categorias
INSERT INTO categorias (nombre_categoria) VALUES ('Ciencia');
INSERT INTO categorias (nombre_categoria) VALUES ('Tecnología');
INSERT INTO categorias (nombre_categoria) VALUES ('Deportes');
INSERT INTO categorias (nombre_categoria) VALUES ('Espectáculos');
INSERT INTO categorias (nombre_categoria) VALUES ('Economía');

-- Insert  en la tabla etiquetas
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Robótica');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Computación');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Teléfonos Móviles');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Automovilismo');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Campeonatos');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Equipos');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Bolsa de valores');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Inversiones');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Brokers');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Celebridades');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Eventos');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Moda');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Avances');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Nobel');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Matemáticas');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Química');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Física');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Largo plazo');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Bienes Raíces');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Estilo');

-- Insert  en la tabla posts
INSERT INTO posts (id, titulo, fecha_publicacion, contenido, estatus, usuario_id, categoria_id)
   VALUES (1,'Se presenta el nuevo teléfono móvil en evento', '2030-04-05 00:00:00', 'Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.',  'activo', 1, 1);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Tenemos un nuevo auto inteligepostsnte','2025-05-04 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',2,2);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Ganador del premio Nobel por trabajo en genética','2023-12-22 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',3,3);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Los mejores vestidos en la alfombra roja','2021-12-22 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',4,4);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Los paparatzi captan escándalo en cámara','2025-01-09 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','inactivo',4,5);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Se mejora la conducción autónoma de vehículos','2022-05-23 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',1,5);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Se descubre nueva partícula del modelo estandar','2023-01-10 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',2,4);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Químicos descubren nanomaterial','2026-06-04 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',2,3);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('La bolsa cae estrepitosamente','2024-04-03 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',2,2);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Bienes raices más baratos que nunca','2025-04-11 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','inactivo',2,1);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Se fortalece el peso frente al dolar','2021-10-09 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',1,1);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Tenemos ganador de la formula e','2022-11-11 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',1,2);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Ganan partido frente a visitantes','2023-12-10 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',2,3);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Equipo veterano da un gran espectaculo','2023-12-01 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','inactivo',2,4);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Escándalo con el boxeador del momento','2025-03-05 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',4,5);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Fuccia OS sacude al mundo','2028-10-10 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.','activo',1,5);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('U.S. Robotics presenta hallazgo','2029-01-10 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.\n','activo',1,4);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Cierra campeonato mundial de football de manera impresionante','2023-04-10 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.\n','activo',2,3);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Escándalo en el mundo de la moda','2022-04-11 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.\n','activo',4,2);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Tenemos campeona del mundial de volleiball','2024-09-09 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.\n','inactivo',2,1);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('Se descubre la unión entre astrofísica y fisica cuántica','2022-05-03 00:00:00','Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.\n','inactivo',3,5);
INSERT INTO posts (titulo,fecha_publicacion,contenido,estatus,usuario_id,categoria_id)
  VALUES ('El post que se quedó huérfano','2029-08-08 00:00:00','\'Phasellus laoreet eros nec vestibulum varius. Nunc id efficitur lacus, non imperdiet quam. Aliquam porta, tellus at porta semper, felis velit congue mauris, eu pharetra felis sem vitae tortor. Curabitur bibendum vehicula dolor, nec accumsan tortor ultrices ac. Vivamus nec tristique orci. Nullam fringilla eros magna, vitae imperdiet nisl mattis et. Ut quis malesuada felis. Proin at dictum eros, eget sodales libero. Sed egestas tristique nisi et tempor. Ut cursus sapien eu pellentesque posuere. Etiam eleifend varius cursus.\n\nNullam viverra quam porta orci efficitur imperdiet. Quisque magna erat, dignissim nec velit sit amet, hendrerit mollis mauris. Mauris sapien magna, consectetur et vulputate a, iaculis eget nisi. Nunc est diam, aliquam quis turpis ac, porta mattis neque. Quisque consequat dolor sit amet velit commodo sagittis. Donec commodo pulvinar odio, ut gravida velit pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.\n\nMorbi vulputate ante quis elit pretium, ut blandit felis aliquet. Aenean a massa a leo tristique malesuada. Curabitur posuere, elit sed consectetur blandit, massa mauris tristique ante, in faucibus elit justo quis nisi. Ut viverra est et arcu egestas fringilla. Mauris condimentum, lorem id viverra placerat, libero lacus ultricies est, id volutpat metus sapien non justo. Nulla facilisis, sapien ut vehicula tristique, mauris lectus porta massa, sit amet malesuada dolor justo id lectus. Suspendisse sit amet tempor ligula. Nam sit amet nisl non magna lacinia finibus eget nec augue. Aliquam ornare cursus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit.\n\nDonec ornare sem eget massa pharetra rhoncus. Donec tempor sapien at posuere porttitor. Morbi sodales efficitur felis eu scelerisque. Quisque ultrices nunc ut dignissim vehicula. Donec id imperdiet orci, sed porttitor turpis. Etiam volutpat elit sed justo lobortis, tincidunt imperdiet velit pretium. Ut convallis elit sapien, ac egestas ipsum finibus a. Morbi sed odio et dui tincidunt rhoncus tempor id turpis.\n\nProin fringilla consequat imperdiet. Ut accumsan velit ac augue sollicitudin porta. Phasellus finibus porttitor felis, a feugiat purus tempus vel. Etiam vitae vehicula ex. Praesent ut tellus tellus. Fusce felis nunc, congue ac leo in, elementum vulputate nisi. Duis diam nulla, consequat ac mauris quis, viverra gravida urna.\n\'','activo',2,3);

-- Insert  en la tabla posts_etiquetas
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (1,43,3);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (2,43,11);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (3,44,2);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (4,44,4);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (5,45,14);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (6,45,13);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (7,46,10);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (8,46,11);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (9,46,12);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (10,46,20);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (11,47,10);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (12,48,1);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (13,48,2);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (14,48,4);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (15,48,13);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (16,49,13);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (17,49,14);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (18,49,17);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (19,50,13);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (20,50,14);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (21,50,16);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (22,51,7);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (23,51,8);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (24,51,9);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (25,51,18);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (26,52,8);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (27,52,18);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (28,53,7);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (29,53,8);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (30,54,4);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (31,54,5);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (32,55,5);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (33,55,6);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (34,56,5);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (35,56,6);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (36,56,10);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (37,58,2);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (38,58,3);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (39,58,13);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (40,59,1);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (41,59,13);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (42,57,10);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (43,60,5);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (44,60,6);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (45,61,10);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (46,61,12);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (47,61,20);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (48,62,5);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (49,62,10);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (50,63,13);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (51,63,14);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (52,63,17);
INSERT INTO `platziblog.posts_etiquetas` (`id`,`post_id`,`etiqueta_id`) VALUES (53,52,19);

```

#### Primer Consulta

```sql
SELECT*
FROM posts
WHERE fecha_publicacion < '2024'
```

### Clase 30 SELECT

**SELECT** se encarga de proyectar o mostrar datos.

- El nombre de las columnas o campos que estamos consultando puede ser cambiado utilizando AS después del nombre del campo y poniendo el nuevo que queremos tener:

```sql
SELECT titulo AS encabezado
FROM posts;
```

Existe una función de SELECT para poder contar la cantidad de registros. Esa información (un número) será el resultado del query:

```sql
SELECT COUNT(*)
FROM posts;
```

Queries de la clase

```sql

SELECT titulo, fecha_publicacion, estatus
FROM posts
```

Usando AS para asignar un alias

```sql
SELECT titulo, fecha_publicacion AS publicado_en, estatus  AS estado
FROM posts;
```

Contar los registros

```sql
SELECT COUNT(*) AS numero_post
FROM posts;
```

### Clase 31 FROM

**FROM** indica de dónde se deben traer los datos y puede ayudar a hacer sentencias y filtros complejos cuando se quieren unir tablas. La sentencia compañera que nos ayuda con este proceso es **JOIN**.

Los diagramas de Venn son círculos que se tocan en algún punto para ver dónde está la intersección de conjuntos. Ayudan mucho para poder formular la sentencia **JOIN** de la manera adecuada dependiendo del query que se quiere hacer.

![teoria_conjuntos](src/Teoria_conjuntos.jpg)

![teoria_conjuntos_sentencias](src/teoria_conjuntos_sentencias.jpg)

### Clase 32 Utilizando la sentencia FROM

Comandos de la clase

Left Join  trae todos los usuarios (tabla A), tengan o no tengan algún Post (tabla b)

```sql
SELECT *
FROM usuarios
 LEFT JOIN posts ON usuarios.id = posts.usuario_id;
```

Left Join sin intersección

```sql
SELECT *
FROM usuarios
  LEFT JOIN posts ON usuarios.id = posts.usuario_id
WHERE posts.usuario_id IS NULL;
```

Left Join  trae todos los Post (tabla B), tengan o no tengan algún Usuario (tabla A)

```sql
SELECT *
FROM usuarios
 RIGHT JOIN posts ON usuarios.id = posts.usuario_id;
```

Right Join sin intersección

```sql
SELECT *
FROM usuarios
 RIGHT JOIN posts ON usuarios.id = posts.usuario_id
WHERE posts.usuario_id IS NULL;
```

Inner Join

```sql
SELECT *
FROM usuarios
 INNER JOIN posts ON usuarios.id = posts.usuario_id;
```

Full Join

```sql
SELECT *
FROM usuarios
 LEFT JOIN posts ON usuarios.id = posts.usuario_id
UNION
SELECT *
FROM usuarios
 RIGHT JOIN posts ON usuarios.id = posts.usuario_id;
```

Diferencia Asimétrica

```sql
SELECT *
FROM usuarios
 LEFT JOIN posts ON usuarios.id = posts.usuario_id
WHERE posts.usuario_id IS NULL
UNION
SELECT *
FROM usuarios
 RIGHT JOIN posts ON usuarios.id = posts.usuario_id
WHERE posts.usuario_id IS NULL;
```

### Clase 33 WHERE

**WHERE** es la sentencia que nos ayuda a filtrar tuplas o registros dependiendo de las características que elegimos.

- La propiedad **LIKE** nos ayuda a traer registros de los cuales conocemos sólo una parte de la información.
- La propiedad **BETWEEN** nos sirve para arrojar registros que estén en el medio de dos. Por ejemplo los registros con id entre 20 y 30

Queries de la clase

Filtrando de forma numérica

```sql
SELECT *
FROM posts
WHERE id <= 10 ;
```

Filtrando con strings

```sql
SELECT *
FROM posts
WHERE estatus = 'activo' ;
```

```sql
SELECT *
FROM posts
WHERE estatus != 'activo' ;
```

Utilizando LIKE % es un wildcard

```sql
-- todos los post con la palabra
SELECT *
FROM posts
WHERE titulo LIKE '%escandalo%' ;
```

```sql
-- todos los post que inicien con la palabra
SELECT *
FROM posts
WHERE titulo LIKE 'escandalo%' ;
```

```sql
-- todos los post que terminen con la palabra
SELECT *
FROM posts
WHERE titulo LIKE '%roja' ;
```

Usando WHERE con fechas

```sql
SELECT *
FROM posts
WHERE fecha_publicacion > "2025-01-01";
```

```sql
SELECT *
FROM posts
WHERE fecha_publicacion < "2025-01-01";
```

Usando BETWEEN para  definir un rangos

```sql
SELECT *
FROM posts
WHERE fecha_publicacion BETWEEN "2025-01-01" AND "2025-12-31";
```

```sql
SELECT *
FROM posts
WHERE id BETWEEN 5 AND 10;
```

Otros filtros con fechas

```sql
SELECT *
FROM posts
WHERE YEAR(fecha_publicacion) BETWEEN "2023" AND "2024";
```

```sql
SELECT *
FROM posts
WHERE MONTH(fecha_publicacion) = "04";
```

### Clase 34 Utilizando la sentencia WHERE nulo y no nulo

El valor nulo en una tabla generalmente es su valor por defecto cuando nadie le asignó algo diferente. La sintaxis para hacer búsquedas de datos nulos es **IS NULL**. La sintaxis para buscar datos que no son nulos es **IS NOT NULL**

Para posts sin usuario

```sql
SELECT *
FROM posts
WHERE usuario_id IS NULL;
;
```

Para posts con usuario

```sql
SELECT *
FROM posts
WHERE usuario_id IS NOT NULL;
;
```

Para posts con usuario y activo, el uso de AND agrega condiciones de tipo filtro como usar excel

```sql
SELECT *
FROM posts
WHERE usuario_id IS NOT NULL
 AND estatus ='activo'
    AND id < 20
    AND categoria_id = 2
 AND year(fecha_publicacion) = '2025'
;

```

### Clase 35 GROUP BY

**GROUP BY** tiene que ver con agrupación. Indica a la base de datos qué criterios debe tener en cuenta para agrupar.

Gruop by te permite agrupar estilo pivot tables, e informes.

```sql
SELECT estatus, COUNT(*) AS post_quantity
FROM posts
GROUP BY estatus
;
```

Ejemplo 2 Agrupando por Año

```sql
SELECT YEAR(fecha_publicacion) AS post_year, COUNT(*) AS post_quantity
FROM posts
GROUP BY post_year
;
```

Ejemplo 3 Agrupando por Mes

```sql
SELECT MONTHNAME(fecha_publicacion) AS post_month, COUNT(*) AS post_quantity
FROM posts
GROUP BY post_month
;
```

Ejemplo 4 Agrupando por Mes y estatus

```sql
SELECT estatus, MONTHNAME(fecha_publicacion) AS post_month, COUNT(*) AS post_quantity
FROM posts
GROUP BY estatus, post_month 
;
```

### Clase 36 ORDER BY y HAVING

La sentencia **ORDER BY** tiene que ver con el ordenamiento de los datos dependiendo de los criterios que quieras usar.

- **ASC** sirve para ordenar de forma ascendente.
- **DESC** sirve para ordenar de forma descendente.
- **LIMIT** se usa para limitar la cantidad de resultados que arroja el query.
- **HAVING** tiene una similitud muy grande con **WHERE**, sin embargo el uso de ellos depende del orden. Cuando se quiere seleccionar tuplas agrupadas únicamente se puede hacer con **HAVING**.

Ejemplo Order by ascendente default

```sql
SELECT *
FROM posts
ORDER BY fecha_publicacion
;
```

Ejemplo Order by ascendente explicito

```sql
SELECT *
FROM posts
ORDER BY fecha_publicacion ASC
;
```

Ejemplo Order by descendente

```sql
SELECT *
FROM posts
ORDER BY fecha_publicacion DESC
;
```

Ordenando con strings se toma el orden alfabetico.

```sql
SELECT *
FROM posts
ORDER BY titulo ASC
;
```

Ejemplo Order by ascendente explicito y limite de 5 registros

```sql
SELECT *
FROM posts
ORDER BY fecha_publicacion ASC
LIMIT 5
;
```

**HAVING** es similar a **WHERE** aunque no muy utilizada, pero es necesaria cuando quieres hacer un filtro con datos agrupados por un ORDER BY, **HAVING** siempre va despues del **GROUP BY**

```sql
SELECT MONTHNAME(fecha_publicacion) AS post_month, estatus, COUNT(*) AS post_quantity
FROM posts
GROUP BY estatus, post_month
HAVING post_quantity > 1
ORDER BY post_month
;
```

### Clase 37 El interminable agujero de conejo (Nested queries)

Los **Nested queries** significan que dentro de un query podemos hacer otro query. Esto sirve para hacer join de tablas, estando una en memoria. También teniendo un query como condicional del otro.

Este proceso puede ser tan profundo como quieras, teniendo infinitos queries anidados.
Se le conoce como un *producto cartesiano* ya que se multiplican todos los registros de una tabla con todos los del nuevo query. Esto provoca que el query sea difícil de procesar por lo pesado que puede resultar, y se considera como no escalable.

Ejemplo 1

```sql
SELECT new_table_projection.date, COUNT(*) AS posts_count
FROM (
SELECT DATE(MIN(fecha_publicacion)) AS date, year(fecha_publicacion) AS post_year
FROM posts
GROUP BY post_year
) AS new_table_projection
GROUP BY new_table_projection.date
ORDER BY new_table_projection.date
```

Ejemplo 2

```sql
SELECT *
FROM posts
WHERE fecha_publicacion = (
SELECT MAX(fecha_publicacion)
FROM posts
);
```

### Clase 38 Como convertir una pregunta en un query SQL

#### De pregunta a Query

**SELECT:** Lo que quieres mostrar
**FROM:** De dónde voy a tomar los datos (tablas unicas o con joins)
**WHERE:** Los filtros de los datos que quieres mostrar
**GROUP BY:** Los rubros por los que me interesa agrupar la información
**ORDER BY:** El orden en que quiero presentar mi información
**HAVING:** Los filtros que quiero que mis datos agrupados tengan



### Clase 39 Preguntandole a la base de datos

**GROUP_CONCAT** toma el resultado del query y lo pone como campo separado por comas.

Criterios.

**DISTINCT:** Evita duplicidad en los valores.
**ORDER BY:** Sirve para decidir el orden de concatenación del campo.
**:** Es el separador a utilizar para separar los valores (por defecto, el separador es una coma “,”).

Preguna 1 Cuantas etiquetas estan ligadas a los blogposts

```sql
SELECT posts.titulo, COUNT(*) num_etiquetas
FROM posts
 INNER JOIN posts_etiquetas ON posts.id = posts_etiquetas.post_id
 INNER JOIN etiquetas ON etiquetas.id = posts_etiquetas.etiqueta_id
GROUP BY posts.id
ORDER BY num_etiquetas DESC
;
```

Usando GROUP_CONCAT para tener campos separados por comas

```sql
SELECT posts.titulo, GROUP_CONCAT(nombre_etiqueta)
FROM posts
 INNER JOIN posts_etiquetas ON posts.id = posts_etiquetas.post_id
 INNER JOIN etiquetas ON etiquetas.id = posts_etiquetas.etiqueta_id
GROUP BY posts.id
;
```

![GROUP_CONCAT](src/GROUP_CONCAT.png)

Saber que posts no tienen etiquetas

```sql
SELECT *
FROM etiquetas
 LEFT JOIN posts_etiquetas ON etiquetas.id = posts_etiquetas.etiqueta_id
WHERE posts_etiquetas.etiqueta_id IS NULL
;
```

### Clase 40 Consultando PlatziBlog

Puedes usar una abreviación para evitar escribir lo mismo cada vez.
Ejemplo:

FROM categorias AS c

Pregunta: Que categoria tiene mas posts escritos

```sql
SELECT c.nombre_categoria, COUNT(*) AS cant_posts
FROM categorias AS c
 INNER JOIN posts AS p ON c.id = p.categoria_id
GROUP BY c.id
ORDER BY cant_posts DESC
LIMIT 1
;
```

Pregunta: Que persona tiene mas posts escritos

```sql
SELECT u.nickname, COUNT(*) AS cant_posts
FROM usuarios AS u
 INNER JOIN posts AS p ON u.id = p.usuario_id
GROUP BY u.id
ORDER BY cant_posts DESC
;
```

```sql
SELECT u.nickname, COUNT(*) AS cant_posts, GROUP_CONCAT(nombre_categoria)
FROM usuarios AS u
 INNER JOIN posts AS p ON u.id = p.usuario_id
 INNER JOIN categorias AS c ON c.id = p.categoria_id
GROUP BY u.id
ORDER BY cant_posts DESC
;
```

Que usuarios no han escrito nada

```sql
SELECT *
FROM usuarios
  LEFT JOIN posts ON usuarios.id = posts.usuario_id 
WHERE posts.usuario_id IS NULL
;
```

## Modulo 4 Introduccion a la bases de datos NO relacionales

### Clase 41 Que son y cuales son los tipos de bases de datos no relacionales

Respecto a las bases de datos no relacionales, no existe un solo tipo aunque se engloben en una sola categoría.

#### Tipos de bases de datos no relacionales:

- **Clave - valor:** Son ideales para almacenar y extraer datos con una clave única. Manejan los diccionarios de manera excepcional. Ejemplos: **DynamoDB, Cassandra**.
- **Basadas en documentos:** Son una implementación de clave valor que varía en la forma semiestructurada en que se trata la información. Ideal para almacenar datos JSON y XML. Ejemplos: **MongoDB, Firestore**.
- **Basadas en grafos:** Basadas en teoría de grafos, sirven para entidades que se encuentran interconectadas por múltiples relaciones. Ideales para almacenar relaciones complejas. Ejemplos: **neo4j, TITAN**.
- **En memoria:** Pueden ser de estructura variada, pero su ventaja radica en la velocidad, ya que al vivir en memoria la extracción de datos es casi inmediata. Ejemplos: **Memcached, Redis**.
- **Optimizadas para búsquedas:** Pueden ser de diversas estructuras, su ventaja radica en que se pueden hacer queries y búsquedas complejas de manera sencilla. Ejemplos: **BigQuery, Elasticsearch**.

Cada base de datos de este tipo soluciona un problema en particular, pero es mala para todo lo demas dada la gran cantidad de datos.

### Clase 42 Servicios administrados y jerarquía de datos

**Firebase** es un servicio de Google donde puedes tercerizar muchos elementos en la nube.
**Jerarquía de datos**:

**1. Base de Datos:** Contiene toda la información que se quiere guardar.
**2. Colección:** Es igual a las tablas en las bases de datos relacionales. Son objetos que agrupan (Documentos) la información que se desea guardar.
**3. Documento:** Es la información que se quiere guardar. Se guarda en un formato muy parecido al formato JSON (es un lenguaje que se utiliza para comunicarse con diferentes lenguajes o aplicaciones). Los documentos dentro de ellos contienen datos.

![jerarquia_firestore](src/jerarquia_firestore.png)

## Modulo 5 Manejo de modelos de datos en bases de datos no relacionales

### Clase 43 Top level collection con Firebase

El modelo de bases de datos no relacionales es un poco más cercano al mundo real en su comportamiento.

- Las top level collections son las colecciones que se tienen de inmediato o entrada en el proyecto.
- **Firebase** es un servicio que tiene múltiples opciones y está pensado principalmente para aplicaciones móviles y web.

Para esta clase creamos una bd en firebase <https://console.firebase.google.com/u/0/?pli=1>

Seguimos  los pasos sencillos de la pagina para crear nuestra base de datos "platziblog"

Creamos proyecto

![firebase_intro_1](src/firebase_intro_1.png)

![firebase_intro_2](src/firebase_intro_2.png)

![firebase_intro_3](src/firebase_intro_3.png)

Panel Inicial

![firebase_intro_4](src/firebase_intro_4.png)

Para crear una Top level collection (las que estan a nivel de la ruta principal) damos en simbolo plus, y creamos /people

![firebase_intro_5](src/firebase_intro_5.png)

![firebase_intro_6](src/firebase_intro_6.png)

![firebase_intro_7](src/firebase_intro_7.png)

### Clase 44 Creando y borrando documentos en Firestore

Jugamos con la interface observamos los tipos de datos:

- **string:** (absorve text,  varchar, etc)
- **number:** (int,float)
- **Map:** permite hacer un arreglo dentro  de otro arreglo (inception)
- **Timestamp:** para datos de tiempo
- **Geopoint** latitud y longitud.
- **Reference:**, hace referencia a otro documento o coleccion

Ejemplos

![firebase_tipos_datos_1](src/firebase_tipos_datos_1.png)

![firebase_tipos_datos_2](src/firebase_tipos_datos_2.png)

![firebase_tipos_datos_3](src/firebase_tipos_datos_3.png)

![firebase_tipos_datos_4](src/firebase_tipos_datos_4.png)

### Clase 45 Colecciones vs subcolecciones

La particularidad de las top level collections es que existen en el primer nivel de manera intrínseca. Las subcolecciones ya no vivirán al inicio de la base de datos.

Si tienes una entidad separada que vas a referenciar desde muchos lugares es recomendado usar un top level collection. Por el otro lado si se necesita hacer algo intrínseco al documento es aconsejable usar subcolecciones.

Creamos la coleccion posts

![colecciones_vs_subcolecciones_1](src/colecciones_vs_subcolecciones_1.png)

![colecciones_vs_subcolecciones_2](src/colecciones_vs_subcolecciones_2.png)

![colecciones_vs_subcolecciones_3](src/colecciones_vs_subcolecciones_3.png)

![colecciones_vs_subcolecciones_4](src/colecciones_vs_subcolecciones_4.png)

![colecciones_vs_subcolecciones_5](src/colecciones_vs_subcolecciones_5.png)

![colecciones_vs_subcolecciones_6](src/colecciones_vs_subcolecciones_6.png)

### Clase 46 Recreando Platziblog

Firestore, es una base de datos basada en documentos, pensada en lo siguiente:

Mantener el estado de tu aplicación.
En como se verán reflejados los datos en el frontend para el usuario.
Podemos hacer consultas sencillas en base a las top level collecttion. Ahora si queremos hacer consultas mas complejas podríamos usar big query, que es un data wharehouse.

### Clase 47 Construyendo Platziblog en Firestore

Construimos categorias "espectaculos","deportes" y "ciencia" como top level collection

![Platziblog_firebase_1](src/Platziblog_firebase_1.png)

![Platziblog_firebase_2](src/Platziblog_firebase_2.png)

Creamosen top level la coleccion usuarios

![Platziblog_firebase_3](src/Platziblog_firebase_3.png)

Creamos la top level posts con dos articulos

![Platziblog_firebase_4](src/Platziblog_firebase_4.png)

![Platziblog_firebase_5](src/Platziblog_firebase_5.png)

Ahora hacemos la relacion del top level collection del usuario /usuarios/qK7F62sQY8bKI8o9w5RY agregando un campo en un documento posts usando el campo reference agregando el usuario

![Platziblog_firebase_6](src/Platziblog_firebase_6.png)

![Platziblog_firebase_7](src/Platziblog_firebase_7.png)

Agregamos las referencias para las categorias

![Platziblog_firebase_8](src/Platziblog_firebase_8.png)

![Platziblog_firebase_9](src/Platziblog_firebase_9.png)

Finalmente agregamos las subcolecciones etiquetas a los posts en agregar coleccion

![Platziblog_firebase_10](src/Platziblog_firebase_10.png)

### Clase 48 Proyecto final: transformando tu proyecto en una db no relacional

Dentro de las bases de datos relacionales tenemos diferentes niveles de datos. En primer lugar tenemos las Bases de Datos o Esquemas como repositorios donde vivirán los datos que nos interesa guardar. Dentro del esquema existen las Tablas que provienen del concepto de entidades; y a su vez dentro de las tablas tenemos las tuplas o renglones.

Cuando trabajamos con bases de datos basadas en documentos como Firestore, aún existe la figura de la base de datos, sin embargo cambiaremos las tablas en favor de las colecciones y las tuplas en lugar de los documentos.

Recuerda:

Tabla -> Colección

Tupla -> Documento

Dentro de las Colecciones existen 2 grandes tipos. Las Top level collection o colecciones de nivel superior y las subcollections o subcolecciones. Estas últimas viven únicamente dentro de un documento padre.

¿Cómo saber cuál escoger?

Para determinar si tu colección debe ser top level o subcolección no hay una regla escrita en piedra y más bien tiene que ver con el caso de uso en particular y con la experiencia que hayas ganado como desarrollador.

Lo cierto es que no hay una sola forma de estructurar nuestra DB basada en documentos, y por tanto no existe una respuesta correcta, sin embargo a continuación te ofrezco un par de reglas guía que puedes utilizar para transformar tu proyecto que ya trabajaste en bases de datos relacionales en un proyecto no relacional.

#### Regla 1. Piensa en la vista de tu aplicación

La primera pista que te puedo dar es que pienses en un inicio en la manera en que los datos serán extraídos. En el caso de una aplicación, la mejor forma de pensarlo es en términos de las vistas que vas a mostrar a un momento determinado en la aplicación.

Es decir, al armar la estructura en la base de datos que sea un espejo o que al menos contenga todos los datos necesarios para llenar las necesidades que tiene nuestra parte visual en la aplicación.

En el caso de Platziblog por ejemplo si tienes una vista de un blog post individual, generalmente conviene mostrar además de los datos inherentes al post como el contenido, datos adicionales como las etiquetas que tiene o por ejemplo el autor (o autores si es colaborativo), en este caso tal vez convenga guardar estas dos “entidades” (autores y etiquetas) como subcolecciones de cada documento blog post.

Regla 2. La colección tiene vida propia

Esta regla se refiere a que la excepción a la regla 1 es cuando tenemos un caso en que la “entidad” que tiene necesidad de vivir y modificarse constantemente de manera independiente a las otras colecciones. Por ejemplo en Platziblog podemos en el ejemplo anterior hacer una excepción a autores porque nos conviene tenerlas como top level collection en el sentido que se añadan, borren, cambien o listen los usuarios sin depender del blog post.

Experimenta aplicando estas dos reglas a un proyecto que ya conozcas en una base de datos relacional y trata de convertirla en un proyecto de Firestore y comentanos los retos a los que te enfrentaste.

## Modulo 6 Bases de datos en la vida real

### Clase 49 Bases de datos en la vida real

Para datos historicos, queries complejos usar bigquery optimizado para datawherehouse

Para datos del estado de nuestra aplicacion usa colecciones con mongo o firebase.

Puedes usar dos bases de datos en un mismo proyecto, guardar datos de mongo, convertirlos pasarlos a bigquery y hacer analisis sobre ellos.

### Clase 50 Big Data

**Big Data** es un concepto que nace de la necesidad de manejar grandes cantidades de datos. La tendencia comenzó con compañías como **YouTube** al tener la necesidad de guardar y consultar mucha información de manera rápida.

Es un gran movimiento que consiste en el uso de diferentes tipos de bases de datos.

Un ejemplo  es cassandra pero tiene ciertos tipos de desventaja, su ventaja manejar datos masivos a gran velocidad

### Clase 51 Data warehouse

**Data Warehouse** trata de guardar cantidades masivas de datos para la posteridad. Allí se guarda todo lo que no está viviendo en la aplicación pero es necesario tenerlo.
Debe servir para guardar datos por un largo periodo de tiempo y estos datos se deben poder usar para poder encontrar cuestiones interesantes para el negocio.

Google usa **BigTable**, usa una sola tabla, pero no sirve tanto para hacer consultas

**Data Warehouse** es un archivo historico, archivo muerto, en  otra base de datos. Sirve para dos actividades principales:

- Guarda una gran cantidad de datos de forma "eterna".
- Poder extraer los datos para hacer analitica.

BigQuery es muy utilizado

### Clase 52 Data mining

El **Data Mining** se dedica a minar datos, a extraerlos de donde sea que estén (archivos muertos, base de datos actual, etc…) y hacer sentido de ellos para darles un uso.

### Clase 53 ETL

**ETL** son las siglas de Extract, Transform, Load (extraer, transformar y cargar). Se trata de tomar datos de archivos muertos y convertirlos en algo que sea de utilidad para el negocio.
También ayuda a tomar los datos vivos de la aplicación, transformarlos y guardarlos en un data warehouse periódicamente.

### Clase 54 Business intelligence

**Business Intelligence** es una parte muy importante de las carreras de datos ya que es el punto final del manejo de estos. Su razón de ser es tener la información lista, clara y que tenga todos los elementos para tomar decisiones en una empresa.
Es necesario tener una buena sensibilidad por entender el negocio, sus necesidades y la información que puede llevar a tomar decisiones en el momento adecuado al momento de realizar business intelligence.

### Clase 55 Machine Learning

**Machine Learning** tiene significados que varían. Es una serie de técnicas que involucran la inteligencia artificial y la detección de patrones.
Machine learning para datos tiene un gran campo de acción y es un paso más allá del business intelligence.
Nos ayuda a hacer modelos que encuentran patrones fortuitos encontrando correlaciones inesperadas.

**Tiene dos casos de uso particulares:**

- Clasificación
- Predicción

### Clase 56 Data Science

**Data Science** es aplicar todas las técnicas de procesamiento de datos. En su manera más pura tiene que ver con gente con un background de estadísticas y ciencias duras.

### Clase 57 Por que aprender bases de datos hoy

¡Has concluido el curso! Ahora tienes potentes herramientas y posibilidades para ingresar en este apasionante campo.

Llevaste diagramas a bases de datos, exploraste un poco el mundo de las bases de datos no relacionales, hicimos un proyecto en firestore y transformamos Platzi blog de una base de datos relacional en una base de datos de documentos.

Dentro de las posibilidades que tienes hoy en día puedes hacer: Machine learning, ETL, Data Warehouse, Data mining, entre otros.

Recuerda practicar mucho con el proyecto. Te invito a que tomes el examen y verifiques tus conocimientos. ¡Exitos!

## Bonus

### Clase 58 Bases de datos relacionales vs no relacionales

Las bases de datos relacionales han estado entre nosotros durante un largo tiempo y han sido usadas por grandes como Google, Amazon, entre otros. Aún son usadas por bancos, aseguradoras, etc.

Las bases de datos no relacionales surgen cuando las grandes empresas sintieron necesidad de guardar y extraer grandes cantidades de datos en muy cortos periodos de tiempo, como YouTube.
