Problema VRPSPDTW con Mochila y Carga Heterogénea. 

Integrantes: Maximiliano Bravo, Max Fernández, Jorge Travieso. 

 

Base Logística: Problema de Ruteo de Vehículos 

Este problema es una variación compleja del Problema de Ruteo de Vehículos clásico (VRP). Este consiste en diseñar un conjunto de rutas óptimas para una flota de vehículos homogéneos que parten desde un único depósito central con el fin de satisfacer las demandas de un conjunto de clientes dispersos geográficamente, para luego regresar al mismo depósito. 

El objetivo primordial es minimizar los costos de la operación, los cuales suelen traducirse en la distancia total recorrida, el tiempo de viaje o la cantidad de vehículos utilizados. 

La restricción base indica que cada cliente debe ser visitado exactamente una vez por un único vehículo, y ningún vehículo puede exceder su capacidad máxima de carga. 

 

Core del Negocio: Selección Estratégica (Componente de la Mochila) 

Sobre este problema, en el cual es obligatorio visitar a todos los clientes, el componente de la mochila rompe esa regla cuando los recursos son insuficientes. Cada cliente ofrece un beneficio económico si es atendido, pero consume espacio de transporte. El problema debe decidir a qué clientes aceptar y cuáles rechazar para maximizar la ganancia neta (equivalente a los ingresos menos los costos de transporte del VRP). 

 

Flujo Bidireccional: Recogida y Entrega Simultánea (SPD) 

En el VRP clásico, el camión sólo entrega mercancía y se va vaciando. Al añadir Simultaneous Pickup and Delivery (SPD), cada parada exige dos acciones a la vez: descargar mercancía (delivery) y cargar devoluciones o nuevos productos (pickup). Con esto, el inventario a bordo fluctúa dinámicamente en cada tramo de la ruta. 

 

Dimensión Temporal: Ventanas de Tiempo (TW) 

A la planificación de las rutas del VRP se le impone un horario de atención rígido para cada cliente mediante un intervalo de tiempo [ei,li]. El vehículo debe llegar dentro de ese margen, puesto que llegar antes implica un desperdicio de tiempo, y llegar tarde invalida la ruta. 

 

La Geometría de la Carga: Heterogeneidad 

Con este agregado, la capacidad del vehículo ya no es un número simple o una unidad estándar, tales como kilos o cajas. Ahora, la carga se compone de objetos con diferentes formas, longitudes, anchos, alturas y pesos, convirtiendo el espacio disponible del camión en un entorno físico tridimensional real. 

 

El Rompecabezas Operativo: Restricciones de Estiba y Accesibilidad 

Finalmente, la mezcla del VRP, la carga heterogénea y el flujo bidireccional exige reglas físicas en el camión: restricciones LIFO (Last-In, First-Out) para que la carga recogida no bloquee las entregas pendientes, límites de apilamiento por fragilidad, y distribución equilibrada de peso por ejes para la seguridad del vehículo en ruta. 

 

En resumen, el problema describe una extensión del VRP clásico. Donde antes sólo se buscaba la ruta más corta para una flota, ahora se buscan los clientes más rentables primero (Mochila), diseñando trayectos que cumplan horarios estrictos (Ventanas de Tiempo), mientras se gestiona un espacio tridimensional dinámico que se llena y vacía en cada parada (Recogida y Entrega) con paquetes de múltiples formas y pesos (Carga Heterogénea). 