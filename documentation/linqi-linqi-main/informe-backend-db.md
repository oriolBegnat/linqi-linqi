# Informe Backend - DB

#### "Información para almacenar en la base de datos de mi proyecto"

#### 1. **Descripción general del proyecto web**

* **¿De qué trata tu web?**

WebApp para practicar y aprender sobre la masterización de audio.

* **¿Qué funcionalidades ofrecerá a los usuarios?**

La aplicación permite al usuario crearse una cuenta, crear proyectos, añadir y modificar efectos, e importar sus propios archivos de audio MP3 y exportarlo de vuelta.

#### 2. **Identificación de entidades principales**

* **¿Qué elementos importantes hay en tu web que necesitan almacenarse?**

Los elementos que deberán almacenarse son los datos de usuarios y sus proyectos, datos de los audios subidos y datos sobre los efectos.

1. **¿Qué tema de información almacena?** \
   Usuarios, proyectos, efectos y audios.
2. <mark style="color:$warning;">**¿Por qué necesitas guardarla en la base de datos?**</mark> _<mark style="color:$warning;">-> Esto nos ayudará a entender si es necesario guardar esta información o no.</mark>_

#### 3. **Datos que se deben guardar de cada entidad (atributos)**

**Usuario**:

* Nombre de usuario — Texto — VARCHAR
* Nombre — Texto — VARCHAR
* Apellidos — Texto — VARCHAR
* Correo electrónico — Texto — VARCHAR
* Contraseña — Texto — VARCHAR
* Fecha de registro  — Fecha — TIMESTAMP

**Proyecto**:

* Nombre de proyecto — Texto — VARCHAR
* Fecha de creación — Fecha — TIMESTAMP
* Fecha de modificación — Fecha — DATETIME

**Audio**:

* Nombre de audio — Texto — VARCHAR
* Tamaño (MB) — Número — DECIMAL
* Fecha de subida — Fecha — DATETIME

**Efecto**:

* Nombre de efecto — Texto — VARCHAR
* Descripción — Texto — TEXT
* URL — Texto — VARCHAR

#### 4. **Relaciones entre las entidades**

¿Cómo se relacionan unas entidades con otras?

* Un usuario puede crear muchos proyectos.
* Un proyecto solo puede tener un audio.
*

#### 5. **Ejemplo de datos (simulación)**

* Incluye un ejemplo de cada entidad con datos ficticios pero realistas.

_Ejemplo de registro en la tabla **Usuario**:_

* _Nombre de usuario: ackackack_
* _Nombre: Oriol_
* _Apellidos: Peña_
* _Email:_ [_openaopena@gmail.com_](https://dmuwut6e40u5o.cloudfront.net/ultra/uiv4001.4.0-rel.31_82fdb43)
* _Fecha de registro: 10/09/2026_

🎯 **Objetivo:** Ver si los datos que se han pensado tienen sentido y si falta algo importante.

#### 6. Reflexiones, d**ificultades y dudas que tienes sobre la base de datos**

* ¿Qué partes te han resultado más difíciles de pensar?

Lo que se ha antojado más difícil inicialmente ha sido pensar tanto en los datos como en todas las posibles relaciones y después, tratar de darle forma estando ante una hoja en blanco.

* <mark style="color:$warning;">¿Qué no tienes claro sobre la información que hay que guardar?</mark>



* <mark style="color:$warning;">Cualquier pregunta que se os ocurra mientras realizabas el informe.</mark>

