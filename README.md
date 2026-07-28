# Laboratorio 7 — Enrutamiento dinámico y análisis de transporte

Trabajo de **Juan Esteban Ortiz Pastrana** y **Santiago Alberto Naranjo Abril**, presentado en la Escuela Colombiana de Ingeniería Julio Garavito el 18 de noviembre de 2023.

## Descripción

El laboratorio estudia el papel de routers y switches en una infraestructura de red, con énfasis en la selección dinámica de rutas y en el análisis de tráfico de transporte.

## Temas abordados

- Enrutamiento estático y dinámico.
- Protocolos de vector distancia y estado de enlace.
- RIP, IGRP, EIGRP y OSPF.
- Subnetting y VLSM.
- Tablas de enrutamiento y configuración remota mediante Telnet.
- Métricas basadas en saltos, pesos y costo.
- Captura y revisión de UDP y TCP con Wireshark.

## Desarrollo

Se configuraron topologías en Packet Tracer para probar distintos mecanismos de enrutamiento. La configuración de EIGRP reemplazó la de RIP y utilizó pesos para calcular la métrica. Posteriormente se configuró OSPF, cuya selección de ruta se relacionó con el costo y el ancho de banda.

Con Wireshark se revisaron campos de UDP y TCP, entre ellos puertos, longitud, checksum, números de secuencia y reconocimiento.

## Conclusiones

Los algoritmos de enrutamiento influyen en la velocidad, estabilidad y administración de una red. La elección del mecanismo depende de la topología y de las necesidades de comunicación.

> Este README fue elaborado exclusivamente a partir del informe `Laboratorio7.docx`.
