# Guía de elementos Markdown compatibles con GFM

Este documento reúne los elementos principales de **Markdown** compatibles con ***GitHub Flavored Markdown (GFM)***.

## Índice

1. [Encabezados](#encabezados)
2. [Párrafos y saltos de línea](#párrafos-y-saltos-de-línea)
3. [Énfasis](#énfasis)
4. [Citas](#citas)
5. [Listas](#listas)
6. [Listas de tareas](#listas-de-tareas)
7. [Código](#código)
8. [Reglas horizontales](#reglas-horizontales)
9. [Enlaces](#enlaces)
10. [Imágenes](#imágenes)
11. [Tablas](#tablas)
12. [Escapado de caracteres](#escapado-de-caracteres)
13. [HTML embebido](#html-embebido)
14. [Notas al pie](#notas-al-pie)
15. [Detalles desplegables](#detalles-desplegables)
16. [Bloque mixto de ejemplo](#bloque-mixto-de-ejemplo)

---

## Encabezados

# Encabezado H1
## Encabezado H2
### Encabezado H3
#### Encabezado H4
##### Encabezado H5
###### Encabezado H6

También existe la sintaxis alternativa para H1 y H2:

Encabezado nivel 1
==================

Encabezado nivel 2
------------------

## Párrafos y saltos de línea

Este es un párrafo normal. GFM agrupa líneas consecutivas dentro del mismo párrafo.

Si quieres separar párrafos, deja una línea en blanco entre ellos.

Para forzar un salto de línea al final de una línea, añade dos espacios.  
Esta línea aparece debajo de la anterior.

## Énfasis

*Cursiva con asteriscos*

_Cursiva con guiones bajos_

**Negrita con asteriscos**

__Negrita con guiones bajos__

***Negrita y cursiva***

~~Texto tachado~~

`Código en línea`

## Citas

> Esta es una cita.
>
> Puede ocupar varias líneas.

> Cita anidada
>> Segundo nivel de cita
>>> Tercer nivel de cita

## Listas

### Lista no ordenada

- Elemento con guion
- Otro elemento
  - Subelemento
  - Otro subelemento
- Elemento final

### Lista no ordenada alternativa

* Elemento con asterisco
* Otro elemento

### Lista ordenada

1. Primer elemento
2. Segundo elemento
3. Tercer elemento

### Lista ordenada con numeración flexible

1. Uno
1. Dos
1. Tres

### Lista con bloques internos

1. Elemento con párrafo.

   Texto adicional dentro del mismo elemento.

2. Elemento con bloque de código:

   ```bash
   echo "hola mundo"
   ```

## Listas de tareas

- [x] Tarea completada
- [ ] Tarea pendiente
- [ ] Otra tarea pendiente

## Código

### Código indentado

    const mensaje = "bloque indentado";
    console.log(mensaje);

### Bloque de código cercado

```js
function saludar(nombre) {
  return `Hola, ${nombre}`;
}
```

### Bloque de código con otro lenguaje

```json
{
  "name": "gfm-demo",
  "version": "1.0.0",
  "private": true
}
```

### Bloque sin resaltado

```text
Texto literal
sin resaltado
de sintaxis.
```

## Reglas horizontales

---

***

___

## Enlaces

### Enlace en línea

[GitHub](https://github.com)

### Enlace con título

[OpenAI](https://openai.com "Sitio de OpenAI")

### Referencia enlazada

[Referencia a GitHub][github-ref]

[github-ref]: https://github.com

### Autolinks

<https://example.com>

<correo@example.com>

### URL literal

https://github.com/features/copilot

## Imágenes

### Imagen en línea

![Texto alternativo](https://placehold.co/600x200 "Título opcional")

### Imagen con referencia

![Logo de ejemplo][img-ref]

[img-ref]: https://placehold.co/120x120

## Tablas

| Columna | Tipo | Descripción |
| --- | --- | --- |
| `id` | entero | Identificador único |
| `nombre` | texto | Nombre visible |
| `activo` | booleano | Estado del registro |

### Alineación en tablas

| Izquierda | Centro | Derecha |
| :--- | :---: | ---: |
| A | B | C |
| 10 | 20 | 30 |

## Escapado de caracteres

\*Esto no será cursiva\*

\# Esto no será un encabezado

\[Texto literal entre corchetes\]

## HTML embebido

<div>
  <strong>HTML inline o en bloque</strong> puede coexistir con Markdown en muchos casos.
</div>

<kbd>Cmd</kbd> + <kbd>K</kbd>

<sub>texto subíndice</sub> y <sup>texto superíndice</sup>

## Notas al pie

Aquí hay una nota al pie.[^1]

Otra nota con más texto.[^nota-larga]

[^1]: Esta es una nota al pie simple.
[^nota-larga]: Esta es una nota al pie más extensa, compatible con la renderización de GitHub.

## Detalles desplegables

<details>
  <summary>Haz clic para expandir</summary>

  Este contenido queda oculto hasta que el lector lo despliega.

  - Sirve para ejemplos largos
  - O para secciones opcionales
</details>

## Bloque mixto de ejemplo

> GitHub soporta algunas extensiones adicionales según el contexto.
> Si necesitas máxima portabilidad, prioriza encabezados, listas, citas, enlaces, tablas, código y énfasis.

### Ejemplo combinado

1. Crear el archivo.
2. Añadir contenido.
3. Revisar el resultado.

```md
# Título

- [x] Escribir contenido
- [ ] Publicarlo

Consulta [la documentación](https://docs.github.com/).
```

Tabla rápida:

| Paso | Estado |
| --- | --- |
| Crear | Hecho |
| Validar | Pendiente |

Fin del documento.
