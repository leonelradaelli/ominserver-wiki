# login
Inicia sesion en el servidor de sockets. Es el unico topic para el que no se necesita estar logueado. Puede loguearse de dos formas distintas:
* **user** _str_: Username de la cuenta.
* **pass** _str_: Contraseña de la cuenta.

El otro modo es con los siguientes campos:
* **id** _int_: Id del usuario.
* **token** _str_: Token de inicio de sesion del usuario.

### Eventos
* **success**: Login ok, devuelve en el **payload** un objeto entidad con nombre, token y link de su logo.


# setLogueado
Cambia el estado a logueado si/no del usuario.
* **logueado** _bool_: Nuevo estado del usuario.

### Eventos
* **success**: Actualización correcta.


# setPushToken
Cambia el push token del usuario.
* **token** _string_: Nuevo token del usuario.

### Eventos
* **success**: Actualización correcta.


# removePushToken
Elimina un push token del usuario.
* **token** _string_: Token del usuario a eliminar.

### Eventos
* **success**: Actualización correcta.


# timeout
Desloguea al usuario y cierra la conexión.
* **Sin parametros**

### Eventos
* **success**: Actualización correcta.