# oracle-sales-package
Paquete PL/SQL para la gestión de ventas con control de órdenes, alta de ítems y reportes de clientes. Incluye manejo de excepciones y sobrecarga de procedimientos.

Desafío:
Crear un paquete PA_VENTAS que contenga lo siguiente:

1) Función pública que recibe el ID de una orden y devuelve TRUE o FALSE dependiendo de si la orden existe o no (esta función NO CANCELA. Debe retornar booleano).

2) Procedimiento que permita dar de alta un ítem.
- Recibe por parámetros: nombre del producto, ID de la orden y cantidad.
- El ID del ítem se debe calcular como el siguiente para la orden indicada.
- Se debe validar con la función del punto anterior que la orden exista. De lo contrario mostrar un mensaje y salir del procedimiento sin cancelar.
- El precio debe ser el precio de lista vigente.
- Informar con un mensaje si se pudo realizar el alta.
- Utilizar la función del punto 3 para obtener el ID del producto.
- No debe cancelar, solo emitir mensajes.

3) Función privada que retorne el ID de un producto.
- Recibirá por parámetro el nombre descriptivo del producto y devolverá el ID.
- En caso de no poder hallar el dato, provocar una excepción propia.

4) Procedimiento que muestre los datos de un cliente.
- Recibe por parámetro el ID de cliente o no recibe ningún parámetro (utilizar sobrecarga. No duplicar código).
- Mostrar su nombre, vendedor, cantidad de órdenes y un detalle de órdenes e ítems.
- Para cada orden mostrar fecha, total y el detalle de ítems.
- Si el cliente no tiene compras, indicarlo con un mensaje.
- Si no recibe parámetro, listar para todos los clientes.
- Presentarlo como en el ejemplo. Ordenado por número de orden.

<img width="424" height="251" alt="image" src="https://github.com/user-attachments/assets/68b55e2b-f352-41a7-9ffd-a3ef6add134f" />

Desarrollé este paquete como un desafío personal para poner a prueba y perfeccionar mis habilidades en PL/SQL. Aunque el código cumple con todos los requerimientos y reglas de negocio solicitadas, siempre busco evolucionar mi técnica: el feedback constructivo y las mejores prácticas son siempre bienvenidos. 🦾

