---
layout: es/post
title: CashAddr, el formato de direcciones de Bitcoin Cash
author: Leo Beltran
date: 2023-01-01
image: generic.jpg
lead:
categories: uncategorized
id:
---

Cuando se desea recibir o enviar un pago utilizando Bitcoin Cash, se utilizan direcciones. La forma en la que se representa esta información se denomina **formato de direcciones**.

**CashAddr** es el formato de direcciones propio de Bitcoin Cash. Fue introducido luego de la actualización de 2017 y se ha convertido en el formato mayoritario adoptado por billeteras, usuarios y plataformas.

Antes de utilizarse el formato CashAddr, se utilizaba el formato **Legacy** —también conocido como **Base58**—, que ya cayó en desuso y solamente es soportado en forma de retrocompatibilidad.

---

**Nota:** Lo que hay que entender es que, al ser un formato diferente, no cambia la dirección, sino la forma de mostrarlo. Es decir que una misma dirección puede representarse como Legacy o CashAddr. Es similar a representar el mismo número en forma decimal («48») o en números romanos («XLVIII»). No cambia el número, solo su formato de representación.

---

Cuando se utiliza CashAddr, por defecto en Bitcoin Cash, las direcciones lucen de esta manera: `bitcoincash:qrxxrefrrup9xwct4j8msyn3yy3m2ks6nut6u0jv5g`

Mientras que la **misma** dirección en formato Legacy se ve así: `1Kdg817SuWmjMVpytvuXewFq9VcQGE9b9j`

Ambas direcciones representan la misma clave pública. Simplemente se muestran de manera diferente.

## Ventajas de CashAddr

Las principales diferencias de las direcciones CashAddr con las Legacy son:

-   Por defecto se incluye el prefijo `bitcoincash:`, aunque es opcional.
-   Solo se utilizan letras minúsculas. Se pueden representar también con letras mayúsculas.
-   Se pueden representar más eficientemente en códigos QR usando el modo alfanumérico.
-   Son exclusivas de Bitcoin Cash, por lo que no hay riesgo de confusión con otras criptomonedas a la hora de hacer un pago.

## Convertir de CashAddr a Legacy y viceversa

La billetera **Electron Cash** permite convertir una dirección CashAddr a Legacy y viceversa, en caso de que algún servicio que se utilice por alguna razón no lo soporte.

También las siguientes páginas web ofrecen una herramienta de conversión en línea:

-   https://cashaddr.bitcoincash.org/
-   https://cashaddr.org/

Sin embargo, es recomendable no utilizar servicios o plataformas que no utilicen CashAddr, ya que, al ser una actualización tan básica y adoptada en la red de Bitcoin Cash, cualquier sistema que no las utilice da la impresión de estar extremadamente desactualizado.
