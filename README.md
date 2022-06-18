# Emtech_Ejercicio4

productos= [ [1, "maiz grano", 285.55] ,
[2,"Pepino",334.72],
[3,"Tomate verde",129.00]
  ]

envio = 1500

ID = int(input("ID del producto: "))
if (ID >= 1):
  ID = ID-1
else:
  print("ID invalido")

productos = productos[ID]

cajasParaVender = int(input("Cantidad de cajas: "))

producto = productos[1]
precio = int(productos[2])

if(cajasParaVender <= 100):
  totalVenta = (precio * cajasParaVender + envio)
  print("Realizará una compra de 100 cajas o menos,     con un precio por envio de: " + str(envio))
  print("PRODUCTO:" + str(producto) + " PRECIO: " +       str(precio) + " TOTAL: " + str(totalVenta))

else:
  totalVenta = (precio * cajasParaVender)
  print("PRODUCTO:" + str(producto) + " PRECIO: " + str(precio) + " TOTAL: " + str(totalVenta))


