# TA13

-	Primary key: <b>negrita</b>
-	Foreign key: subrayado

•	Ejercicio 1
Atleta (numero_dorsal, nombre, dorsal reemplazo)

•	Ejercicio 2
Elemento (nombre_elemento¸peso_atómico, símbolo, num_atómico)
Compuesto_por(nombre_compuesto, nombre_elemento, proporción)
Gaseoso (nombre_compuesto, estado, coef_expansion, temp_lic)
Líquido (nombre_compuesto, estado, densidad, temperatura_evaporacion)
Sólido (nombre_compuesto, estado, color, olor, dureza)

•	Ejercicio 3
Sucursal (num_surcursal, ciudad, activo)
Cliente (DNI, num_surcursal, nombre, apellidos, dirección, ciudad)
Cuenta (num_cuenta, num_surcursal, saldo)
Abrir (num_cuenta, DNI)
Transacción (num_transacción, num_cuenta, fecha, tipo_operación, cantidad)

•	Ejercicio 4
Parque_bomberos (cod_parque, nombre, dirección, teléfono, categoría)
Coche (num_coche, cod_parque, marca, modelo, num_matrícula, fecha_compra, fecha_ult_rev)
Bombero (cod_bombero, cor_parque, cod_turno, nombre, apellidos, fecha_nac, DNI, dirección, teléfono, puesto, cod_equipo)
Trabaja_en (cod_bombero, fecha_inicio, fecha_fin)
Turno (cod_turno, descripción)
Período (fecha_inicio, fecha¬_fin, cod_turno)
Petición_servicio (cod_pet_serv, tipo_serv, grado_urgencia, cod_equipo)
Recibe (cod_parque, cod_pet_serv, fecha, hora)
Equipo (cod_equipo, nombre)

•	Ejercicio 5
Préstamo (num_préstamo, fecha_prestamo, num_socio, signatura)
Socios (num_socio, nombre, apellidos, teléfono, fecha¬_cad)
Sanción (num_días, num_socio)
Préstamos_s (num_préstamo, tipo)
Préstamo_e (num_préstamo, fecha¬_devolución, tipo)
Libro (signatura, disponible, titulo, autor)
Fondo (titulo, autor, cantidad)	

•	Ejercicio 6 
Cliente (cod_cliente)
Pedido (cod_pedido, fecha¬_pedido, cod¬_cliente, cod_producto, num_unidades)
Producto (cod_producto, cantidad, cod_proveedor, unidades, fecha_encargo)
Proveedor (cod_proveedor)

•	Ejercicio 7
Arrendatario (CIF_NIF, nombre_fiscal, nombre_firmante, carga_firmante, dirección, código postal, localidad, provincia, teléfono_fijo, teléfono_móvil, fax, actividad)
Nave (código_nave, polígono, calle, número, localidad, código_postal, provincia, teléfono, características, foto, datos¬_escritura, alquilada, gastos_comunidad CIF_NIF, número_cuenta, días_pago, fecha_alquiler, fecha_fin_alquiler, importe_alquiler)
Recibo (número_recibo, importe_total, importe_IVA, pagado, fecha, código_nave, CIF_NIF)

•	Ejercicio 8
Piso (puerta, DNI, nombre, apellidos, dirección, código_postal, localidad, provincia, teléfono)
Cargo (código_cargo, nombre, funciones)
Ostenta(código_cargo, puerta, fecha_posesión)
Anotación (código_anotación, fecha, importe)
Ingreso_recibo (código_anotación, mes, pagado, puerta)
Ingreso_extra (código_anotación, concepto)
Gasto_fijo (código_anotación, fecha_inicio, fecha_fin, consumo, código_tipo_gasto)
Gasto_variable (código_anotación, fecha_facturación, concepto, número_factura)
Tipo_gasto_fijo (código_tipo_gasto, nombre, descripción)
Detalle_recibo (número¬_línea, concepto, importe, código¬_anotación)
