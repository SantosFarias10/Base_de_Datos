# Base de Datos

## Introduccion

### ¿Que es una Base de Datos?

Una **Base de Datos** (*BD*) es un conjunto de datos organizazdos, generalmente se trata de datos estructurados e interrelacionados. Se gestionan mediante **Sistemas de Gestion de Base de Datos** (*SGBD*).

### Aplicaciones de Base de Datos

* ¿Que permiten hacer?

    - **Navegar** y **Consultar** los datos.
    - **Modificar** los datos.
    - **Controlar el acceso** y garantizar la seguridad de los datos.

* Aplicaciones Web de Base de Datos:

    - El usuario **Accede** a la aplicacion desde un navegador web (*Browser*) que contiene la **UI** y envia solicitudes.
    - El servidor web **Procesa Solicitudes** (Pasando consultas al Sistema de Gestion de Base de Datos) y **Genera Respuestas** (a partir de los resultados enviados por el Sistema de Gestion de Bases de Datos).
    - El servidor web **Interactua con el Sistema de Gestion de Base de Datos** para **Almacenar**, **Recuperar**, o **Modificar** datos segun las acciones del usuario.

### Esquemas e Instancias

Los conceptos de **Esquema** es similar al de *Tipo* y el de **Instancia** es similar al de *Variable* en los lenguajes de programacion.

* **Esquema**: Describe la **Estructura** de la Base de Datos. Describe **Entidades**, **Relaciones** entre ellas y **Atributos** de las entidades.

    - Por **ejemplo**: La Base de Datos de un *Banco* consiste de **Entidades** (Clientes, Cuentas) donde:
        
        * Los *Clientes* tienen **Atributos** (*Nombre* y *DNI*).
        * Las *Cuentas* tienen **Atributos** (*Numero*, *Saldo*).

* **Instancia**: Es el **Contenido Actual** de la Base de Datos en un momento dado. Corresponde a los **Valores Concretos Almacenados**.

    - Por **ejemplo**: En la Base de Datos de un *Banco*:

        * Clientes: Juan Perez con DNI: 333 y Diego Gonzalez con DNI: 444.
        * Cuentas: Tiene las cuentas (numero: 1111, saldo: $1000) y (numero: 2222, saldo: $500).
        * Tiene cuentas: Juan Perez tiene la cuenta 1111 y Diego Gonzalez tiene la cuenta 2222.

### Diseño de Base de Datos

**Diseñar una Base de Datos** es construir un **Esquema** (que defina su estructura) y **Especificar el comportamiento esperado**, osea sus **Propiedades** que las instancias deben satisfacer. Estas propiedades se les llama **Restricciones de Integridad**.
<br> En Resumen **Diseño de Base de Datos = Estructura + Restricciones de Integridad**.

#### ¿Para que es necesario definir las restricciones de integridad?

Para la validacion de las instancias, cada vez que se **Modifica una instancia** (**Agregar**, **Eliminar**, **Actualizar Datos**) se debe verificar que las restricciones de integridad se mantengan.

Existen dos **Tipos distintos de esquemas de Base de Datos**:

* **Diseño de modelos de entidad-relacion**.
* **Diseño de modelos Relacional**.

### Diseño de Entidad-Relacion

Se modela la Base de Datos de una organizacion como una **Coleccion de Entidades y Relaciones**. Un diseño de entidad-relacion se representa diagramaticamente.

* **Entidad**: Es un objeto en una organizacion destinguible de otros objetos, se describe por medio de atributos.

    - **Atributo**: Es una **propiedad** de una entidad, esta propiedad tiene un valor en un dominio.

        * **Dominio**: Es un conjunto de valores.

* **Relacion**: Es una asociacion entre entidades.

#### Ejemplo

![Ejemplo de Diagrama de Entidad-Relacion](../Base_de_Datos/Imagenes/Ejemplo_Diagrama_Entidad-Relacion.png)

* Los **Ovalos** son los atributos.
* Los **Rectangulos** son los conjuntos de entidades.
* Los **Rombos** son los conjuntos de relaciones.

### Diseño Relacional

Un **Esquema Relacional** es una **Lista de nombres de atributos**. Los esquemas relacionales tiene **Dos Partes**:

* Nombre de esquema = Lista de nombre de atributo.

    - Por ejemplo: Instructor = (ID, nombre, nombre de departamento, salario).

Una **Instancia** de un esquema relacional es una **Tabla**, esta tabla se le llama **Relacion**

### Modelo Relacional

Los datos (instancias) son almacenados en **Tablas**. Por ejemplo: Una tabla en el modelo relacional:

![Ejemplo de Modelo Relacional](../Base_de_Datos/Imagenes/Ejemplo_Modelo_Relacional.png)

* Las columnas representan **Atributos** (o propiedades) para los elementos de la tabla (tuplas).

### Esquemas e Instancias Relacionales

Una **Instancia** de un diseño de Base de Datos relacional son las **Tablas para los esquemas** de la misma.

* **Notacion**: $r(R)$ significa $r$, donde es una relacion (tabla) con esquemas de la relacion $R$, o sea, las columnas de $r$ tienen como nombres los atributos de $R$.

### Atributos

