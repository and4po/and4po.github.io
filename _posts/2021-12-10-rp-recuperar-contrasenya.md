---
layout: single
title: Recuperar la contrasenya de la teva Raspberry Pi
excerpt: "Se t'ha oblidat algun cop la contrasenya de la teva Raspberry Pi? A mi sí. Doncs aquí t'explico com recuperar-la pas a pas."
date: 2021-12-10
classes: wide
header:
  teaser: /assets/images/Passwd-RSPI/Icona.png
  teaser_home_page: true
  icon:
categories:
  - Raspberry Pi
  - Contrasenya
tags:  
  - RaspberryPi
  - Linux
---

Això serà possible gràcies a que el sistema operatiu Raspberry OS està instal·lat en una targeta Micro SD, els fitxers de la qual podem modificar per a recuperar la contrasenya.

Primer, hem de treure la targeta Micro SD de la nostra Raspberry Pi i amb un adaptador posar-la al nostre ordinador Windows, Mac o Linux. Després, hem d'obrir el fitxer _cmdline.txt_ amb qualsevol editor de textos i al final, escriure-hi el següent text `init=/bin/sh`.

![screen](/assets/images/Passwd-RSPI/IMG-1.png)

Seguidament, desarem els canvis i expulsarem la targeta Micro SD de l’ordinador i la tornarem a posar a la Raspberry Pi. En tornar a encendre la nostra Raspberry Pi ens apareixerà un cursor parpellejant, haurem d’escriure `passwd pi`. (Si no veus cap canvi a la pantalla, no passa res, per defecte les contrasenyes no es previsualitzen). Després, escriure-hi la nova contrasenya i pressionar Enter dues vegades. Només haurem d’executar el següent text: `sync exec /sbin/init`.
Veurem que la Raspberry Pi es reinicia. Quan hagi acabat l’apagarem, expulsarem la targeta i al nostre ordinador esborrarem el text que hem escrit abans (`init=/bin/sh`). 

I en tornar a inserir la targeta al petit ordinador ja tornarà a funcionar perfectament!

Si vols saber el perquè de tot el que hem fet clica [aquest](example.com) enllaç.
