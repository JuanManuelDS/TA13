# TA13

-	Primary key: <b>negrita</b>
-	Foreign key: <u>subrayado</u>

•	Ejercicio 1
Atleta (<b>numero_dorsal</b>, nombre, <u>dorsal_reemplazo</u>)

•	Ejercicio 2
Elemento (<b>nombre_elemento</b>¸peso_atómico, símbolo, num_atómico)<br/>
Compuesto_por(<b>nombre_compuesto</b>, nombre_elemento, proporción)<br/>
Gaseoso (<b>nombre_compuesto</b>, estado, coef_expansion, temp_lic)<br/>
Líquido (<b>nombre_compuesto</b>, estado, densidad, temperatura_evaporacion)<br/>
Sólido (<b>nombre_compuesto</b>, estado, color, olor, dureza)<br/>

•	Ejercicio 3
Sucursal (<b>num_surcursal</b>, ciudad, activo)<br/>
Cliente (<b>DNI</b>, <b><u>num_surcursal</u></b>, nombre, apellidos, dirección, ciudad)<br/>
Cuenta (<b>num_cuenta</b>, <b><u>num_surcursal</u></b>, saldo)<br/>
Abrir (<b><u>num_cuenta</u></b>, <b><u>DNI</u></b>)<br/>
Transacción (<b>num_transacción</b>, <b><u>num_cuenta</u></b>, fecha, tipo_operación, cantidad)<br/>

•	Ejercicio 4
Parque_bomberos (<b>cod_parque</b>, nombre, dirección, teléfono, categoría)<br/>
Coche (<b>num_coche</b>, <b><u>cod_parque</u></b>, marca, modelo, num_matrícula, fecha_compra, fecha_ult_rev)<br/>
Bombero (<b>cod_bombero</b>, <u>cod_parque</u>, <u>cod_turno</u>, nombre, apellidos, fecha_nac, DNI, dirección, teléfono, puesto, <u>cod_equipo</u>)<br/>
Trabaja_en (<b><u>cod_bombero</u></b>, <b><u>fecha_inicio</u></b>, <b><u>fecha_fin</u></b>)<br/>
Turno (<b>cod_turno, descripción</b>)<br/>
Período (<b>fecha_inicio</b>, <b>fecha_fin</b>, <u>cod_turno</u>)<br/>
Petición_servicio (<b>cod_pet_serv</b>, tipo_serv, grado_urgencia, <u>cod_equipo</u>)<br/>
Recibe (<b><u>cod_parque</u></b>, <b><u>cod_pet_serv</u></b>, fecha, hora)<br/>
Equipo (<b>cod_equipo</b>, nombre)<br/>

•	Ejercicio 5
Préstamo (<b>num_préstamo</b>, fecha_prestamo, <u>num_socio</u>, <u>signatura</u>)<br/>
Socios (<b>num_socio</b>, nombre, apellidos, teléfono, fecha_cad)<br/>
Sanción (<b>num_días</b>, <u>num_socio</u>)<br/>
Préstamos_s (<b><u>num_préstamo</u></b>, tipo)<br/>
Préstamo_e (<b><u>num_préstamo</u></b>, fecha_devolución, tipo)<br/>
Libro (<b>signatura</b>, disponible, <u>titulo</u>, <u>autor</u>)<br/>
Fondo (<b>titulo</b>, <b>autor</b>, cantidad)	<br/>

•	Ejercicio 6 
Cliente (<b>cod_cliente</b>)<br/>
Pedido (<b>cod_pedid</b>o, fecha_pedido, <u>cod_cliente</u>, <u>cod_producto, num_unidades</u>)<br/>
Producto (<b>cod_producto</b>, cantidad, <u>cod_proveedor</u>, unidades, fecha_encargo)<br/>
Proveedor (<b>cod_proveedor</b>)<br/>

•	Ejercicio 7
Arrendatario (<b>CIF_NIF</b>, nombre_fiscal, nombre_firmante, carga_firmante, dirección, código postal, localidad, provincia, teléfono_fijo, teléfono_móvil, fax, actividad)<br/>
Nave (<b>código_nave</b>, polígono, calle, número, localidad, código_postal, provincia, teléfono, características, foto, datos_escritura, alquilada, gastos_comunidad, <u>CIF_NIF</u>, número_cuenta, días_pago, fecha_alquiler, fecha_fin_alquiler, importe_alquiler)<br/>
Recibo (<b>número_recibo</b>, importe_total, importe_IVA, pagado, fecha, <u>código_nave</u>, <u>CIF_NIF</u>)<br/>

•	Ejercicio 8
Piso (<b>puerta</b>, DNI, nombre, apellidos, dirección, código_postal, localidad, provincia, teléfono)<br/>
Cargo (<b>código_cargo</b>, nombre, funciones)<br/>
Ostenta(<b>código_cargo</b>, <b>puerta</b>, fecha_posesión)<br/>
Anotación (<b>código_anotación</b>, fecha, importe)<br/>
Ingreso_recibo (<b><u>código_anotación</u></b>, mes, pagado, puerta)<br/>
Ingreso_extra (<b><u>código_anotación</u></b>, concepto)<br/>
Gasto_fijo (<b><u>código_anotación</u></b>, fecha_inicio, fecha_fin, consumo, código_tipo_gasto)<br/>
Gasto_variable (<b><u>código_anotación</u></b>, fecha_facturación, concepto, número_factura)<br/>
Tipo_gasto_fijo (<b>código_tipo_gasto</b>, nombre, descripción)<br/>
Detalle_recibo (<b>número_línea</b>, concepto, importe, <b><u>código_anotación</u></b>)<br/>
