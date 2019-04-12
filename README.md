Grupo
Integrantes: Ivan Gabriel Marsetti, 0099941
Negocio Elegido: Administracion de Clientes de una Cafeteria

*RESTFUL API*
Crear Cliente
Cartera de Cliente ($)
Compra de producto
Puntos obtenidos - Beneficios
Ingreso dinero

* Crear Cliente
  POST /cliente
  
* Cartera Cliente
  GET /cliente/saldo
  
* Compra de producto
  GET /cliente/id/saldo
  GET /producto/id/precio
  if (saldo < precio){
    X
    else:
    PATCH /cliente/id/saldo = saldo - precio
    PATCH /cliente/id/puntos = puntos + precio * 0,2
  }

* Puntos obtenidos
  GET /cliente/id/puntos
  GET /beneficios
  
* Ingreso dinero
  PATCH /cliente/id/saldo = saldo + ingreso
  
