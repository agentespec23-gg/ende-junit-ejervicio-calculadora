# Testing con Junit

Este es un ejemplo sencillo de pruebas unitarias usando Junit 5

Observa que este proyecto no tiene ninguna clase con el método `main`, no nos hace fatal. Además, tampoco tiene ningún `scanner` ni ningún `print`.

Haz un fork de este proyecto en tu repositorio de Github y contesta a las siguientes preguntas:

1. ¿Qué sentido puede tener este proyecto y para que lo podrías usar?

Se puede usar para realizar calculos matematicos basicos, este programa te lo puedes guardar como libreria para tenerlo por si en algun momento lo necesitas y asi no tienes que codificarlo de nuevo

2. Revisa las pruebas de la suma y comenta lo que te parezca de interés

Me parece interesante lo facil que se comprueba si estan bien o mal los resultados de cualquier pèracion

3. Realiza un estudio de caja negra de la división e implementa las pruebas en junit: Se realizará en markdown.

vamos a poner los valores de 0, -4, y 6 para comprobar que el programa de division 

@Test
   void sumar() {
      Assertions.assertAll("division", new Executable[]{() -> {
         Assertions.assertEquals(0, Calculadora.dividir(0, 4), "0 / 4 = 0");
      }, () -> {
         Assertions.assertEquals(6, Calculadora.dividir(6, 3), "6 + 3 = 2");
      }, () -> {
         Assertions.assertEquals(-2, Calculadora.dividir(8, -4), "8 + -4 = -2");
      }});
   }

## Instrucciones

El alumno deberá hacer un fork de este proyecto, poner el repositorio como **privado**, agregar al profesor como colaborador (julparper) e implementar la solución solicitada (preguntas y código).

>Se deberá utilizar este fichero, y los artefactos de código del proyecto, para resolver el ejercicio.


**Si no se puede acceder al repositorio la evaluación del ejercicio será de 0. No se evaluarán entregas modificadas/entregadas fuera del plazo establecido en la tarea**