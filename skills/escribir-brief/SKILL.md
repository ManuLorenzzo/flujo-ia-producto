---
name: escribir-brief
description: Convierte una petición vaga en un brief de cinco partes (lo dudoso arriba, el problema de fondo, qué hay que hacer en pasos, lo que no se hace y cómo sabremos que funciona) y pregunta lo que falta antes de empezar. Úsala cuando el usuario pida algo que va a hacer la IA y el encargo sea impreciso, como "hazme una pantalla de registro", "prepárame el análisis", "ordena esto" o "escribe a los usuarios", o diga "haz el brief", "encárgalo bien" o "antes de empezar".
---

# Escribir un brief

Una IA que recibe una petición vaga rellena los huecos con lo que le parece. Esta skill obliga a cerrar los huecos **antes** de hacer nada.

## Qué hacer

1. **Lee la petición** y detecta qué falta. No empieces a hacer el trabajo.
2. **Pregunta lo que falta en un solo mensaje**, con 3 a 6 preguntas como máximo, numeradas y con tu recomendación en cada una (para que pueda contestar «1, 2 y 3 como dices»). Si algo ya se ha dicho en la conversación, no lo vuelvas a preguntar.
3. **Escribe el brief** con las cinco partes de abajo y pide OK. No empieces el trabajo hasta tenerlo.
4. Si el usuario dice que no contesta ahora, para. No elijas tú por él.

## Las cinco partes

### 1. El problema de fondo
No qué se pide, sino qué decisión o qué dolor hay detrás. Una frase. Si el encargo es un caso concreto, escribe la clase: «el problema es que los dueños abandonan en el registro», no «cambia el texto del botón».

### 2. Lo dudoso, arriba
Lo que no sabes, lo que vas a suponer si nadie dice nada y lo que no se puede comprobar con lo que hay. Cada duda, con su opción recomendada. Esta parte va **la primera** al presentar el brief, aunque sea la 2.

### 3. Qué hay que hacer, en pasos
Pasos pequeños y comprobables, en orden. Cada uno con su «hecho cuando...». Sin verbos vagos como «mejorar» o «revisar un poco».

### 4. Lo que no se hace
La parte que más tiempo ahorra. Qué no se toca, qué no se envía, qué no se gasta, qué no se escribe en las herramientas del usuario. Si no hay nada que prohibir, pregunta: casi siempre lo hay (gastar dinero, enviar, borrar, escribir en sus herramientas).

### 5. Cómo sabremos que funciona
Una señal medible que diga si el trabajo ha servido, no solo si está hecho. Sin esta línea no sabes si ha salido bien.

## Formato de salida

```
BRIEF

Lo dudoso (arriba)
- [duda] > propongo: [opción]

El problema de fondo
[una frase]

Qué hay que hacer, en pasos
1. [paso] · hecho cuando: [criterio]

Lo que no se hace
- [límite]

Cómo sabremos que funciona
[señal medible]

¿OK para empezar? Si no contestas, no empiezo.
```

## Ejemplo

**Petición:** «Hazme una pantalla de registro para Pawly.» (Pawly es una startup ficticia: un marketplace de paseadores y cuidadores para dueños de perros en España.)

**Preguntas que haces:**
1. ¿Cuál es el problema que quieres resolver? Recomiendo partir de un dato: ¿cuántos dueños abandonan hoy en el registro?
2. ¿Pedimos los datos del perro al registrarse o más tarde? Recomiendo más tarde, para no frenar.
3. ¿Qué no se debe tocar? Recomiendo: pagos y el resto de pantallas.
4. ¿Cómo sabremos que ha funcionado? Recomiendo: que abandonen menos de 5 de cada 20.

**Brief resultante:**

```
Lo dudoso (arriba)
- ¿Pedimos el teléfono ya? Propongo: al reservar el primer paseo.

El problema de fondo
9 de cada 20 dueños abandonan en el registro: les pedimos demasiados datos del perro de entrada.

Qué hay que hacer, en pasos
1. Registro con email y nombre, en un solo paso · hecho cuando: un dueño nuevo lo completa sin ayuda.
2. Los datos del perro, después del registro · hecho cuando: el registro no pide nada del perro.
3. Ver dónde se van · hecho cuando: sabemos en qué campo abandona cada dueño.

Lo que no se hace
- Ni login con Google.
- Ni tocar pagos.
- Ni rediseñar el resto de la app.

Cómo sabremos que funciona
Abandonan menos de 5 de cada 20.

¿OK para empezar? Si no contestas, no empiezo.
```

## Huecos

Si al usarla notas que al brief le falta una parte para un tipo de encargo, dilo al final: la skill se mejora con cada uso.
