# **Agenda**
mis apuntes
## **apuntes de lo aprendido en clases**
aprendimos utilizar el **visual basic excel** y sus comandos

## 1 **inicio y final**
 para iniciar un programa tiene que tener un comienzo tener un sub **(nombre)** y
 para finalizar es end sub
## **para empezar a ejecutar lo que escribes**
para empezar lo que quieres escribir y como ejecutar es con el comando de
> msgbox   = > maria
## **variables**
a las variables se le asigna un valor y tambien pues se pueden reemplazar
por ejemplo si queremos asignar una valor a una variable debemos poner entre
comillas el nombre que le vamos asignar a la variable dentro de comillas " luis "
y para reemplazar ponemos >msgbox
## **diagrama de flujo**
en el diagrama de flujo podrmos ordenar y organizar de como va a ser todo lo
que vamos a ejecutar en el programa ejemplo de es:

>sub
>nom = "luis"
>num = 10
>msgbox en cada una de ellas de los valores que se le dan a la variable para ejecutars
>end sub

### viernes 2 de septiembre


´´´´

    Sub actividad()
        
        For y = 2 To 21
            nom = nombres.Cells(y, 1)
            ult = Len(nom) - 1
            nombres.Cells(y, 2) = Mid(nom, ult, 2)
            
        Next y
        
    End Sub

# Programacion (algoritmo)
si (estructura)
inicio
|
| si cond entonces
| sino
| fin si
fin 
inicio
|
| si 1 > 9 entonces
|  escriba "si"  
| sino
| escriba " no"
| fin si
| fin