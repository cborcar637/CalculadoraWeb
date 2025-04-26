# Calculadora en HTML, CSS y JavaScript

Este repositorio contiene una **plantilla de calculadora** creada con **HTML, CSS y JavaScript**.  
El **contenido** (HTML) y la **apariencia** (CSS) están completos, pero el **código JavaScript** está incompleto, por lo que tendrás que editarlo para que la calculadora funcione correctamente.

---

## ¿Cómo se hace?

### 1. Pasos iniciales

La calculadora puede hacerse **desde cero** o a partir de **esta plantilla** (opción más sencilla).  Si eliges usar la plantilla, tienes dos formas de obtener el código:

#### Opción recomendada

- Pulsa en **`Code > Download ZIP`** para descargar el repositorio.
- Descomprime el archivo ZIP en tu ordenador.
- Edita los archivos para completar la calculadora.
- Cuando termines, **sube tu versión a GitHub** y **publica la web con GitHub Pages** (como en el primer trabajo en grupo).

#### Opción alternativa

- Pulsa en **`Fork > Create a new fork`**. Esto creará una copia del repositorio en tu cuenta de GitHub.
- Edita el código directamente desde ahí.

---

### 2. Edición del código

Dentro del archivo JavaScript encontrarás líneas marcadas con `// TODO`.  Tienes que **sustituir esas líneas** por el código que haga lo que se indica en el comentario.  

Por ejemplo, la línea 15 contiene esto:

```js
// TODO: Resetear el valor de la variable `valorEnPantalla`
```

Tendrás que reemplazarla por:

```js
valorEnPantalla = "";
```

> 🔍 **Consejo**: Antes de empezar a modificar, **lee y analiza bien el código**. Prueba poco a poco y asegúrate de entender qué hace cada parte.

Cuando se hayan reemplazado todas las líneas `// TODO` por las líneas de código correspondientes, y se haya probado que la calculadora funciona, **sube tu versión a GitHub** y **activa GitHub Pages** para que tu calculadora esté publicada en la web.

---

## Funcionamiento del código

### Variables principales

- `valorEnPantalla` (texto): contiene lo que se muestra en el display.
- `operando1` (número): contiene el valor del primer operando.
- `operando2` (número): contiene el valor del segundo operando.
- `operador` (texto): almacena el operador (`+`, `-`, `*`, `/`).

### Lógica general

El código funciona de la siguiente forma:

1. El usuario pulsa números y conforme va pulsando se van añadiendo al valor de la variable  `valorEnPantalla`.
2. Al pulsar un operador, se guarda el valor actual en la variable `operando1` y el operador en la variable `operador`. También se borra `valorEnPantalla` para limpiar el display y que el usuario introduzca el segundo número.
4. El usuario introduce el segundo número de la misma forma que en el punto 1.
5. Al pulsar `=`, se guarda el valor en `operando2`, se realiza la operación y se muestra el resultado en el display.
6. Al pulsar `C`, se reinician todas las variables.

---

## Funciones que debes completar

- **`resetearVariables`**: borra los valores de todas las variables (`""` para texto y `null` para números). Se ejecuta cuando se pulsa C o cuando termina una operación.
- **`actualizarDisplay`**: muestra en el display el contenido de `valorEnPantalla`. Se llama cada vez que "valorEnPantalla" cambia.
- **`agregarNumero`**: añade el número pulsado a `valorEnPantalla`. Se ejecuta cuando se pulsa un número del 0 al 9.
- **`operadorPulsado`**: se ejecuta al pulsar un operador (`+`, `-`, `*`, `/`).
- **`calcular`**: se ejecuta al pulsar `=`. Realiza la operación con los valores que hay en `operando1`, `operando2` y `operador` y muestra el resultado.

---

## 📺 Vídeo explicativo

Puedes ver una explicación paso a paso en el siguiente vídeo:  
🔗 [[Enlace al vídeo explicativo](https://youtu.be/ab8X9I8gh7c)](#)
