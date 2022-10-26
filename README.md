# **agaenda**
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
```
>sub
>nom = "luis"
>num = 10
>msgbox en cada una de ellas de los valores que se le dan a la variable para ejecutars
>end sub
```

### viernes 2 de septiembre


´´´´

    Sub actividad()
        
        For y = 2 To 21
            nom = nombres.Cells(y, 1)
            ult = Len(nom) - 1
            nombres.Cells(y, 2) = Mid(nom, ult, 2)
            
        Next y
        
    End Sub

´´´´

# taller-26-de-agosto

```
Sub actividad()

  ingresos = InputBox("ingrese impuestos anuales de la empresa")

  If ingresos >= 0 And ingresos < 1000 Then
      MsgBox "no paga impuesto"
  Else
      If ingresos >= 1001 And ingresos < 10000 Then
          valor = 0.05 * ingresos
          MsgBox "el impuesto a pagar anual es:" & valor
          Else
          If ingresos >= 10001 And ingresos < 100000 Then
              valor = 0.1 * ingresos
              MsgBox "el impuesto a pagar anual es:" & valor
          Else
              If ingresos >= 100001 And ingresos < 1000000 Then
                  valor = 0.15 * ingresos
                  MsgBox " el impuesto a pagar es:" & valor
              Else
                  If ingresos >= 1000001 And ingresos < 10000000 Then
                  valor = 0.2 * ingresos
                  MsgBox " el impuesto a pagar es:" & valor
                  Else
                  If ingresos >= 10000001 Then
                      valor = 0.25 * ingresos
                      MsgBox "el impuesto a pagar es:" & valor
                  Else
                      MsgBox "No se puede"
                  End If
                  End If
              End If
          End If
      End If
  End If
  End Sub
```


## taller- for

Sub evento()
    siabon = 0
    noabon = 0
    abono_s10000 = 0
    totalabon = 0
    ab = 0
    
    For i = 1 To 3
        ab = Int(InputBox("ingrese la cantidad a donar"))
        If ab >= 1000 Then
               siabon = siabon + 1
             If ab >= 10000 Then
               abono_s10000 = abono_s10000 + 1
             End If
        Else
             noabon = noabon + 1
        End If
           
    totalabon = totalabon + ab
    
    Next i
    promedio = totalabon / siabon
    MsgBox "Donaron" & "(" & siabon & ")" & " personas"
    MsgBox "No donaron " & "(" & noabon & ") " & " personas"
    MsgBox "Donaron mas de 10000 " & "(" & abono_s10000 & ")" & "personas"
    MsgBox "El total abonado es " & total_abonado
    MsgBox "El promedio de los estudiantes que abonaron fue de " & promedio
End Sub
```

## taller-dart-cadenas 

```
void main() {
 
  Gato gato = Gato();
  gato.emitirSonidos();
  
  Vaca vaca = Vaca();
  vaca.emitirSonidos();
  
  Perro perro = Perro();
  perro.emitirSonidos();
  perro.nombre = "camilo";
  print(perro.nombre);
  
  Carnivoro.imc(8,9);  
}
abstract class Animal{ 
 void emitirSonidos ();
}
class Gato implements Animal{ 
  @override 
 void emitirSonidos (){ 
   print('el sonido del gato es: miau');
 }
} 
class Vaca implements Animal{ 
   @override
 void emitirSonidos (){ 
   print('el sonido de la vaca es: muu');
 }
}
class Perro extends Carnivoro implements Animal{ 
 void emitirSonidos (){ 
   print('el sonido que hace el perro es: gua');
 }
} 
class Carnivoro{ 
 String? nombre;
 static void imc (int altura, int peso){ 
   print(altura*peso);
 }
}
```
## taller-herencia
```
void main(){
  
  Conejo conejo = Conejo();
  
  conejo.nombre = 'conejo';
  conejo.edadPromedio = 6;
  conejo.reproduccion = 'sexual';
  conejo.alimento = 'zanahoria, lechuga';
  conejo.bioma = 'bosques';
  Leon leon = Leon();
  
  leon.nombre = 'leon';
  leon.edadPromedio = 10;
  leon.reproduccion = 'sexual';
  leon.alimento = 'antilopes, bufalos';
  leon.bioma = 'sabanas';
  Hiena hiena = Hiena(); 
  
  hiena.nombre = 'hiena';
  hiena.edadPromedio = 20;
  hiena.reproduccion = 'sexual';
  hiena.alimento = 'serpientes, lagartos';
  hiena.bioma = ' sabana, matorrales y desierto.';
  Hombre hombre = Hombre();
  
  hombre.nombre = 'hombre';
  hombre.edadPromedio = 66;
  hombre.reproduccion = 'sexual';
  hombre.alimento = 'carnes, vegetales';
  hombre.bioma = 'terrestres, vegetacion';
  print("""
  animal 1
  El nombre del conejo es : ${conejo.nombre}.
  El promedio del conejo es: ${conejo.edadPromedio} años. 
  El tipo de reproduccion del conejo es: ${conejo.reproduccion}.
  Se alimenta de: ${conejo.alimento}.
  los conejos habitan en los: ${conejo.bioma}.
  animal 2 
  El nombre es: ${leon.nombre}.
  La edad promedio es: ${leon.edadPromedio} años. 
   El tipo de reproduccion del leon es: ${leon.reproduccion}.
  s Los leones e alimenta de: ${leon.alimento}.
  los leones habitan en: ${leon.bioma}
  animal 3
  El nombre es: ${hiena.nombre}.
  La edad promedio es: ${hiena.edadPromedio} años. 
   El tipo de reproduccion de la hiena es : ${hiena.reproduccion}.
  Las hienas se alimenta de: ${hiena.alimento}.
  las hienas  habitan en: ${hiena.bioma}
  animal 4
  El nombre es: ${hombre.nombre}.
  La edad promedio es: ${hombre.edadPromedio} años. 
  El tipo de reproduccion del hombre es: ${hombre.reproduccion}.
  El hombre se alimenta de: ${hombre.alimento}.
  el hombre habita en: ${hombre.bioma}
  """);
  
  
}

class Animal{
  String? nombre;
  int? edadPromedio;
  String? reproduccion;
  String? alimento;
  String? bioma;
}
class Hervivoro extends Animal{
  String tipo = 'Hervivoro';
}
class Conejo extends Hervivoro{}
class Carnivoro extends Animal{
  String tipo = 'Carnivoro';
  
}
class Leon extends Carnivoro{}
class Hiena extends Carnivoro{}
class Omnivoro extends Animal{
  String? tipo = 'Omnivoro';
}
class Hombre extends Omnivoro{}
```