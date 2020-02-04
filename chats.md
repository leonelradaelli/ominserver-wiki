# getHome
Genera una lista con los casos del usuario y los casos que no fueron asignados(estos ultimos max 50).
* **no necesita parametros**
### Eventos
* **success**: Acción correcta. Se devuelve en el payload una colección de mensajes que representan el home


# adopt
Asigna al usuario actual el caso seleccionado. Se notifica al resto de los usuarios de la entidad esta acción.
* **bot_id** _str_: Id del canal relacionado al caso
* **id_servicio** _str_: Identificador relacionado al caso

Además se recibirá esta misma acción cuando un tercero adopte un caso. El cliente deberia borrar todos los mensajes pertenecientes al caso. El evento vendrá con los siguientes valores:
* **bot** _str_: Id del canal del caso adoptado.
* **servicio** _str_: Identificador del caso adoptado.
* **by** _int_: Id del usuario que adopto el caso

### Eventos
* **success**: Actualización correcta. Se notifica a todos los usuarios el caso recien adoptado y el id del usuario que realizo la accion.

# newMsg
De este evento solo se puede recibir. El cliente lo recibirá cuando le llegue un mensaje nuevo de uno de sus casos o de sus canales.