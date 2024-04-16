# Autor:
- Apellido: Pacheco
- Nombre: Cristian Ezequiel

# Compilador
- Version Compilador : gcc (Rev3, MSYS2) 13.2.0
- Compilada con C Version : C18

# Aclaraciones
Para simplificar el proceso he creado un archivo makefile que compila y crea el archivo "output.txt"

El comando que se utiliza es
- make create_txt

``` Makefile
    SOURCE = hello.c
    BIN = hello.exe
    TXT = output.txt
    CC = gcc
    CFLAGS = -std=c18

    $(BIN): $(SOURCE)
        $(CC) $(SOURCE) -o $(BIN) $(CFLAGS)

    run: $(BIN)
        ./$(BIN)

    create_txt: $(BIN)
        ./$(BIN) > $(TXT)

    clean:
        rm -f $(BIN) $(TXT)
```

Comandos extra
- make clean (permite eliminar los archivos creados)
- make run (ejecuta el programa hello.exe)

# Enunciado
1. **Cuenta en GitHub**
    
    a. Si no tiene, cree una cuenta GitHub.
    
    b. Si no lo hizo, asocie a su cuenta GitHub el email @frba y verifíquelo. Es posible asociar más de una cuenta email a una cuenta GitHub.
    
    c. Si no lo hizo, indique que su cuenta email @frba es pública. Esto permite a la cátedra encontrar a los estudiantes. Si por temas de privacidad prefiere no tener como pública esa dirección, puede cambiarla al final del proceso.
    
2. **Repositorio público para la materia**
    
    a. Cree un repositorio público llamado SSL.
    
    b. En la raíz de ese repositorio, escriba el archivo readme.md que actúa como front page del repositorio personal.
    
    c. Cree la carpeta 00-CHelloWorld.
    
    d. En esa carpeta, escriba un segundo archivo readme.md que actúa como front page de la resolución.
    
3. **Compilador**
    
    a. Seleccione, instale, y configure, y pruebe un compilador C11 ó C18. Los más osados pueden buscar un compilador que soporte C2x.
    
    b. Registre los resultados anteriores de la siguiente manera:
        
    1. Indique en el readme.md el compilador seleccionado.
        
    2. Pruebe el compilador con un programa hello.c que envíe a stdout la línea Hello, World! o similar.
        
    3. Ejecute el programa y verifique que la salida es la esperada.
        
    4. Ejecute el programa con la salida redireccionada a un archivo output.txt; verifique su contenido.
            
4. **Publicación**
    Publique el trabajo en el repositorio personal SSL la carpeta 00-CHelloWorld con readme.md, hello.c, y output.txt.



