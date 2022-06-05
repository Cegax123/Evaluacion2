# Evaluacion2

---

*Ejecuta el programa y presenta los resultados y explica que sucede.*

Luego de ejecutar el programa, obtenemos el siguiente resultado:

```
Lista de pasajeros de vuelos de negocios:
Cesar
Lista de pasajeros de vuelos economicos:
Jessica
```

Se ejecutan ciertos escenarios posibles, pero las pruebas no son exhaustivas. Por ejemplo, tratar de añadir y remover un pasajero VIP de un vuelo de tipo económico.

---

1. Si ejecutamos las pruebas con cobertura desde IntelliJ IDEA, ¿cuales son los resultados que se muestran?, ¿Por qué crees que la cobertura del código no es del 100%?

    Los resultados obtenidos son los siguientes

    ![Alt text](images/preg1.PNG)

    Podemos ver que las pruebas "Dado que hay un vuelo de negocios" fallan.

   Esto sucede porque para relizar las pruebas, existe una colisión de nombres en el atributo `flightType`

   En el método addPassenger(), se comprueba si es de tipo "Negocios"

   ![Alt text](images/vuelonegocios.PNG)

   En la prueba, se instancia un objeto de tipo "Business"

   ![Alt text](images/testAirport1.PNG)

---

2. ¿Por qué John tiene la necesidad de refactorizar la aplicación?

   El error en las pruebas que se cometió es muy sencillo de que pueda volver a pasar. Sobre todo, si se trabaja en un equipo, no todos sabrán que el `flightType` tiene que ser 'Negocios' y no 'Business'. Por lo que necesitamos refactorizar el código, para evitar que se de el mismo error en el futuro.

---

*Revisa la Fase 2 de la evaluación y realiza la ejecución del programa y analiza los resultados.*

Ahora podemos observar que todas las pruebas pasaron correctamente:

![img.png](images/testAirport2.png)

Por lo que la refactorización se realizó con éxito

---

