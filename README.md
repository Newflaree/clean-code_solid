# Proyecto para practicar

Este es un proyecto de Vanilla TypeScript en Vite, para trabajar los ejercicios del curso sobre Principios SOLID y CleanCode.

Clonar o descargar el proyecto y luego:
```
yarn
```

Para ejecutar el proyecto, simplemente ejecuten
```
yarn dev
```

# Clean Code y Deuda técnica
### ¿Qué es la deuda técnica?
Básicamente, es la falta de calidad en el código, que genera una deuda que repercutirá en costos futuros. Estos costos, usualmente, son contos económicos y se ven reflejados en:
* Tiempo en realizar mantenimiento.
* Tiempo en refactorizar código.
* Tiempo en comprender el código.
* Tiempo adicional en la transferencia del código

## Esquema de deuda técnina de Martin Fowler
Hay cuatro cuadrantes en los cuales nosotros podemos agrupar nuestra deuda.
* Deuda Imprudente y Deliberada: Es el tipo de deuda en la cuál es desarrollador actúa de forma conciente y de forma imprudente. Esto suele resultar en un proyecto que tiene mala calidad y es poco tolerante al cambio.
```
"No hay tiempo, sólo copia y pega eso de nuevo"
```

* Deuda Imprudente e Inadvertida: Probablemente es la deuda más peligrosa ya que esta se genera por el desconocimiento o falta de experiencia. Usualmente, esta deuda es generada por desarrolladores de perfil Junior o lo que es peor, un falso Senior.
```
"¿Qué son los patrones de diseños?"
```

* Deuda Prudente y Deliberada: Es cuando sabemos que tenemos una deuda y estamos concientes de ella. El peligro radica en que si no se paga a tiempo, más interes vamos a pagar después. Este tipo de deuda es bastante común cuando se llega a un punto del proyecto y decimos "dejemos un TODO y luego lo hacemos".
```
"Tenemos que entregar rápido, ya refactorizaremos"
```

* Deuda Prudente e Inadvertida: Es común que en la mayoría de los proyectos, ya sea cuando está comenzando, nosotros no temenos el conocimiento total de cómo va a terminar luciendo el mismo. Este tipo de deuda se encuentra cuando el proyecto ya está avanzado, no la estructura o analisas del mismo, si no cuendo empezamos a codificar la aplicación. Ahí nos damos cuenta que quizás no utilizamos la mejor arquitectura o la mejor forma de abordarlo. En el punto en que cae la deuda, nosotros vamos a considerar si vale la pena volverlo a hacer o seguimos adelante.
```
"Ahora sabemos cómo lo deberíamos haber hecho"
```

- Usualmente, caer en la deuda técnica es normal y a menudo es inevitable. Siempre hay que estar pendiente de la deuda técnica y preocuparse por pagarla

### ¿Cómo se paga una deuda técnica?
La palabra clave es la Refactorización. Es simplemente un proceso que tiene como objetivo mejorar el código sin alterar su comportamiento para que sea más entendible y tolerante a cambios.

Usualmente, para que una refactorización fuerte tenga el objetivo esperado, es imprescindible contar con pruebas automáticas.

Si no tenemos pruebas automáticas, no tenemos manera de saber que la refactorización funcionó de la manera esperada. Usualmente esto produce el famoso "Si funciona, no lo toques" ya que el código no es robusto ni tolerante a cambios. Si nosotros no tenemos una forma ordenada de trabajar ni pruebas automáticas, se tiene menos confianza al realizar un cambio necesario. Esto es más común cuando se trabaja con código que no escribimos.

La mala calidad del Software siempre la acaba pagando o asumiendo alguien. Ya sea el cliente, el proveedor con recursos o el propio desarrollador dedicando tiempo a refactorizar o malgastando el tiempo programando sobre un sistema frágil.

Existen dos tipos de programadors. Los que ya han experimentado esto y los que están a punto de experimentarlo.

## Clean Code
```
"Código Limpio es aquel que se ha escrito con la intención de que otra persona (o tú mismo en el futuro) lo entienda." - Carlos Blé
```

```
"Nuestro código tiene que ser simple y directo, debería leerse con la misma facilidad que un texto bien escrito." - Grady Booch
```

```
"Programar es el arte de decirle a otro humano lo que quieres que la computadora haga." - Donald Knuth
```

Cuando estamos hablando de código limpio, se procura que nuestro código sea universal y muy fácil de leer.
