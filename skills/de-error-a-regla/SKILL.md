---
name: de-error-a-regla
description: Cuando algo sale mal con una IA (tiempo perdido, dinero gastado, trabajo rehecho), escribe la línea de las instrucciones en tres partes (qué pasó, la regla, cómo se comprueba) y se niega a dar por buena una regla sin forma de comprobarla. Úsala cuando el usuario cuente un fallo o diga "esto no puede volver a pasar", "apúntalo en las instrucciones", "hazme una regla" o "me ha costado X horas".
---

# De error a regla

Un error que no se convierte en una línea escrita vuelve a pasar. Una regla sin forma de comprobarla es un deseo. Esta skill hace las dos cosas: escribe la línea y exige la comprobación.

## Qué hacer

1. **Pregunta lo mínimo** si falta algo (en un solo mensaje): qué pasó exactamente, cuánto costó en tiempo o dinero, y cómo se detectó. Si ya lo ha contado, no lo repitas.
2. **Busca la causa, no el síntoma.** Pregúntate dónde nació el fallo, no dónde se vio. «El correo salió con el precio viejo» es el síntoma; «hay tres plantillas con precios copiados» es la causa. La regla va contra la causa.
3. **Redacta la regla** en una frase corta, en imperativo y con un criterio que se pueda cumplir o incumplir. «Revisa mejor» no es una regla; «nada sale sin que otro chat lo haya revisado» sí.
4. **Propón una comprobación concreta**: algo que se pueda hacer en menos de un minuto o que ocurra solo, y que falle visiblemente si la regla se rompe.
5. **Entrega la línea** en el formato de tres columnas, lista para pegar en el registro de las instrucciones del proyecto, con la fecha.

## Lo que NO haces

- **No das por buena una regla sin comprobación.** Si el usuario dice «la regla es que se tenga más cuidado», contestas que eso no se puede comprobar y propones tres alternativas que sí.
- No escribes reglas que valgan solo para el caso concreto («no uses el logo azul en el correo de Marta»). Sube a la clase: «los logos salen de una única carpeta».
- No inventas lo que pasó. Si hay un dato que no sabes (importe, fecha), lo dejas marcado como `[DATO]` y lo pides.

## Tipos de comprobación, de mejor a peor

1. **Automática**: un límite de gasto en la cuenta del servicio, una alerta, una validación que bloquea.
2. **Un paso fijo con prueba a la vista**: «antes de enviar, el borrador lleva un bloque con las dudas».
3. **Un revisor distinto**: otro chat, sin ver la explicación del autor, da el visto bueno.
4. **Una revisión periódica**: cada viernes, cinco minutos mirando X. Es la más débil: úsala solo si no hay otra.

Si la única opción es «acordarse», díselo claro: esa regla se romperá.

## Formato de salida

```
| Qué pasó | La regla | Cómo se comprueba |
|---|---|---|
| [hechos, con la cifra de lo que costó y la fecha: AAAA-MM-DD] | **[Regla en una frase.]** | [Comprobación concreta, de qué tipo es y quién la hace.] |
```

Después, una línea: «¿La añado a tus instrucciones como está, o la afinamos?»

## Ejemplo

**Usuario:** «Le pasé la IA a las 2.000 grabaciones de sesiones de dueños de perros de Pawly (una startup ficticia) sin mirar el coste y a fin de mes llegó una factura de uso que no esperábamos.»

| Qué pasó | La regla | Cómo se comprueba |
|---|---|---|
| [FECHA]: se analizaron 2.000 grabaciones de sesiones de dueños de perros con un servicio de pago sin estimar el coste y llegó una factura de uso inesperada de [IMPORTE]. | **Nada que gaste dinero sin mi OK y con el coste estimado delante.** | Antes de cada tarea de pago, la IA da una cifra estimada («unos 60 $, ilustrativo») y propone probar con 50 primero; espera mi «vale». Un límite de gasto en la cuenta del servicio avisa antes de que llegue la factura. |

Los datos que faltan (fecha, importe) los dejas como `[DATO]` y los pides.

## Huecos

Si el usuario describe un error que no encaja en el formato, dilo y propón cómo ampliarlo.
