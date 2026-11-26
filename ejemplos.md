# Ejemplos: así se nota la diferencia

*Ejemplos ilustrativos, escritos para enseñar la diferencia.* *Pawly es una startup ficticia: el caso que seguimos en la sesión.* Es un marketplace de paseadores y cuidadores para dueños de perros en España, donde 9 de cada 20 dueños abandonan en el registro. Es una sola historia y los datos y las cifras son inventados. Un caso por cada una de las reglas que [`prompt-instrucciones.md`](prompt-instrucciones.md) mete en tus instrucciones.

---

## 1. Pregunta a ciegas, compara tú después

**Antes**

> Aquí tienes 20 entrevistas con dueños de perros. Creo que el problema es el precio, ¿lo confirmas?

**La IA responde**

> Sí, el precio aparece como la preocupación principal en varias entrevistas. Te recomiendo revisar la estructura de planes.

**Después**

> Agrupa los problemas por frecuencia y cita la frase literal de cada uno. No te digo lo que creo.

**La IA responde**

> 1. Piden demasiados datos del perro de entrada (11 de 20): «me pedían hasta el microchip». 2. Precio (4 de 20): «no sé si me compensa». 3. Falta de integraciones (3 de 20)...

**Qué cambia:** si le dices lo que crees, te lo confirma. Si no, te enseña lo que de verdad dicen tus dueños de perros: el problema no era el precio, era pedir demasiado del perro nada más entrar.

---

## 2. Brief

**Antes**

> Hazme una pantalla de registro para Pawly.

**La IA responde**

> Te he preparado el registro con login social (Google y Apple), reglas de contraseña con indicador de seguridad y, ya que estaba, un rediseño del resto de la app para que sea coherente.

**Después** (con el brief)

> **Lo dudoso, arriba:** ¿pedimos el teléfono ya? Sin decidir.
> **Qué hay que hacer, en 3 pasos:** 1. Email y nombre. 2. Los datos del perro, después. 3. Ver dónde se van.
> **Lo que NO se hace:** ni login con Google, ni tocar pagos.
> **Cómo sabremos que funciona:** abandonan menos de 5 de cada 20.

**La IA responde**

> Te propongo el plan en tres pasos y espero tu OK. Antes, la duda que dejaste abierta: ¿el teléfono lo pedimos ya o al reservar el primer paseo? Propongo al reservar, para no frenar el registro. Al acabar, mediré cuántos de cada 20 abandonan.

**Qué cambia:** de tres cosas que no pediste, a la que necesitabas, con la única duda real encima de la mesa y una forma de saber si ha funcionado.

---

## 3. Si necesitas una excepción para un caso, para

**Antes**

> Que el formulario valide el código postal.

Lo prueban con un código postal de Valencia (46001).

> **La IA:** Hecho.

Con el siguiente dueño falla: vive en Canarias y su código postal empieza por 35.

**Después** (con la regla en las instrucciones)

> **La IA:** Para que pase tu ejemplo tendría que validar solo los códigos que empiezan como el de Valencia. Pawly opera en toda España, también Baleares, Canarias, Ceuta y Melilla: ¿qué zonas atendemos de verdad? Paro y te pregunto.

**Qué cambia:** en vez de programar para el ejemplo que le diste, se detiene y te pregunta dónde está de verdad tu cliente.

---

## 4. No te fíes del informe del autor

**Antes** (un solo chat hace y se revisa)

> **Chat 1:** Listo. Solo he tocado el registro de Pawly.

**Después** (otro chat revisa, sin leer esa frase)

> **Tú al chat 2:** Revisa estos cambios. Dime qué se ha modificado y qué no debería. [pegas solo los cambios]
> **Chat 2:** También ha cambiado el texto del botón de pago y ha quitado la validación del email.

**Qué cambia:** «solo he tocado el registro» era el informe del autor. Al revisor solo le llegaba el trabajo, y vio dos cosas que nadie había pedido.

---

## 5. Nada que gaste dinero sin mi OK

**Antes**

> Pásale la IA a las 2.000 grabaciones de sesiones de dueños de perros en Pawly.

La IA las procesa todas. A fin de mes llega una factura de uso que nadie esperaba.

**Después**

> **La IA:** Esto costará unos 60 $ estimados (2.000 grabaciones; cifra ilustrativa). ¿Sigo, o lo pruebo con 50 primero y te digo el coste real?

**Qué cambia:** el gasto se decide antes, con una cifra delante, y no después en forma de sorpresa.

---

## 6. Lo dudoso, arriba

**Antes**

> Analiza la conversión del registro de Pawly de las últimas dos semanas.

La IA entrega tres páginas. Faltaban los datos de la semana pasada y los rellenó con una estimación, que aparece en el párrafo siete como un dato más.

**Después**

> **La IA:** **Dudas, primero.** Faltan los datos del martes; los he estimado con la media. La conversión real podría ser distinta. Lo demás sale de los datos que me diste.
> [después, el análisis]

**Qué cambia:** el mismo análisis, pero lo que no está comprobado se ve en la primera línea y no en el párrafo siete.
