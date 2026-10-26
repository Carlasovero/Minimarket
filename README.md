# Proyecto Minimarket
## Inventario, carrito de compras
**Bibliotecas usadas: Pandas, ipyWidgets**
### El archivo esta dividido en cinco celdas. 
## 1era Celda "Importamos el inventario con Pandas"
## 2da Celda  "Funciones básicas del carrito
  *a)Def Buscar productos b) Def Agregar al carrito c)Def quitar del carrito e)Def calcular total d)Def mostrar carrito*
## 3era Celda "Componentes de la Interfaz" importamos ypiwidgets (Titulos, Botones, salidas y mensajes)
## 4ta Celda "Conexión de los botones con las funciones"
  *a)Def acción limpiar botón b)Def acción buscar botón c)Def acción agregar botón d) Def acción mostrar botón e)Def acción quitar botón f)Def vaciar boton.*
## 5ta Celda "Organizacion y visualizacion" (Aqui definimos el orden, el color de las cajas de cada una de los botones, apariencia y mostramos en Display)
`print (def buscar_productos(inventario, texto, categoria):

    if texto != '':
        nombres = inventario['nombre'].str.lower()
        inventario = inventario[nombres.str.contains(texto.lower())]

    if categoria != 'Todas':
        inventario = inventario[inventario['categoria'] == categoria]

    return inventario)`
