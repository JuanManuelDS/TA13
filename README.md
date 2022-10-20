# TA13

- Primary key: <b>negrita</b>
- Foreign key: <ins>subrayado</ins>

## • Ejercicio 1<br/>

Atleta (<b>numero_dorsal</b>, nombre, <ins>dorsal_reemplazo</ins>)<br/>

## • Ejercicio 2<br/>

Elemento (<b>nombre_elemento</b>¸peso_atómico, símbolo, num_atómico)<br/>
Compuesto_por(<b>nombre_compuesto</b>, <b>nombre_elemento</b>, proporción)<br/>
Gaseoso (<b>nombre_compuesto</b>, estado, coef_expansion, temp_lic)<br/>
Líquido (<b>nombre_compuesto</b>, estado, densidad, temperatura_evaporacion)<br/>
Sólido (<b>nombre_compuesto</b>, estado, color, olor, dureza)<br/>

## • Ejercicio 3<br/>

Sucursal (<b>num_surcursal</b>, ciudad, activo)<br/>
Cliente (<b>DNI</b>, <b><ins>num_surcursal</ins></b>, nombre, apellidos, dirección, ciudad)<br/>
Cuenta (<b>num_cuenta</b>, <b><ins>num_surcursal</ins></b>, saldo)<br/>
Abrir (<b><ins>num_cuenta</ins></b>, <b><ins>DNI</ins></b>)<br/>
Transacción (<b>num_transacción</b>, <b><ins>num_cuenta</ins></b>, fecha, tipo_operación, cantidad)<br/>

## • Ejercicio 4<br/>

Parque_bomberos (<b>cod_parque</b>, nombre, dirección, teléfono, categoría)<br/>
Coche (<b>num_coche</b>, <b><ins>cod_parque</ins></b>, marca, modelo, num_matrícula, fecha_compra, fecha_ult_rev)<br/>
Bombero (<b>cod_bombero</b>, <ins>cod_parque</ins>, <ins>cod_turno</ins>, nombre, apellidos, fecha_nac, DNI, dirección, teléfono, puesto, <ins>cod_equipo</ins>)<br/>
Trabaja_en (<b><ins>cod_bombero</ins></b>, <b><ins>fecha_inicio</ins></b>, <b><ins>fecha_fin</ins></b>)<br/>
Turno (<b>cod_turno</b>, descripción)<br/>
Período (<b>fecha_inicio</b>, <b>fecha_fin</b>, <ins>cod_turno</ins>)<br/>
Petición_servicio (<b>cod_pet_serv</b>, tipo_serv, grado_urgencia, <ins>cod_equipo</ins>)<br/>
Recibe (<b><ins>cod_parque</ins></b>, <b><ins>cod_pet_serv</ins></b>, fecha, hora)<br/>
Equipo (<b>cod_equipo</b>, nombre)<br/>

## • Ejercicio 5<br/>

Préstamo (<b>num_préstamo</b>, fecha_prestamo, <ins>num_socio</ins>, <ins>signatura</ins>)<br/>
Socios (<b>num_socio</b>, nombre, apellidos, teléfono, fecha_cad)<br/>
Sanción (<b>num_días</b>, <ins>num_socio</ins>)<br/>
Préstamos_s (<b><ins>num_préstamo</ins></b>, tipo)<br/>
Préstamo_e (<b><ins>num_préstamo</ins></b>, fecha_devolución, tipo)<br/>
Libro (<b>signatura</b>, disponible, <ins>titulo</ins>, <ins>autor</ins>)<br/>
Fondo (<b>titulo</b>, <b>autor</b>, cantidad) <br/>

## • Ejercicio 6 <br/>

Cliente (<b>cod_cliente</b>)<br/>
Pedido (<b>cod_pedido</b>, fecha_pedido, <ins>cod_cliente</ins>, <ins>cod_producto</ins>, num_unidades)<br/>
Producto (<b>cod_producto</b>, cantidad, <ins>cod_proveedor</ins>, unidades, fecha_encargo)<br/>
Proveedor (<b>cod_proveedor</b>)<br/>

## • Ejercicio 7<br/>

Arrendatario (<b>CIF_NIF</b>, nombre_fiscal, nombre_firmante, carga_firmante, dirección, código postal, localidad, provincia, teléfono_fijo, teléfono_móvil, fax, actividad)<br/>
Nave (<b>código_nave</b>, polígono, calle, número, localidad, código_postal, provincia, teléfono, características, foto, datos_escritura, alquilada, gastos_comunidad, <ins>CIF_NIF</ins>, número_cuenta, días_pago, fecha_alquiler, fecha_fin_alquiler, importe_alquiler)<br/>
Recibo (<b>número_recibo</b>, importe_total, importe_IVA, pagado, fecha, <ins>código_nave</ins>, <ins>CIF_NIF</ins>)<br/>

## • Ejercicio 8<br/>

Piso (<b>puerta</b>, DNI, nombre, apellidos, dirección, código_postal, localidad, provincia, teléfono)<br/>
Cargo (<b>código_cargo</b>, nombre, funciones)<br/>
Ostenta(<b>código_cargo</b>, <b>puerta</b>, fecha_posesión)<br/>
Anotación (<b>código_anotación</b>, fecha, importe)<br/>
Ingreso_recibo (<b><ins>código_anotación</ins></b>, mes, pagado, puerta)<br/>
Ingreso_extra (<b><ins>código_anotación</ins></b>, concepto)<br/>
Gasto_fijo (<b><ins>código_anotación</ins></b>, fecha_inicio, fecha_fin, consumo, código_tipo_gasto)<br/>
Gasto_variable (<b><ins>código_anotación</ins></b>, fecha_facturación, concepto, número_factura)<br/>
Tipo_gasto_fijo (<b>código_tipo_gasto</b>, nombre, descripción)<br/>
Detalle_recibo (<b>número_línea</b>, concepto, importe, <b><ins>código_anotación</ins></b>)<br/>
