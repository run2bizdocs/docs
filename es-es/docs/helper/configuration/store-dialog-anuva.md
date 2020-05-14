Title: Almacenar informaciones en los diálogos
# Almacenar informaciones en los diálogos

Muchas veces el usuario durante un diálogo, nos proporciona información que será utilizada en otro momento para una mejor comprensión del interés del usuario. Helper reconoce esta información como Atributos.

En una conversación, por ejemplo, en que el usuario pide que Helper informe qué restaurantes italianos existentes a menos de 10 km de distancia, podemos tener tres atributos: tipo de establecimiento, categoría y distancia.

En este caso, creamos Atributos que sean capaces de almacenar esta información para responder de forma más precisa al usuario.
Los tipos de atributos definen el formato de la información que se puede guardar en el mismo. Helper trabaja con los siguientes tipos:

 - Text slot: en el que puede agregar valores de tipo de texto;

 - Boolean slot: utilizado para valores reconocidos como true o false;

 - Categorical slot: utilizado para almacenar un valor de una lista predefinida;

 - Float slot: donde podemos añadir valores numéricos con límites mínimo y máximo;


!!! Abstract "NOTA"
    
    Observe que no sería posible crear interés que representase todas las combinaciones 
    posibles para esas tres informaciones. En este caso lo ideal sería utilizar los atributos.


Procedimiento
------------

1. Acceder al menú “Atributos”;

2. Hacer clic en "Nuevo";

3. Completar el nombre y el tipo de atributo;

4. Informar a los demás campos necesarios de acuerdo con el tipo y hacer clic en "Guardar".


!!! tip "About"

    <b>Product/Version:</b> 4biz | Helium &nbsp;&nbsp;
    <b>Updated:</b>11/03/2020
