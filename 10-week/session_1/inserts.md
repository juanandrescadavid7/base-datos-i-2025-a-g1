INSERT INTO categoria (nombre, descripcion) VALUES
('Electrónica', 'Dispositivos y productos electrónicos de consumo'),
('Ropa', 'Prendas de vestir para todos los géneros'),
('Alimentos', 'Comestibles y bebidas'),
('Muebles', 'Muebles para el hogar'),
('Deportes', 'Equipos y accesorios deportivos');



INSERT INTO producto (nombre, descripcion, categoria_id) VALUES
('Smartphone', 'Teléfono móvil inteligente', 1),
('Laptop', 'Computadora portátil', 1),
('Camiseta', 'Camiseta de algodón', 2),
('Jeans', 'Pantalones de mezclilla', 2),
('Galletas', 'Galletas de chocolate', 3),
('Silla', 'Silla de oficina ergonómica', 4),
('Pelota', 'Pelota de fútbol', 5);


INSERT INTO persona (nombre, apellido, fecha_nacimiento, correo, direccion, telefono) VALUES
('Juan', 'Pérez', '1985-05-12', 'juanperez@email.com', 'Calle Falsa 123', '555-1234'),
('María', 'González', '1990-03-25', 'mariagonzalez@email.com', 'Avenida Siempre Viva 456', '555-5678'),
('Carlos', 'Sánchez', '1978-10-30', 'carlossanchez@email.com', 'Calle Real 789', '555-8765'),
('Ana', 'Rodríguez', '1982-08-22', 'anarodriguez@email.com', 'Calle Luna 101', '555-4321'),
('Luis', 'Martínez', '1995-01-05', 'luismartinez@email.com', 'Calle Sol 102', '555-3456');


INSERT INTO cliente (codigo, fecha_vinculacion, persona_id) VALUES
('CL001', '2023-01-15', 1),
('CL002', '2023-02-20', 2),
('CL003', '2023-03-10', 3),
('CL004', '2023-04-01', 4),
('CL005', '2023-04-05', 5);


INSERT INTO empleado (codigo, fecha_vinculacion, salario, tipo_contrato, persona_id) VALUES
('EM001', '2020-06-25', 35000.00, 'Indefinido', 1),
('EM002', '2021-07-10', 30000.00, 'Temporal', 2),
('EM003', '2022-01-05', 25000.00, 'Indefinido', 3),
('EM004', '2020-11-12', 28000.00, 'Indefinido', 4),
('EM005', '2022-09-01', 32000.00, 'Temporal', 5);


INSERT INTO metodo_pago (nombre, descripcion) VALUES
('Tarjeta de Crédito', 'Pago con tarjeta de crédito'),
('Transferencia Bancaria', 'Pago mediante transferencia desde cuenta bancaria'),
('Efectivo', 'Pago en efectivo en tienda'),
('PayPal', 'Pago online mediante PayPal'),
('Bitcoin', 'Pago utilizando criptomoneda Bitcoin');


INSERT INTO inventario (nombre, fecha, precio, stock, fecha_lote, fecha_vencimiento, producto_id) VALUES
('Smartphone', '2023-03-01', 500.00, 100, '2023-02-01', '2025-03-01', 1),
('Laptop', '2023-03-15', 800.00, 50, '2023-02-15', '2025-03-15', 2),
('Camiseta', '2023-03-10', 20.00, 200, '2023-02-10', '2025-03-10', 3),
('Jeans', '2023-03-18', 30.00, 150, '2023-02-18', '2025-03-18', 4),
('Galletas', '2023-03-20', 2.50, 500, '2023-02-20', '2024-03-20', 5),
('Silla', '2023-03-25', 75.00, 80, '2023-02-25', '2025-03-25', 6),
('Pelota', '2023-03-28', 15.00, 120, '2023-02-28', '2025-03-28', 7);


INSERT INTO factura (codigo, fecha, valor_bruto, valor_descuento, valor_incremento, valor_neto, cliente_id, medio_pago_id) VALUES
('FAC001', '2023-04-10', 500.00, 50.00, 0.00, 450.00, 1, 1),
('FAC002', '2023-04-11', 800.00, 0.00, 0.00, 800.00, 2, 2),
('FAC003', '2023-04-12', 100.00, 10.00, 5.00, 95.00, 3, 3),
('FAC004', '2023-04-13', 150.00, 15.00, 5.00, 140.00, 4, 4),
('FAC005', '2023-04-14', 200.00, 20.00, 10.00, 190.00, 5, 5);


INSERT INTO detalle_factura (cantidad, porcentaje_descuento, porcentaje_incremento, subtotal, producto_id, factura_id) VALUES
(1, 10.00, 0.00, 450.00, 1, 1),
(2, 0.00, 5.00, 800.00, 2, 2),
(3, 5.00, 0.00, 95.00, 3, 3),
(1, 10.00, 5.00, 140.00, 4, 4),
(4, 5.00, 10.00, 190.00, 5, 5);