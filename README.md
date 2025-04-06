# Escritura de Archivo de Texto

# Abrimos el archivo "my_notes.txt" en modo escritura ('w')
archivo = open("my_notes.txt", "w")

# Escribimos tres líneas de texto
archivo.write("Primera nota: hoy aprendí a escribir archivos en Python.\n")
archivo.write("Segunda nota: también aprendí a leerlos línea por línea.\n")
archivo.write("Tercera nota: siempre debo cerrar el archivo después de usarlo.\n")

# Cerramos el archivo después de escribir
archivo.close()

# Lectura de Archivo de Texto

# Abrimos el archivo en modo lectura ('r')
archivo = open("my_notes.txt", "r")

# Leemos línea por línea y mostramos cada una en consola
linea = archivo.readline()
while linea != "":
    print(linea.strip())  # .strip() elimina espacios y saltos de línea
    linea = archivo.readline()

# Cerramos el archivo después de leer
archivo.close()
