### PROBLEMA 1
![Ejercicio 1](/LAB1-SIS2310/contenido/Imagenes/image1.png)
>Escriba un script bash que imprima la cadena "HOLA".
```
echo "HELLO"
```
![Ejercicio 1](/LAB1-SIS2310/contenido/Imagenes/image2.png)

### PROBLEMA 2
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image3.png)
>Su tarea es utilizar bucles for para mostrar solo números naturales impares del 1 al 99.
```
for((i=1;i<=99;i++))do
if((i%2!=0))
then 
echo $i
fi
done
```
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image4.png)

### PROBLEMA 3
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image5.png)
>Escriba un script Bash que acepte `name` como entrada y muestra el saludo "Bienvenido (nombre)">
```
read  name
echo "Welcome $name"
```
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image6.png)

### PROBLEMA 4
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image7.png)
>Utilice un bucle for para mostrar los números naturales de 1 al 50.
```
for((i=1;i<=50;i++))do
echo $i
done
```
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image8.png)

### PROBLEMA 5 
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image9.png)
>Dados dos números enteros,`x` y `y`, encuentra su suma, diferencia, producto y cociente.
```
read a
read b
echo $[a+b]
echo $[a-b]
echo $[a*b]
echo $[a/b]
```
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image10.png)

### PROBLEMA 6
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image11.png)
>Dados dos números enteros,`x`y `y`, identificar si `x < y`o `x > y`o `x = y`
```
read x
read y
if (($x < $y))
then
  echo "X is less than Y"
elif (($x > $y))
then
  echo "X is greater than Y"
else
  echo "X is equal to Y"
fi
```
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image12.png)
### PROBLEMA 7
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image13.png)
>Lee un carácter de la entrada estándar.
Si el carácter es 'Y' o 'y', se muestra "SÍ".
Si el carácter es 'N' o 'n', se muestra "NO".
No se proporcionará ningún otro carácter como entrada.
```
read Y
if [[ $Y = 'y' ]]
then
    echo "YES"
elif [[ $Y = 'Y' ]]; then
    echo "YES"
else
echo "NO"
fi
```
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image14.png)

### PROBLEMA 8
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image15.png)
>Dados tres números enteros (X, Y, Z) que representan los tres lados de un triángulo, identifica si el triángulo es escaleno, isósceles o equilátero.
Si los tres lados son iguales, salida EQUILATERAL.
De lo contrario, si dos lados son iguales, se genera ISOSCELES.
De lo contrario, salida SCALENE.
```
read a
read b
read c 
if (( $a == $b && $b == $c )) 
then
echo "EQUILATERAL"
elif (( $a == $b || $a == $c || $b == $c )); then
echo "ISOSCELES"
else
echo "SCALENE"
fi
```
![Ejercicio 2](/LAB1-SIS2310/contenido/Imagenes/image16.png)
