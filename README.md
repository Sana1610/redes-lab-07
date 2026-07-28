# Laboratorio 7 — Enrutamiento dinámico y transporte

**Autores:** Juan Esteban Ortiz Pastrana y Santiago Alberto Naranjo Abril  
**Institución:** Escuela Colombiana de Ingeniería Julio Garavito  
**Grupo:** 2  
**Fecha:** 18 de noviembre de 2023

## Introducción

Routers y switches dirigen el tráfico dentro de una infraestructura. Los routers toman decisiones de enrutamiento con base en las direcciones IP de destino; los switches conectan dispositivos dentro de redes locales.

## Marco teórico

El informe compara:

- **Enrutamiento estático:** las rutas son configuradas manualmente.
- **Enrutamiento dinámico:** los routers construyen y actualizan sus tablas según la topología.
- **Vector distancia:** calcula dirección y distancia y comunica cambios a los vecinos.
- **Estado de enlace:** mantiene información de la topología y calcula rutas.

También se estudian RIP, IGRP, EIGRP y OSPF, junto con sus métricas y mecanismos de actualización.

## Experimentación

### RIP y VLSM

Se realiza subnetting, se asignan direcciones a las LAN y se configuran routers. Mediante Telnet se accede de forma remota a los dispositivos para definir las redes participantes.

### EIGRP

La configuración anterior se reemplaza y se habilita EIGRP. Su métrica utiliza valores `K` o pesos que pueden ajustarse.

### OSPF

Se elimina la configuración de EIGRP y se habilita OSPF. La selección se basa en el costo, relacionado con el ancho de banda: un mayor ancho de banda produce un costo menor.

## Análisis de transporte

Con Wireshark se capturan y revisan:

- **UDP:** puertos de origen y destino, longitud, checksum y tamaño.
- **TCP:** puertos, número de secuencia, número de reconocimiento y longitud.

## Conclusiones

La experimentación muestra que el algoritmo de enrutamiento puede afectar la velocidad de transmisión y la estabilidad de la red. Por ello es necesario comprender el funcionamiento de cada protocolo y elegir el mecanismo más apropiado según la red.

## Contenido del repositorio

- Informe completo en DOCX y PDF.
- Topologías DHCP y EIGRP desarrolladas por Santiago Naranjo.
- Hoja de cálculo de subnetting.
