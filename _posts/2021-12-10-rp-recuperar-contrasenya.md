---
layout: single
title: Recuperar la contraseña de la teva Raspberry Pi
excerpt: "Se t'ha oblidat algun cop la contraseña de la teva Raspberry Pi? A mi sí. Doncs aquí t'explico com recuperar-la pas a pas."
date: 2021-12-10
classes: wide
header:
  teaser: /assets/images/Passwd-RSPI.png
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

Primer, hem de treure la targeta Micro SD del nostre ordinador i amb un adaptador posar-la al nostre ordinador Windows, Mac o Linux. Després hem d'obrir el fitxer _cmdline.txt_ amb qualsevol editor de textos i escriure-hi al final el següent text `init=/bin/sh`.

<! --- Imatge
