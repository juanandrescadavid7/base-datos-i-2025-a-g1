-- Actualizar el nombre y descripción de una categoría
UPDATE categoria SET nombre = 'Tecnología', descripcion = 'Productos tecnológicos' WHERE id = 1;

-- Actualizar el nombre y descripción de un producto
UPDATE producto SET nombre = 'Smartphone Pro', descripcion = 'Teléfono móvil inteligente con mejores características' WHERE id = 1;

-- Actualizar la fecha de nacimiento de una persona
UPDATE persona SET fecha_nacimiento = '1986-06-25' WHERE id = 1;

-- Actualizar el correo electrónico de un cliente
UPDATE cliente SET codigo = 'CL006' WHERE id = 5;

-- Actualizar el salario de un empleado
UPDATE empleado SET salario = 36000.00 WHERE id = 1;

-- Actualizar el tipo de contrato de un empleado
UPDATE empleado SET tipo_contrato = 'Por obra' WHERE id = 2;

-- Actualizar el precio de un producto en el inventario
UPDATE inventario SET precio = 550.00 WHERE id = 1;

-- Actualizar el stock de un producto
UPDATE inventario SET stock = 120 WHERE id = 1;

-- Actualizar la dirección de un cliente
UPDATE persona SET direccion = 'Calle Nueva 123' WHERE id = 2;

-- Actualizar el valor bruto de una factura
UPDATE factura SET valor_bruto = 520.00 WHERE id = 1;

-- Actualizar el valor de descuento en una factura
UPDATE factura SET valor_descuento = 60.00 WHERE id = 2;

-- Actualizar el porcentaje de descuento en un detalle de factura
UPDATE detalle_factura SET porcentaje_descuento = 15.00 WHERE id = 1;

-- Actualizar la cantidad de productos en un detalle de factura
UPDATE detalle_factura SET cantidad = 2 WHERE id = 2;


