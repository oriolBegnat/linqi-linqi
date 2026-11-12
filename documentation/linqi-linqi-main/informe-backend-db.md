---
description: Información para almacenar en la base de datos de mi proyecto
---

# Informe Backend - DB

#### 1. **Descripción general del proyecto web**

* **¿De qué trata tu web?**

Aplicación web diseñada para el aprendizaje y la práctica acerca de la masterización de audio.

* **¿Qué funcionalidades ofrecerá a los usuarios?**

La aplicación permite al usuario crearse una cuenta, crear proyectos, añadir y modificar efectos, e importar sus propios archivos de audio MP3 y para después, exportarlo de vuelta con el resultado final.

#### 2. **Identificación de entidades principales**

* **¿Qué elementos importantes hay en tu web que necesitan almacenarse?**

Los elementos que deberán almacenarse son los datos de usuarios y sus proyectos, datos de los audios subidos y datos sobre los efectos.

**¿Qué tema de información almacena?**&#x20;

* _UserProfile_
* _Project_
* _Audio_
* _Effect_

<figure><img src="../.gitbook/assets/Diagrama Entidad-Relación linqi-linqi.png" alt=""><figcaption></figcaption></figure>

#### 3. **Datos que se deben guardar de cada entidad (atributos)**

<details>

<summary><em><strong>UserProfile</strong></em></summary>

* Nombre de usuario — Texto — VARCHAR
* Nombre — Texto — VARCHAR
* Apellidos — Texto — VARCHAR
* Correo electrónico — Texto — VARCHAR
* Contraseña — Texto — VARCHAR
* Fecha de registro  — Fecha — TIMESTAMP

</details>

<details>

<summary><em><strong>Project</strong></em></summary>

* Nombre de proyecto — Texto — VARCHAR
* Fecha de creación — Fecha — TIMESTAMP
* Fecha de modificación — Fecha — DATETIME

</details>

<details>

<summary><em><strong>Audio</strong></em></summary>

* Nombre de audio — Texto — VARCHAR
* Tamaño (MB) — Número — DECIMAL
* Fecha de subida — Fecha — DATETIME

</details>

<details>

<summary><em><strong>Effect</strong></em></summary>

* Nombre de efecto — Texto — VARCHAR
* Descripción — Texto — TEXT
* URL — Texto — VARCHAR

</details>

#### 4. **Relaciones entre las entidades**

¿Cómo se relacionan unas entidades con otras?

* Un usuario puede crear muchos proyectos.
* Un proyecto solo puede tener un audio.
*

#### 5. **Ejemplo de datos (simulación)**

{% tabs %}
{% tab title="UserProfile" icon="user" %}
* _Nombre de usuario:_ ackackack
* _Nombre:_ Oriol
* _Apellidos:_ Peña
* _Email:_ [openaopena@gmail.com](https://dmuwut6e40u5o.cloudfront.net/ultra/uiv4001.4.0-rel.31_82fdb43)
* _Contraseña:_ a5d1d4bd24b50c460c023388de22b15ebc4d70c86619bcd2347fb35ae04526105bca2b224da0c9cba49f57f9c7a5c25cd7d9e30d71e76d9ca91e11ae27276580
* _Fecha de registro:_ 10/09/2026
{% endtab %}

{% tab title="Project" icon="folder" %}
* _Nombre de proyecto:_ Proyecto 1
* _Fecha de creación:_ 10/09/2026
* _Fecha de modificación:_ 13/09/2026
{% endtab %}

{% tab title="Audio" icon="volume-high" %}
* _Nombre de audio:_ Maqueta\_20261006
* _Tamaño (MB)_: 12.30
* _Fecha de subida:_ 10/09/2026
{% endtab %}

{% tab title="Effect" icon="waveform" %}
* _Nombre de efecto:_ EQ
* _Descripción: "_&#x55;n ecualizador paramétrico (EQ paramétrico) es una herramienta de procesamiento de audio que permite modificar el volumen de frecuencias específicas con total precisión."
* _URL:_ ¯\\\_(o.o')\_/¯
{% endtab %}
{% endtabs %}

#### 6. Reflexiones, d**ificultades y dudas que tienes sobre la base de datos**

Pensar tanto en los datos, como en todas las posibles relaciones y, tratar de darle forma teniendo delante una hoja en blanco es, por mucho, lo que se ha antojado más difícil inicialmente.

Las dudas que pueda tener ahora, son más por toda la información y/o tablas que puedan surgir según avance el proyecto.

