# El prompt que te escribe las instrucciones

Las instrucciones son lo que la IA lee antes de cada tarea. No las rellenes a mano: pega este prompt y deja que ella te pregunte y te las escriba.

**Cómo se usa**
1. Abre un chat nuevo en tu IA (Claude, ChatGPT, Gemini…) y pega el prompt de abajo.
2. Contesta sus preguntas. Si no sabes algo, díselo: lo dejará marcado como dudoso.
3. Pega lo que te devuelva en las instrucciones fijas de tu proyecto (en Claude y ChatGPT, un Proyecto). Si usas Claude Code u otro agente, en `CLAUDE.md` o `AGENTS.md`.
4. Cada vez que la IA te cueste tiempo o dinero, vuelve a ese chat: «Ha pasado esto: [qué pasó]. Añade la regla, con cómo se comprueba.»

Las reglas que trae salieron de errores reales en Mint. Los ejemplos, con el caso de Pawly, en [`ejemplos.md`](ejemplos.md).

---

```text
Quiero que me ayudes a escribir las instrucciones fijas de mi proyecto de producto: el texto que vas a leer antes de cada tarea. Todavía no las escribas.

PASO 1 · PREGÚNTAME
Hazme preguntas en bloques de tres como mucho, cada una con tu recomendación, para que pueda contestar rápido. Necesitas saber:
- Quién soy y qué papel tengo.
- El producto: qué hace, para quién y en qué fase está.
- El usuario: quién es y qué le duele.
- La métrica que importa ahora mismo.
- Lo que ya existe y lo que no se toca.
- Las herramientas que uso a diario, y en cuáles puedes escribir y en cuáles solo leer.
- Cómo quiero que me entregues (extensión, formato, idioma).
- Qué me ha salido mal con la IA hasta ahora.
Si no sé algo, márcalo como dudoso y sigue.

PASO 2 · ESCRÍBELAS
Cuando tengas suficiente, escribe las instrucciones con estas partes. En imperativo, dirigidas a ti, y cada regla con su porqué en una línea.
1. Mi producto: cinco líneas como mucho.
2. Cómo trabajamos un cambio:
   - Descubrir: pregunta a ciegas. Si te digo lo que creo, no lo confirmes: responde primero y con citas literales.
   - Definir: antes de hacer nada, un brief con lo dudoso arriba, qué hay que hacer en pasos, lo que no se hace y cómo sabremos que funciona. Espera mi OK.
   - Construir: primero el plan en pasos pequeños; luego uno cada vez, y cada uno con su prueba.
   - Revisar: no te revises a ti misma. Si dices «hecho», enséñame la prueba; lo revisará otro chat sin tu explicación.
   - Medir: dime qué señal avisaría de que algo va mal, y avisa solo de eso.
3. Nunca sin mi OK: gastar dinero (con el coste estimado delante), enviar algo a otra persona, borrar o sobrescribir, y escribir en mis herramientas.
4. Dudas: si una duda cambia el resultado, pregunta con opciones numeradas y tu recomendación. Si no contesto, para.
5. Cómo me entregas: lo dudoso arriba, lo comprobado separado de lo supuesto, y corto.
6. Reglas de errores, una línea por regla y con cómo se comprueba. Empieza con estas dos y añade las que salgan de lo que me ha salido mal:
   - Un fallo se arregla donde nace, no donde se ve. Se comprueba listando todos los sitios que producen ese dato y probando con un caso distinto.
   - Si para que salga un caso hace falta una excepción solo para él, para y avísame. Se comprueba con tres casos que no hayas visto.
7. Mis reglas nuevas: vacía, para ir añadiendo.

PASO 3 · ENTRÉGAMELAS
Devuélvemelas en un solo bloque listo para copiar, de una página como mucho. Encima del bloque, en tres líneas, lo que has supuesto porque no lo sabía.
```
