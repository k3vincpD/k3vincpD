# Clase 1
---
git + markdown

## Clase dedicada al entendimiento del uso del github y el uso del markdown.

### Cortado matricial en el visual studio funciona con: shift + alt.

------
## Tipos de titulos 
### titulo 1=#
### titulo 2=##  
### titulo 3=###
### titulo 4=####
---
# comandos del git que he utilizado 

### $ git config --global user.name "Mona Lisa"

### $   git config --global user.name "Kevin Cepeda"

### $  git username
### $   git config --global user.email kevin.llugcha@gmail.com
### $  git version
### $  git version
### $  pwd
### $  git status
### $ git init
### $ history
---
# Clase 2  
## Introduccion a C 
 ### Primer programa realizado en C 

### El comando ($ git push) es para enviar de la nube 
### El comando ($ git pull) es para traer a la nube
# Pasos al entrar al visual studio code 
### Usar el comando (git version) para ver si trabaja el git 
### Usar el comando (gcc --version) para ver si esta trabajando el c 
### Usar el comando (pwd) para saber en que erachivo estamos trabajando.
### Usar el comando  (echo *.el archico que quiero que sea ignorado >> .gitignored) 

# <strong> Codigo realizado 

    ``` C
     #include <stdio.h>

    void main ()
    {
        printf("hello word :)\n");
    }
    ```

# Clase 3
---
Numeros enteros definidos: int
Letras o caracteres definidos: char
Numeros reales o en comaflotante: float o double 
# void
- procedimiento 
- lineas de codigo que no debuelven nada 
# return 
- Si devuelve
## <strong> **Diferencias entre error,bug,issue**
 ***Error*** :
 ### Puede ser del compilador osea un error sintactico o sintactio o tambien puede ser un error lógico es decir por ejemplo una division entre 0, el error puede hacer que el pogrma muera o no arranque.
 ***Bug*** :
 ###   Son errores de sistema que pueden ser utilizados para corromper el programa 
 ***issue*** :
 ### Algo que falla perro el programa puede seguir corriendo, __se puede convertir en un error__
 # Clase 4
 ## __Algoritmia__ 
 Proceso antes de programar en la la aplicacion o solucionar errores.
 - Paso 1
    
    _Pseudocódigo_: se realiza un código sencillo y fácil de entender.
- Paso 2
   
    _Flujograma_: Se esquematiza el codigo para entender como va a funcionar .
- Paso 3

    _Codificación_: 

- Paso 4

    _Trace_: Se corre el programa y se corrige posibles errores.
# clase 5
## Punetos y arrays 
### Arrays 
- Es una bariable estructurada donde cada elemento se alasena de forma consecutica en la memoria ejm:
### "int a[10]" donse se almacena 10 enteros.

- en ejemplo anterios se declara un  array de 10 punteros

## Como se programa en c?
1. Se llama las librerias 
2. se declaran variables globales, y se declaran procedimientos 
3. bloque principal 
# Tipos de dato 
![](https://dc722jrlp2zu8.cloudfront.net/media/uploads/2020/10/20/pildora-02-captura-2.jpg)
# *Bucles*
## *for >strong<>*
### Repite el bloque de instrucciones un número prederminado de veces. 
## *while* 
### Un bucle while permite repetir la ejecución de un grupo de instrucciones mientras se cumpla una condición
## *for while*
### Primero hace las cosas luego pregunta.
____
### Directorio de entrada es el src
### y el directorio de salida es el output para mandar a compilar con el git se hase asi en c:
  
 `gcc src/main.c -o output/main.exe`
 
 ### entonces seria de donde sale? nombre del programa.c -o a donde se ejecuta/nombre del archivo.exe
### (no se sube al git)
# ejemplo 
 ```C
 #include <stdio.h>

 int main(){
    int nrosigno=0;
    printf("ingrese numero:);
    scanf("i",%nrosigno);
    for (int i+0;i < nrosigno;i++){
        printf("+);
    }
    return 0;
 }
```
el bucle for va a hacer euq imprima + tanto como se le haya asignado
***
# Clase 6
## *Series*
*PROCEDIMIENTO* siempre se usa void debe estar e accion verval.
despues se lleva al codigo principal.
## ejemplo
```C
void signosalternos(){
int nrterminos;
for (int i+0;i<nrtermnimos;i++)
{
    printf(+);
}
}
int main(){
    printf("ingrese numero:);
    scanf("i",%nrosigno);
    signosalternos();
}
```
## EJmplo de marco de cuadrado 
```C
#include <stdio.h>
int main()
    
{
    int n;
    printf("Escriba el tamaño del borde delcuadrado: ");
    scanf("%i", &n);
    printf("\n");
        for (int i = 1; i <= n; i++)
        {
            for (int j = 1; j <= n; j++)
            {
                if (i==1||i==n|j==1||j==n)
                {
                    if(i%2==0 || j%2==0)
                    printf("+");
                    else
                    printf("-");
                }
                else{
                    printf(" ");
                }
                
                
            }
            printf("\n");
        }
    
    return 0;
}
```
para segir para el programa se usa el debag, al momento de correr(no entendi);
***
# Clase 7 
## matrices  
## *en progracacion las matrices empiezan en 00*
se puede hacer mediante asignar fila por fila o todo de una sola 
ejemplo 
```C
#include <stdio.h>

void logomatiz()
{
    char mc [5 ][5 ]={
                        {'*','*','*','*','*'}
						,{'*','*','*','*','*'}
						,{'*','*','*','*','*'}
						,{'*','*','*','*','*'}
						,{'*','*','*','*','*'}
                    }
                    
    
```
se usa el sytem("clear") o el system ("cls")para limpiar.

Para que imprima lineas y filas segun se pude hacer con el bucle for
## ejemplo 

```C
 #include <stdio.h>

void logomatiz()
{
    char mc [5 ][5 ]={
                        {'*','*','*','*','*'}
						,{'*','*','*','*','*'}
						,{'*','*','*','*','*'}
						,{'*','*','*','*','*'}
						,{'*','*','*','*','*'}
                    };
    char fila = sizeof(mc)/sizeof (mc[ 0]);
    char columa=sizeof(mc[0])/sizeof (mc[0][0]);
    char numerode= sizeof (mc)/sizeof(mc[0][0]);
	for (char  fi= 0; fi < fila; fi++)
	{
	for (char cu = 0; cu < columa; cu++)
		
			if((fi+cu)==3||cu==0||((3*fi)-(2*cu))==5||(4*fi)-(cu*3)==7)
				printf("%c \t", mc[fi][cu]);
			else
				printf ("\t");
		printf("\n");
	}
}
void main()
{
	//system("clear");
	logomatiz();
}
```
es decir la fila o columna debe cumplir condiciones que son agregadas al condicional if para que imprima y para eso se debe encontrar el metodo.
***
# Clase 8
Crear proyecto en c en que me ayude el visual studio siempre y cuando tenga la extencion **c/c++ project generator** si ausa el atajo en mi caso el comando __(ctrl+shift+p)__.

*Para crear libreria con lenguaje declarativo tambien comocid como heders(no se si este bien escrito).
 se crea un nuevo doc con terminacion.h donde se ba a crar codigo de manera general, y en el archivo.c se lo manda a llamar con
  #include "nombre del archivo"
ejemplo*

# poner imagen 

# Clase 9 

 **coreccion del workshop** 

# Clase 10
Archivos
##c
los archivos de texto terminan en .txt.
 para leer archivo:
```C++
void leerarchivo(string pathfile) {
    string s;
    ifstream f(pathfile);
    if(!f.isopen())
    cerr.<< "error de abrir el archivo"<< endl;
    else 
        do{
            getline(f,s);
            cot<<s<<endl;
        }while(!f.eof());
        f.close();
}
```
Recomendacion
copiar el nombre de las carpetas y pegar pra evitar errores.
depues en el int void se manda a llamar y se escrive de la sigiente manera
```C++
leer archivo(".\\files\\listado.txt");
```
el punto significa directorio raiz
despues va el nombre de la carpeta y por ultimo va el nombre del archivo.txt .
cons dos putnos me salgo ara buscar 
## Para sobreescribir el archivo 
```c++
void sobreescribir(string pathfile){
ofstream f;
f.open(pathfile, ios_base:: app);

f<<"primera linera\n">>;
f<<"segunda linera\n">>;
f<<"tercera linera\n">>;
f.close();
}
```
el app agrega y si en vez del app se pone out crea y remplaza todo.
# Clase 11


