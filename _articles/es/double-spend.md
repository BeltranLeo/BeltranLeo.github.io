---
layout: es/post
title: ¿Qué es un doble gasto y cómo Bitcoin Cash lo evita?
author: Leo Beltran
date: 13-01-2023
image: generic.jpg
lead:
categories: uncategorized
id: double-spend
---

Se conoce como **doble gasto** al pago de un bien o servicio utilizando dos veces la misma moneda.

En el mundo del dinero fíat, un doble gasto se realiza cuando una transacción digital, como transferencia, tarjeta de crédito, aplicaciones de pago, etc., es revertida y el dinero devuelto.

En términos de Bitcoin Cash, esto sería utilizar más de una vez el mismo UTXO (‘salida no gastada de transacción’) para realizar un pago.

Dado que, según las reglas de consenso de Bitcoin Cash, si existen dos transacciones conflictivas solo una puede ser aceptada como válida, intentar realizar un doble gasto es una forma de estafar o perjudicar al legítimo receptor de esas monedas.


## Soluciones de Bitcoin Cash

Actualmente, la capacidad de un usuario de realizar con éxito un doble gasto es extremadamente baja e improbable. Existen múltiples mitigaciones implementadas en la cadena de bloques y en los nodos para que esto no ocurra.

En primer lugar, las reglas de consenso prohíbe la existencia de dos transacciones conflictivas, es decir, contradictorias. Esto significa que no puede haber una transacción esté gastando una moneda (llamado también _output_) que haya sido gastado en una transacción previa.

Por otro lado, en la actualización de Bitcoin Cash de 2021 fueron incorporadas las **DS Proofs**, que permiten detectar y probar criptográficamente un intento de doble gasto por un usuario antes de que las transacciones sean incluídas en un bloque.
