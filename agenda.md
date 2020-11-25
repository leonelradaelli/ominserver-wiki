# getTypes
Genera la estructura de la agenda de la empresa.

### Eventos
* **success**: Acción correcta. Se devuelve en el payload la estructura de la agenda.


# updateType
Actualiza un item de la agenda. Por ejemplo un campo select.
* **activo** _boolean_: Activa/desactiva temporalmente el campo de la agenda
* **borrado** _boolean_: Desactiva permanentemente el campo
* **id** _int_: Id del campo a modificar
* **listar** _boolean_: Determina si se muestra o no en la tabla de agenda
* **nombre** _str_: Nombre del campo
* **obligatorio** _boolean_: false: Determina si es obligatoria la carga
* **orden** _int_: Orden del campo dentro del formulario
* **placeholder** _str_: Valor  
* **primario** _boolean_: Determina si es identificatorio del cliente. Seria primario un campo nombre y apellido por ejemplo, o un legajo

### Eventos
* **success**: Acción correcta. Se devuelve en el payload una colección de mensajes que representan el caso.
