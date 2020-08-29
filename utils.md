
# getCaseStatusTypes
Genera una lista con los tipos de estados subjetivos que pueden tener los casos:

### Eventos
* **success**: Accion correcta, devuelve en el **payload** una lista types con id, nombre y color en cada item.



# getFreqAnswers
Genera una lista con las respuestas frecuentes del usuario y de la entidad:

### Eventos
* **success**: Accion correcta, devuelve en el **payload** una lista de respuestas frecuentes con id, client(0 para entidad, o el id del usuario) y msg.



# getUsers
Genera una lista con los usuarios para, por ejemplo, transferirles casos:

### Eventos
* **success**: Accion correcta, devuelve en el **payload**  una lista de usuarios con id, user_L y nombre.

