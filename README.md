Práctica de 3 usuarios
Explicación
Esta práctica se desarrollará en grupos de 3 participantes. Existen 3 roles (A, B y C) en la
práctica, y cada participante deberá desempeñar uno de los roles. Tras haberla concluido una
primera vez, se rotarán los roles y se repetirá la práctica. Así hasta que cada participante haya
desempeñado los 3 roles.
Es necesario montar un repositorio conjunto en GitHub y un equipo de trabajo de 3 personas.
Todas ellas tienes que tener todos los privilegios sobre el repositorio.
Cada integrante deberá seguir los pasos se citan a continuación. Finalmente, detalla todos los
pasos realizados por cada miembro.
En un repositorio remoto, es aconsejable tener al menos dos ramas, master (nombre por
defecto), que representa la versión en producción; y develop, donde se van fusionando las
contribuciones de los colaboradores hasta que se obtiene una versión definitiva que se pueda pasar a
producción, es decir, fusionar a master. En resumen, en master siempre estará la última versión de
un producto susceptible de poner en producción.
Alumno A
1. Crea un repositorio en GitHub, llamado facturas, que contenga un README.md y un
archivo de licencia. Utiliza las plantillas que te ofrece GitHub para seleccionar el tipo de plantilla
para el archivo .gitignore que mejor se ajuste a un proyecto Java y créalo también.
2. Crea en local un proyecto Java, que sea también un repositorio de Git, con nombre facturas
y súbelo al repositorio remoto a la rama master.
3. Crea en local una rama alumnoA para trabajar tu.
4. Se te ha encargado crear una interfaz, que será implementada por todas las facturas. Se
llama Ifactura.java, y contiene tres métodos:
void cambiarEstado(Estados estado);
float getTotal();
float getCantidadIva();
5. Crea una clase enumerado llamado Estados.java, que se llame Estados y que tenga como
valores Aprobada, Pendiente y Cobrada.
6. Crea un commit para añadir el enumerado.
7. Crea un commit para añadir la interfaz.
8. Vuelca el trabajo a la rama master y borra la rama que has usado.
9. Cuando tengas en tu repositorio la clase Factura que ha implementado tu compañero, crea
una rama para corregir un bug referente a la propiedad estado de la clase Factura.
10. Corrige el bug: cambia la visibilidad de public a private. Haz un commit con esta
corrección.
11. Vuelca la modificación a la rama master y borra la rama que has usado.
12. Cuando esté lista la primera puesta en producción mediante la rama master, bájala a tu
repositorio local.
Alumno B
1. Se te ha encargado empezar el esqueleto de la clase Factura. Crea una rama para ello, 
llamada alumnoB, a partir de la versión actualizada de master.
2. Crea un archivo llamado Factura.java para la clase Factura, con los siguientes miembros
además del método main():
public int num;
public float base;
public float tipoIva;
public Estados estado;
3. Comenta la línea de la propiedad "estado", porque aún no está implementado el enumerado
Estados.
4. Crea un commit con la clase.
5. Vuelca el trabajo a la rama master y borra la rama que has usado.
6. Cuando tengas la interfaz y el enumerado (desarrollada por otro compañero) en tu
repositorio local, crea una rama para aplicar los siguientes cambios.
7. Descomenta la línea que comentaste en el punto 3 y haz un commit con esta modificación.
8. Implementa la interfaz en tu clase Factura (no hace falta que añadas nigún código a los
métodos, simplemente déjalos en blanco).
9. Crea un commit con este último cambio.
10. Corrige un bug: cambia la visibilidad de la propiedad estado a protected. Haz un commit
con esta corrección. Si más adelante hay un conflicto con algún compañero del equipo, ésta es la
visibilidad que tiene que quedarse definitivamente.
11. Vuelca el trabajo a la rama master y borra la rama que has usado.
12. Eres el encargado de preparar la primera versión que irá a producción:
13. Añade un tag al último commit de master con la versión 0.1.0.
Alumno C
1. Se te ha encargado implementar algunos métodos de la clase Factura y un enumerado de
estados. Empieza creando una rama llamada alumnoC para el enumerado a partir de la versión
actualizada de master.
2. Crea un archivo llamado Estados.java para un enumerado, que se llame Estados y que tenga
como valores Aprobada, Pendiente, Cobrada y Anulada.
3. Si más adelante aparece este mismo enumerado en la rama de algún compañero del equipo
y hay conflictos, éstos son los cuatro valores definitivos que tienen que quedar.
4. Crea un commit para añadir el enumerado.
5. Vuelca el trabajo a la rama master y borra la rama que has usado.
6. Cuando tus compañeros hayan añadido estos dos métodos a la clase Factura,
impleméntalos:
getTotal();
getCantidadIva();
7. Crea un commit con los cambios.
8. Vuelca el trabajo a la rama master y borra la rama que has usado.
9. Sube los cambios de develop al repositorio remoto.
10. Cuando esté lista la primera puesta en producción mediante la rama master, bájatela a tu
repositorio local.
