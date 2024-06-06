# save
Crea o edita un cliente de la empresa.
* **bot_id** _str_: Id del canal relacionado al caso.
* **id_servicio** _str_: Identificador relacionado al caso.
* **id** _int_: Id del cliente a editar. Si se esta creando uno nuevo este debe ser 0.
* **campos** [ _campoCliente_ ]: Lista de campos del cliente a guardar. Cada objeto campoCliente tiene la forma:
  * **tipo** _int_: Id del tipo del campo a guardar.
  * **valor** _str_: Valor del campo a guardar.

### Eventos
* **success**: Actualización correcta.

# attach
Relaciona un caso con un cliente preexistente.
* **bot_id** _str_: Id del canal relacionado al caso.
* **id_servicio** _str_: Identificador relacionado al caso.
* **id** _int_: Id del cliente a relacionar.

### Eventos
* **success**: Actualización correcta. Se envia en el payload el objeto AgendaCliente recien insertado.

# deattach
Borra la relación de un caso con un cliente.
* **bot_id** _str_: Id del canal relacionado al caso.
* **id_servicio** _str_: Identificador relacionado al caso.
* **id** _int_: Id del cliente a relacionar.

### Eventos
* **success**: Actualización correcta. Se envia en el payload el objeto AgendaCliente eliminado.