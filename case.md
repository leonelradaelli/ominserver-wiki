# getCase
Genera una colección de los mensajes recibidos y enviados del caso
* **bot_id** _str_: Id del canal relacionado al caso
* **id_servicio** _str_: Identificador relacionado al caso

### Eventos
* **success**: Acción correcta. Se devuelve en el payload una colección de mensajes que representan el caso.


# setCaseLeido
Actualiza todos los mensajes relacionados de un caso a estado leido.
* **bot_id** _str_: Id del canal relacionado al caso
* **id_servicio** _str_: Identificador relacionado al caso

### Eventos
* **success**: Actualización correcta.


# sendMsg
Envía un mensaje al caso y por consiguiente al cliente. Se le avisará a todas las sesiones activas de este usuario. Además se actualizará el
estado del caso a respondido.
* **bot_id** _str_: Id del canal relacionado al caso.
* **id_servicio** _str_: Identificador relacionado al caso.
* **mensaje** _str_: Mensaje a enviar.

### Eventos
* **success**: Actualización correcta. Devuelve el mensaje insertado en el payload.


# close
Cierra un caso.
* **bot_id** _str_: Id del canal relacionado al caso.
* **id_servicio** _str_: Identificador relacionado al caso.
* **tipo** _int_: Id de tipo de cierre a efectuar.

### Eventos
* **success**: Actualización correcta.


# transfer
Transsfiere un caso a otro usuario de la entidad.
* **bot_id** _str_: Id del canal relacionado al caso.
* **id_servicio** _str_: Identificador relacionado al caso.
* **comentarios** _str_: Comentario de la transferencia.
* **tipo** _int_: Id de tipo de transferencia.
* **receptor** _int_: Id del usuario al que se lo transfiere.

### Eventos
* **success**: Transferencia correcta.

# changeState
Actualiza el estado subjetivo de un caso. Se le avisará a todas las sesiones activas de este usuario.
* **bot_id** _str_: Id del canal relacionado al caso.
* **id_servicio** _str_: Identificador relacionado al caso.
* **tipo** _str_:  Id de tipo de estado subjetivo(tiene que estar activo).