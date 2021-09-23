# ConversorDec2Bin
 
Este programa tiene como propósito transformar numeros en *decimal* a :sparkles:binario:sparkles:\. Para hacer esto hacemos uso de la siguiente función\:
```python
def dec2bin(numero_decimal, numero_bits):
    numero_binario = bin(numero_decimal)
    if numero_decimal >= 0:
        numero_binario = numero_binario[2:len(numero_binario)]  # quita el "0b" del principio
        while len(numero_binario) < numero_bits:      # añade 0's a la izquierda si hace falta
            numero_binario = "0" + numero_binario
    else:
        numero_binario = numero_binario[3:len(numero_binario)] # quita el "-0b" del principio
        while len(numero_binario) < numero_bits: # añade 1's a la izquierda si hace falta
            numero_binario = "1" + numero_binario

    return numero_binario
```
**A partir de aquí voy a poner ejemplos de formateo de markdown**\.
Aquí|voy a
----|------
escribir|una tabla

Ahora voy a poner una de mis citas favoritas, como dijo un filósofo antiguo\:
>Si no se te ocurre ninguna cita, invéntatela. Y al autor también.

Y aquí una foto de un :dog:\:
![foto de un perrito de una web de imágenes gratuitas, para que no sea plagio](https://images.pexels.com/photos/2253275/pexels-photo-2253275.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)