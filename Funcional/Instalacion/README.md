## ¿Qué hay que instalar?

### Git

[Link](https://git-scm.com/downloads) para descargar `Git` 

### Stack

`Stack` es una herramienta para construir y manejar proyectos en Haskell, el lenguaje que vamos a usar en este paradigma.

[Link](https://docs.haskellstack.org/en/stable/README/#how-to-install) para descargar Stack, para diferentes sistemas operativos :) 


### Editor de texto

- Recomendado: Visual Studio Code.
- Instalar el plugin [`Haskell`](https://marketplace.visualstudio.com/items?itemName=haskell.haskell),

## Instalacion per se

1. El primer paso ahora es clonar este repositorio, desde la terminal. 

2. Ahi mismo, y en este paso, le pedimos a stack que compile el proyecto con `stack build`.
Este paso va a tardar un rato.
Como aun no tenemos Haskell instalado, en este paso Stack va a descargar la versión de Haskell que esté especificada en el proyecto. Como en todos los ejercicios vamos a usar la misma versión, es la única vez que va a pasar esto.

3. Una vez que terminó de descargarse e instalarse todo en el paso interior, vamos a correr los tests para garantizar que todo haya salido bien: `stack test`.
  
   Si ves este mensaje significa que todo ya está instalado y andando:
   ```
   Test de ejemplo
   El doble de un número es el número más si mismo
   ```

4. Abrir el proyecto con Visual Studio Code y validar que el plugin `Haskell` se haya instalado correctamente:
Desde visual studio code, abren la carpeta del ejercicio y van a `src/Library.hs`, si poniendo el cursor sobre "numero" les aparece un cartel que dice `Number`, significa que el plugin está funcionando :D.
 

### ¿Por qué Stack? 
Estamos usando Stack porque permite hacer algunas cosas que serían más difíciles de hacer con Haskell "pelado" como por ejemplo:
- Asegurarse que todos estemos trabajando con la misma versión de Haskell.
- Instalar dependencias (como el PdePreludat).
- Correr los tests.
### ¿Qué es `import PdePreludat`?
PdePreludat es una librería que se usa en pdep en vez de la librería estandar que usa Haskell por defecto (la cual se llama Prelude). Idealmente simplifica algunas cosas que no son necesarias a la materia y mejora algunos mensajes de error que les pueden aparecer en Haskell. El `import PdePreludat` lo necesitamos para poder usar un montón de funciones que vamos a usar en la materia (como la función suma `(+)` que aparece en este ejercicio).
