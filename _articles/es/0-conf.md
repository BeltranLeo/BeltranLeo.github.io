---
layout: es/post
title: ¿Qué es 0-conf?
author: Leo Beltran
date: 12-01-2023
image: instant-payment.jpg
lead:
categories:
id: 0-conf
---

**0-conf** es una capa de utilidad existente en Bitcoin Cash que permite aceptar transacciones sin confirmaciones, lo que facilita los pagos y da una experiencia cómoda e instantánea.

Cuando una persona utiliza Bitcoin Cash para pagar por un bien o servicio, sobre todo en persona, la transacción puede demorar hasta diez minutos en ser incluida en un bloque. A esto se lo denomina **confirmación**. Por ejemplo, una transacción que fue incluida en el último bloque generado, tiene _una confirmación_. Una que fue incluida hace tres bloques tiene _tres confirmaciones_.

A medida que una transacción obtiene confirmaciones, la posibilidad de que esta sea revertida disminuye considerablemente, haciendo que algunos servicios, como _exchanges_, exijan un determinado número de confirmaciones antes de acreditar el balance.

Sin embargo, esto no significa que si alguien paga por un café tiene que estar esperando en el local hasta que el pago se haya confirmado. 0-conf le da mayor seguridad al comerciante de que el pago no puede ser revertido y que será incluido en el próximo bloque.

Además, el comerciante puede hacer uso de los BCH recibidos de forma instantánea (también usando 0-conf), logrando que no tenga que esperar una confirmación para poder usarlo. Tal cual el dinero en efectivo, solo que en forma digital.

Aún así, cabe resaltar que un comerciante puede decidir no aceptar transacciones sin confirmaciones, dependiendo del tipo de producto o servicio que ofrezca. Es completamente voluntario.

## Cómo funciona 0-conf

Los usuarios, al hacer una transacción utilizando una billetera, construyen una transacción y la firman con las claves privadas correspondientes a las monedas de Bitcoin Cash que están intentando gastar. Esta transacción es comunicada vía internet a los nodos y a los mineros que mantienen la seguridad de la red. Los mineros chequean que la transacción sea válida (cumpliendo con las reglas de consenso) y la agregan a la **_mempool_**, que es el espacio en memoria donde aguardan las transacciones para ser incluidas en un bloque futuro.

Si un usuario malicioso, en un intento de estafar a un comerciante, envía una nueva transacción gastando las mismas monedas, esta será rechazada por la mayoría de los nodos, que están configurados para no aceptar transacciones que intenten gastar monedas no válidas o aquellas que ya estén incluidas dentro de la **_mempool_**.

Por este motivo, dado que el incentivo de los mineros honestos es incluir la mayor cantidad de transacciones en la cadena de bloques para cobrar las tarifas que estas pagan, lo más probable es que las nuevas transacciones sin confirmación sean incluidas en el próximo bloque hallado.  

## Seguridad

La seguridad de 0-conf se basa en el sistema de seguridad de Bitcoin Cash y es ampliamente utilizada por la gran mayoría de las herramientas del ecosistema. El funcionamiento es simple y **no requiere configuración por parte del usuario.**

Además, en la actualización de mayo de 2021, se incluyó un sistema de seguridad conocido como DSProofs, que permite generar y propagar por toda la red una prueba criptográfica de doble gasto, permitiendo identificar más fácilmente un intento de doble gasto en una transacción fraudulenta.

Por otro lado, la seguridad provista por 0-conf es variable. Es natural pensar que para un café o una hamburguesa un comerciante que acepte Bitcoin Cash decidirá no esperar una confirmación, aceptando transacciones tan pronto como su sistema de pagos las detecte. Un auto o una casa requerirá confirmaciones, pero hay suficiente traspaso de tiempo como para que esto no sea un problema.
