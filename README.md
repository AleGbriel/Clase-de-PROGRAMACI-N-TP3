PUNTO NUMERO 1
Proceso NumeroPositivoNegativoOCero
    Escribir "Ingrese un número:"
    Leer num
    Si num > 0 Entonces
        Escribir "El número es positivo."
    Sino
        Si num < 0 Entonces
            Escribir "El número es negativo."
        Sino
            Escribir "El número es cero."
        FinSi
    FinSi
FinProceso



PUNTO NUMERO 2

Proceso NumeroParOImpar
    Escribir "Ingrese un número entero:"
    Leer num
    Si num % 2 = 0 Entonces
        Escribir "El número es par."
    Sino
        Escribir "El número es impar."
    FinSi
FinProceso




PUNTO NUMERO 3

Proceso ConjuntoDeNumeros
    Definir numeros, opcion, n Como Entero
    Dimension numeros[100]
    contador <- 0
    Repetir
        Escribir "1. Agregar número"
        Escribir "2. Verificar número"
        Escribir "3. Salir"
        Leer opcion
        Segun opcion Hacer
            1:
                Escribir "Ingrese un número:"
                Leer n
                contador <- contador + 1
                numeros[contador] <- n
            2:
                Escribir "Ingrese el número a verificar:"
                Leer n
                encontrado <- Falso
                Para i <- 1 Hasta contador Hacer
                    Si numeros[i] = n Entonces
                        encontrado <- Verdadero
                    FinSi
                FinPara
                Si encontrado Entonces
                    Escribir "El número está en el conjunto."
                Sino
                    Escribir "El número no está en el conjunto."
                FinSi
        FinSegun
    Hasta Que opcion = 3
FinProceso



PUNTO NUMERO 4

Proceso PromedioDeCinco
    Definir i, suma, num Como Real
    suma <- 0
    Para i <- 1 Hasta 5 Con Paso 1 Hacer
        Escribir "Ingrese el número ", i, ":"
        Leer num
        suma <- suma + num
    FinPara
    Escribir "El promedio es: ", suma / 5
FinProceso



PUNTO NUMERO 5


Proceso ContarCaracteres
    Definir frase Como Cadena
    Escribir "Ingrese una frase:"
    Leer frase
    Escribir "La frase tiene ", Longitud(frase), " caracteres."
FinProceso



PUNTO NUMERO 6


Proceso SumaHastaNegativo
    Definir num, suma Como Real
    suma <- 0
    Repetir
        Escribir "Ingrese un número (negativo para terminar):"
        Leer num
        Si num >= 0 Entonces
            suma <- suma + num
        FinSi
    Hasta Que num < 0
    Escribir "La suma de los números ingresados es: ", suma
FinProceso


