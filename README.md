# p02_ModeloEntidad-Relacion_Viveros
Descripcion de las entidades: 
  1. Viveros, instalaciones fisicas de la empresa
  2. Zonas, las diferentes zonas dentro de los viveros
  3. Producto, los diferentes productos vendidos por la empresa
  4. Empleado, los trabajadores destinados a los viveros
  5. Cliente, aquellos que pertenecen al programa Tajinaste Plus
  6. Pedid, las compras realizadas por los clientes fidelizados
Descripcion de los atributos de las entidades y relaciones:
  1. Viveros: Coordenadas, refleja la latitud y longitud de la localizacion fisica.
     ID_Vivero, codigo de identificacion del vivero
  2. Zona: Coordenadas, refleja la latitud y longitud de la localizacion fisica.
     ID_Zona: codigo de identificacion de la zona
  3. Producto: ID_Producto, codigo de identificacion del producto
  4. Empleado: Id_Empleado, codigo de identificacion del empleado
  5. Pedido: ID_Pedido, codigo de identificacion del pedido
  6. Cliente: ID_cliente, codigo de identificacion del cliente
     Compras, volumen de compras en un mes
     Bonificaciones, bonificaciones obtenidas por ese cliente
  7. Relacion Zona-Producto: Stock, cantidad de producto disponible en esa zona
  8. Relacion Empleado-Zona: Historico Destinos, registro de las diferentes zonas a las que ha sido asignado un empleado
  9. Relacion Producto-Pedido: Cantidad, numero de productos vendidos en ese pedido
     Precio, coste del pedido
Descripcion de cada una de las relaciones:
  1. Vivero-Zona, relacion uno a muchos, un vivero puede tener muchas zonas, una zona solo puede estar contenida en un vivero, relacion de dependencia, sin vivero no puede existir una zona
  2. Zona-Producto, relacion muchos a muchos, una zona puede tener muchos productos y un mismo producto puede estar en varias zonas
  3. Empleado-Zona, muchos a muchos, una misma zona puede tener varios empleados asignados y un mismo empleado puede haber sido asignado durante un periodo prolongado de tiempo a varias zonas, no obstante no puede pertenecer a dos zonas a la vez en un mismo periodo
  4. Empleado-Pedido, uno a muchos, un mismo empleado puede gestionar varios pedidos pero un pedido solo puede ser gestionado por un empleado
  5. Pedido-Cliente, uno a muchos, un mismo cliente puede realizar varios pedidos, pero un pedido solo puede ser realizado por un unico cliente
  6. Pedido-Producto, muchos a muchos, un pedido puede contener muchos productos y muchas unidades del mismo, un mismo producto puede aparecer en varios pedidos
