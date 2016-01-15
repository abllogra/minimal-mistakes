---
layout: post
title: El Éxito De Mi Aplicación en El Mercado Negro
author: abel_llopis
modified:
categories:
excerpt:
tags: []
image:
  feature:
date: 2014-11-19T10:21:53+01:00
---

Hace un par de meses publiqué [Drocks](https://itunes.apple.com/es/app/drocks/id916689478?mt=8), un juego de habilidad en el que iban cayendo bloques y debías de cambiar rápidamente la base para que su color coincidiera con el color de los bloques.


La finalidad de la publicación del juego no era hacerme rico aunque sí ver un poco recompensado el tiempo dedicado al desarrollo del juego y el orgullo de poder decir, he publicado un juego propio en la App Store.


Durante 2 meses el juego ha estado (sigue estando) en la App Store y a día de hoy he tenido un total de 37 descargas. Lo que me ha reportado unos ingresos de 18 dólares que al cambio con impuestos y demás tasas me han ingresado en el banco un total de 9 euros.


La mayoría de esas 37 compras han sido por familiares, amigos, compañeros y seguidores de Twitter. No es que sean muchas pero ya son más de las que me esperaba sin haber invertido dinero en campañas de publicidad, solamente una [página en Facebook](https://www.facebook.com/drocksgame) y una [cuenta de Twitter](https://twitter.com/drocks_app) haciendo spam a mis seguidores.


Una de las cosas que me llamó la atención tras la publicación del juego es que no había pasado ni 2 días y ya había webs que ofrecían mi juego para descargar gratuitamente.


Las estadísticas de descargas en la plataforma de Apple no son en “vivo”, tardan un día o dos en actualizarse y mi referencia era el número de jugadores que aparecían en Game Center.


Al principio no había casi jugadores pero conforme iban pasando los días crecían de una media de 10 a 20 jugadores diarios. Qué alegría ver cómo crece el número de jugadores y  piensas que tu juego está teniendo éxito.


Cuando te detienes unos segundos y analizas las cifras, te das cuenta que tienes un total de 258 jugadores en Game Center que juegan o han jugado a [Drocks](https://itunes.apple.com/es/app/drocks/id916689478?mt=8) pero sólo 37 jugadores han pagado por él. Partiendo de la base que todos los que se han descargado el juego, ya sea de forma legal o ilegal, tienen activada su cuenta de Game Center, hay un mínimo de 221 jugadores que se han descargado el juego de forma ilegal, esto supone que al menos el 85% de los jugadores de [Drocks](https://itunes.apple.com/es/app/drocks/id916689478?mt=8) tienen el famoso jailbreak y han pirateado mi juego.


#### Llegados a este punto, ¿qué podemos hacer los desarrolladores?


He estado investigando si hay alguna forma de evitar que tu app se pueda instalar en dispositivos con jailbreak y es imposible controlarlo. Cuando se instala una app en un dispositivo con jailbreak no se puede controlar si se está instalando en un dispositivo “limpio” o no. Así que investigué si se podía saber si mi app está ejecutándose en un dispositivo pirata,  en este sentido hay más información.


No hay una forma 100% fiable de controlar que tu app no haya sido comprada y se esté ejecutando en un dispositivo con jailbreak pero podemos añadir algunas comprobaciones para detectar que tienen una copia pirata de nuestra app. Para detectarlo podemos hacer varias comprobaciones:


- Comprobar si la app Cydia está instalada en el dispositivo. Si existe el path /Applications/Cydia.app
- Comprobar si es posible el acceso al path /bin/bash, en caso afirmativo, el dispositivo tiene jailbreak.


Existen más formas para intentar detectar el jailbreak, para más información podéis consultar este enlace.


¿Qué hacemos una vez sabemos que tiene jailbreak? Este tema ya va a gustos del programador, en mi caso yo estaba entre 2 opciones:

- **1ª opción:** Evitar que los jugadores pudieran hacer más de un par de puntos e indicarles que han pirateado mi juego con un gracioso mensaje.
- **2ª opción:**  Añadir Admob sólo a los jugadores con jailbreak, con ello podría obtener algún beneficio con los piratearon mi juego.

Al final he optado por la segunda opción, estoy actualizando mi juego para añadir publicidad al iniciar el juego y al reiniciar una partida, obligatoriamente deberán visualizar un video para poder continuar. Con este tema me ha surgido otra duda ¿Existe alguna forma de “ocultar” Admob con jailbreak? Y la respuesta es afirmativa, existen herramientas para que no se visualice la publicidad. De todas formas, voy a probar con esta opción y en unas semanas sabré los resultados.

#### ¿Qué pasaría con los usuarios que tienen el dispositivo con jailbreak y las apps compradas?

Seguramente no haya ninguna persona que tenga su dispositivo con jailbreak y decida comprar una aplicación si la puede tener gratis. Pero confiemos en la buena fé de las personas. Si realizamos alguna acción si el dispositivo tiene jailbreak no podremos saber si compró o no la app por lo tanto, también les afectaría. Tendrá una versión legal de mi juego pero se ejecutaría como si fuera pirata ya que su dispositivo tiene jailbreak.

Un “truco” que los desarrolladores podemos utilizar para obligar a que la descarga sea legal es publicar las apps gratuitamente e incluir compras dentro de la aplicación. Para ello tenemos que limitar las características de la aplicación y ofrecer extras o nuevas características en forma de compra. Esta opción tiene un riesgo, si no consigues enganchar al usuario posiblemente no obtengas la compra. Hay que verlo cómo un reto, conseguir que al usuario le guste tu app y decida comprar la versión completa o las características nuevas que ofreces.

#### ¿Qué diferencias hay entre publicar una app de pago y una app gratis con compras?

En una app que contiene compras en su interior a través de la App Store, cuando el usuario realiza la compra, el desarrollador puede validar si la información recibida es válida y así evitar que los dispositivos con jailbreak puedan obtener las compras gratuitamente y disfrutar de la versión completa. En la documentación de Apple está detallado cómo debe realizarse.

#### ¿Apple? ¿Estás ahí?

Para finalizar, Apple debería poner mecanismos para que no se pudieran instalar/ejecutar tus aplicaciones en un dispositivo con jailbreak o al menos para intentar detectar si el dispositivo ha sido modificado. En este sentido los desarrolladores estamos desprotegidos, debemos pagar una cuota para poder desarrollar nuestras apps y publicarlas en la App Store.  Cuando desarrollas una app debe pasar unos “controles de calidad” y cumplir ciertos requisitos para que sea aprobada y que los usuarios se la puedan descargar. ¿Podemos exigir algo a cambio?

Lo que me queda de esta experiencia es que al menos en el “mercado negro” mi juego gusta y es una sensación contradictoria, alegría y decepción.
