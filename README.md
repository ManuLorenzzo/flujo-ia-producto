# Menos herramientas, más flujo

**El pack de la sesión de Lanzadera: instrucciones, brief y skills.**

Material de la sesión de Lanzadera (26 de noviembre de 2026) de Manu Lorenzo: cómo hace producto Mint con IA, y lo que nos costó aprenderlo. Lo que hay aquí es lo que usamos para que la IA no nos cueste tiempo ni dinero, contado con ejemplos de producto.

Versión visual: [manulorenzzo.github.io/flujo-ia-producto](https://manulorenzzo.github.io/flujo-ia-producto/)

Tiene tres partes: unas **instrucciones** para pegar en cualquier IA (valen en cualquier plan), un **brief** para encargar bien y **tres skills** para Claude.

## 1. Las instrucciones (empieza por aquí)

[`plantilla-instrucciones.md`](plantilla-instrucciones.md): las instrucciones del proyecto, lo que la IA lee antes de cada tarea. Se pegan en un Proyecto de Claude, ChatGPT o Gemini. Traen un registro de reglas con seis reglas reales de Mint ya rellenas (qué pasó, la regla, cómo se comprueba) y una tabla vacía para las tuyas.

Cada vez que la IA te cueste tiempo o dinero, añade una fila. Sin forma de comprobarla, no es regla.

Ejemplos de antes y después de cada regla, con una sola historia (el registro de Pawly, una startup ficticia): [`ejemplos.md`](ejemplos.md).

## 2. Las tres skills

| Skill | Para qué sirve | Cómo pedírselo |
|---|---|---|
| **escribir-brief** | Convierte una petición vaga en un brief (lo dudoso arriba, el problema de fondo, qué hay que hacer en pasos, lo que no se hace y cómo sabremos que funciona) y pregunta lo que falta antes de empezar. | «Escríbeme el brief de este encargo: [lo que quieres]» |
| **revisor-desconfiado** | Revisa un resultado sin fiarse de la explicación de quien lo hizo y busca las siete tentaciones. Termina con veredicto: vale, vale con cambios o no vale. | «Revisa esto sin fiarte de lo que dice el autor» (y pegas el resultado) |
| **de-error-a-regla** | Cuando algo sale mal, escribe la línea de las instrucciones y no la da por buena sin una comprobación concreta. | «Esto ha salido mal: [qué pasó]. Hazme la regla.» |

### Cómo instalar una skill

1. Descarga el ZIP desde la carpeta [`zips/`](zips/). No hace falta descomprimirlo.
2. En Claude, ve a **Personalizar > Skills**, pulsa **+** y sube el ZIP.
3. Comprueba que aparece en la lista y está **activada**.

> Si en tu app los menús se llaman distinto, busca **Skills** dentro de **Personalizar**.
>
> **Si la skill no aparece en tu plan, usa la plantilla en texto**, que funciona en cualquiera. Las tres skills también se pueden pegar tal cual (el contenido de `SKILL.md`) en las instrucciones de un Proyecto.

Las tres skills son solo texto, sin código: puedes leerlas en [`skills/`](skills/) antes de instalarlas. Hazlo siempre con cualquier skill que te llegue de fuera.

## Aviso

Mint sale aquí como ejemplo de dónde salieron las reglas, no como producto. Las reglas son tuyas para copiar y cambiar.

## Licencia y autoría

Creado por Manu Lorenzo. Licencia [MIT](LICENSE): úsalo, cópialo y adáptalo a tu empresa libremente.
