# Ejercicio2
Ejercicio 2 Calculo de Saldo
#  Calculo de Saldo Financiero (Ejercicio 2)


## Descripción
Este Sitema calcula el saldo financiero total procesando una lista de transacciones que pueden ser de tipo "ingreso" o "egreso".
Es una solución eficiente diseñada para manejar diversos escenarios de datos financieros.

- Proceso
    -Comenzar con un saldo inciial de 0
    -Verificar si la lista de transacciones está vacía
    -Recorrer cada dato en la lista secuencialmente
    -Validación para la identificaciond el tipo de transaccion (ingreso/egreso)
    -Operacion matematica para Sumar o Restar saldo
    -Devolver el saldo final calculado


## Analisis de Complejidad
-Temporal
    -Número de transacciones en la lista
    -Cada transacción se procesa solo 1 vez
    -Validaciones por si la lista esta vacía

-Espaciles
    -Uso de memoria contante
    -Utilización de solo 1 variable (saldo acumulado) para el almacenamiento
    -La estructura de la lista


## Casos de prueba
** Caso 1 Mixta

    {
        "datos": [
            {"id": 1, "monto": 300, "tipo": "ingreso"},
            {"id": 2, "monto": 50, "tipo": "egreso"},
            {"id": 3, "monto": 100, "tipo": "ingreso"},
            {"id": 4, "monto": 100, "tipo": "egreso"}
        ]
    }

    Cálculo : 300 - 50 + 100 - 100 = 250
    Saldo esperado : 250

** Caso 2
    {
        "datos": [
            {"id": 1, "monto": 100, "tipo": "egreso"},
            {"id": 2, "monto": 50, "tipo": "egreso"},
            {"id": 3, "monto": 75, "tipo": "egreso"}
        ]
    }
    Cálculo : 100 - 50 - 75 = -225
    Saldo esperado : -225

** Caso 3

    {
        "datos": []
    }
     
    Saldo esperado :0
