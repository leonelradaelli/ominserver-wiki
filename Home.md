Cada archivo de la documentacón representa a un topic para comunicarse y subscribirse al [servidor API](http://omnicanalapi.tech/) de omnicanal. La conexión está basada en [socket.io](https://socket.io/).

Dentro de cada archivo se especifican las diferentes acciones disponibles para el topic y los parametros necesarios para efectuarlas.

***

Ej: 
`socket.io.emit("sesion", {
    action: 'login',
    id: 1,
    token: 'abc123'
})`