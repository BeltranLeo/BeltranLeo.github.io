---
layout: es/post
title: Qué es CashFusion y cómo usarlo en Bitcoin Cash
author: Leo Beltran
date: 12-01-2023
image: generic.jpg
lead:
categories: privacy
id: cashfusion
---

**CashFusion** es una tecnología presente en Bitcoin Cash que permite obtener y mejorar la privacidad y el anonimato. Es una implementación de **CoinJoin**, que es un sistema por el cual dos o más usuarios realizan una transacción conjunta, agregando sus monedas en un pozo común y luego retirándolas sin que los demás participantes sepan qué monedas corresponden a quién.

## ¿Por qué se necesita CashFusion?

Como la cadena de bloques de Bitcoin Cash es pública, el registro de todas las transacciones realizadas por los usuarios queda registrado. Empresas como **Chainalysis** se dedican a estudiar el tráfico de la red y tratar de combinar metadatos para identificar las monedas que pertenecen a determinados usuarios.

Con CashFusion no solo se vuelve exponencialmente más caro, sino que es virtualmente imposible descomponer una transacción realizada con esta tecnología para identificar a los usuarios.

## Ventajas

-   **Mejora la resistencia a la censura.** CashFusion es una herramienta efectiva para evadir controles, regulaciones y listas negras.
-   **Es autocustodial.** CashFusion funciona de forma que no se requiere dar acceso a los bitcoins a ningún tercero. El usuario mantiene en todo momento control de sus fondos.
-   **No tiene comisión.** En otras cadenas de bloque, los protocolos de privacidad cobran a los usuarios una tarifa extra para ser utilizados. Con CashFusion solamente se paga la tarifa de la red.

## ¿Cómo funciona CashFusion?

Una transacción tradicional de Bitcoin Cash puede verse de la siguiente manera:

```
Inputs | Outputs
-------+--------
2 BCH  | 2.5 BCH
1 BCH  | 0.5 BCH
```

Es casi seguro que se trata de un usuario haciendo un pago por el equivalente a 2.5 BCH, ya que si fuera 0.5 no haría falta uno de los _inputs_. Por este motivo, podemos estar casi seguros de que ambas direcciones de _input_ y el _output_ de 0.5 BCH pertecenen al mismo individuo.

Para que esto no ocurra, se puede introducir confusión en la transacción.

```
Inputs | Outputs
-------+--------
2 BCH  | 2.5 BCH
1 BCH  | 0.5 BCH
```

---

El protocolo de funcionamiento de CashFusion es el siguiente:

1. El usuario se conecta a un servidor de CashFusion y se registra en una lista pública para anunciar el tamaño de las monedas que desea mezclar. Este servidor está encargado de coordinar la transacción entre los diferentes participantes.
2. El servidor y los diferentes participantes aguardan hasta que haya suficientes personas esperando para hacer una fusión.
3. La fusión inicia. Cada uno de los participantes envía información al servidor, pero de una manera en la cual no es posible saber qué monedas pertenecen a quién, garantizando la privacidad.
4. Cada usuario selecciona nuevas direcciones para recibir los bitcoins fusionados. La idea es utilizar direcciones que no hayan sido vistas anteriormente en la red.

## ¿Cómo utilizar CashFusion?

La forma más simple es descargar la versión de escritorio de la billetera **Electron Cash**.

## Enlaces externos

-   Página oficial de CashFusion: https://cashfusion.org/
-   Enlace a la billetera Electron Cash, con soporte para CashFusion: https://electroncash.org/
