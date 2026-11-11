# Tarea: Mi prompt profesional

## Funcionalidad elegida
CRUD (Crear, Leer, Actualizar, Eliminar) básico para el registro y gestión de mantenimiento de maquinaria pesada (excavadoras y camiones mineros).

## Version 1: prompt basico
```text
Crea un sistema en Java para guardar excavadoras y camiones mineros.
```
**Qué cambié y qué mejoró:** Faltaba contexto y formato. La IA generó un código enorme, desordenado y con clases innecesarias. Para la versión 2, agregaré el rol y le pediré que no use bases de datos.

## Version 2
```text
Actua como desarrollador de software. Haz un CRUD en Java para guardar maquinaria pesada (excavadoras y camiones mineros). Usa una clase Maquinaria. No uses base de datos.
```

## Version 3: Prompt final
```text
Actua como ingeniero de software senior. Desarrolla un CRUD basico en Java para gestionar el mantenimiento de maquinaria pesada en una mina a tajo abierto. 
El sistema debe manejar una clase 'Maquinaria' con los atributos: id, tipo_vehiculo, estado_operativo y horas_uso. 
Ejemplo de metodos esperados: getHorasUso(), setHorasUso(int horas). 
No uses librerias externas, utiliza solo un ArrayList para almacenar en memoria. 
Formato: Presenta el codigo de la clase primero, seguido de un metodo main corto para probarlo.
```
