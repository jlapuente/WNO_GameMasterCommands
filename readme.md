# Guía de comandos

En esta sección se detallan los comandos disponibles, su uso y los parámetros requeridos.

## Comando: `/SetRagdollInfo`

- **Descripción**: Este comando permite crear cadaveres para roles médicos o ambientaciones.
- **Uso**: `/SetRagdollInfo <nombre> <motivo_muerte>`
- **Parámetros**:
  - `<nombre>`: El nombre del cadaver. *(Opcional)* Si no se especifica, se generará uno aleatoriamente.
  - `<motivo_muerte>`: El motivo de la muerte. *(Opcional)* Si no se especifica, se generará uno aleatoriamente.
  
- **Ejemplo**:
    ```bash
    /SetRagdollInfo "Paquita Salas"
    /SetRagdollInfo "" "Muerte cerebral"
    /SetRagdollInfo
    ```

---

## Comando: `/PlaySound`

- **Descripción**: Reproduce un sonido para todos los jugadores (si no se introduce rango) o para los jugadores en el rango.
- **Uso**: `/PlaySound <sound> <range>`
- **Parámetros**:
  - `<sound>`: La ruta al sonido. *(Obligatorio)*
  - `<range>`: La distancia a la que se oirá el sonido. 500 es un numero mas que decente.
- **Ejemplo**:
    ```bash
    /PlaySound ambience/wind1.wav 200
    ```

---

## Comando: `/ScreenShake`

- **Descripción**: Shakes the screen of everyone in the specified range. Specify the amplitude, the frequency and the radius for it to work.
- **Uso**: `/ScreenShake <time(seconds)> <amplitude> <frequency> <radius>`
- **Parámetros**:
  - `<time>`: Los segundos que dura. *(Obligatorio)*
  - `<amplitude>`: idk *(Obligatorio)*
  - `<frequency>`: Cada cuanto se repite *(Obligatorio)*
  - `<radius>`: El radio en el que los jugadores recibiran el efecto *(Obligatorio)*
- **Ejemplo**:
    ```bash
    /ScreenShake 20 20 25 500
    ```

---

## Comando: `/LocalEvent`

- **Descripción**: Haz un evento IC de administrador que sólo pueda ser escuchado dentro de un radio determinado.
- **Uso**: `/LocalEvent <mensaje> <radio>` 
- **Parámetros**:
  - `<mensaje>`: El texto que será enviado a los jugadores. *(Obligatorio)*
  - `<radio>`: El rango en el que será mostrado el evento. 500 es un rango mas que aceptable *(Opcional)*
- **Ejemplo**:
    ```bash
    /LocalEvent "El viento recorre fuertemente la calle" 200 
    ```

---

## Comando: `/event`

- **Descripción**: Haz un evento IC de administrador. Se lee en todo el servidor. Usalo solo en casos necesarios.
- **Uso**: `/event message`
- **Parámetros**:
  - `<message>`: Descripción del parámetro. *(Obligatorio)*
- **Ejemplo**:
    ```bash
    /event "Cayó la noche en la ciudad"
    ```
---

## Comando: `/PermanentPropDescriptionAdd`

- **Descripción**: Añade una descripción permanente a un prop.
- **Uso**: `/PermanentPropDescriptionAdd <title> <description>` 
- **Alias**: PermPropDescAdd
- **Parámetros**:
  - `<title>`: El texto que será enviado a los jugadores. *(Obligatorio)*
  - `<description>`: El rango en el que será mostrado el evento. 500 es un rango mas que aceptable *(Opcional)*

- **Ejemplo**:
    ```bash
    /PermanentPropDescriptionAdd "Taza de Mark" "La taza de café del famoso Mark Fontana"
    ```

---

## Comando: `/StaticCharActionAdminSet`

- **Descripción**: Asigna una acción estática a un personaje.
- **Alias**: `/sasa` & `SetAdminAction`
- **Uso**: `/StaticCharActionAdminSet <character> <action>` 
- **Parámetros**:
  - `<character>`: El jugador que recibirá la acción estática. *(Obligatorio)*
  - `<action>`: El rango en el que será mostrado el evento. 500 es un rango mas que aceptable *(Opcional)*

- **Ejemplo**:
    ```bash
    /StaticCharActionAdminSet "Mark" "Tiene la pierna rota"
    ```

---

## Comando: `/notify`

- **Descripción**: @notifyPlayer
- **Uso**: `/notify character text`
- **Parámetros**:
  - `<character>`: Personaje que notificar. *(Obligatorio)*
  - `<text>`: Texto a notificar. *(Obligatorio)*

- **Ejemplo**:
    ```bash
    /notify Pedro "Detectas una hormiga en tu pantalon"
    ```

---

## Comando: `/SetJumpPower`

- **Descripción**: Edita el valor de salto de un personaje.
- **Uso**: `/setjumppower character value`
- **Parámetros**:
  - `<character>`: Personaje *(Obligatorio)*
  - `<value>`: Salto. *(Obligatorio)*

- **Ejemplo**:
    ```bash
    /setjumppower Paco 200
    ```

--- 

## Comando: `/SetRunSpeed`

- **Descripción**: Edita la velocidad al correr de un personaje.
- **Uso**: `/setrunspeed character value`
- **Parámetros**:
  - `<character>`: Personaje *(Obligatorio)*
  - `<value>`: Velocidad. *(Obligatorio)*

- **Ejemplo**:
    ```bash
    /setrunspeed Paco 200
    ```
---

## Comando: `/SetWalkSpeed`

- **Descripción**: Edita la velocidad al andar de un personaje.
- **Uso**: `/setwalkspeed character value`

- **Parámetros**:
  - `<character>`: Personaje *(Obligatorio)*
  - `<value>`: Velocidad. *(Obligatorio)*

- **Ejemplo**:
    ```bash
    /setwalkspeed <valores de ejemplo>
    ```

---

Esta guía cubre algunos de los comandos más comunes en el proyecto. Cada uno puede tener diferentes parámetros según la necesidad.
