Precisiones del código:
1.- Opera en R Studio, en formado RMD.
2.- La asignación de género se da partir de la identificación de nombres coincidentes con un banco de nombres con el género asignado anteriormente.
3.- El banco de nombres fue construido desde 0. Como referencia, al correr el código API "genderizer", además de que tiene una utilidad limitada por temas de suscripción, no contemplaba que en Perú la variedad de nombres es mucho mayor. De esta manera, se decició crear un banco de nombres con nombres presentes en la sociedad. Se recomienda tomar el mismo criterio para otros países o contextos.
4.- Para evitar que los nombres usados también como apellidos puedan arrojar resultados erróneos, se codificó que se asigne el género mayoritario (es decir, si una persona se llama María Antonieda, y se apellida Manuel Díaz, R le asignará femenino al identificar 2 nombres femeninos por sobre uno masculino).
5.- El banco podría ser más grande. Se preparó en un lapso de una semana a partir de bases de nombres con decenas de filas. Es probable que falten nombres comunes.

Guía para usar el código:
1.-El archivo "Bancodenombres" es, justamente, el banco donde se encuentra cada nombre con el género asignado previamente. Contiene 1800.
2.-El archivo "NombresyApellidos" debe contener los nombres y apellidos (o en desorden) a analizar. Solo se debe usar la primera columna. Considerar que solo la celda A1 no debe cambiarse, debe mantenerse en "Nombres".
3.- Es necesario establecer el directorio de trabajo para que se importen los archivos. En el código se encuentra la ruta con el teclado para ello.
4.- Luego de correr todo el código, se habrá actualizado el archivo "RESULTADO", contendrá la misma columna de nombres y apellidos a analizar, con el género en la columna de al lado.
5.- Considerar que si no se hallaron coincidencias, R dejará vacía la fila correspondiente (no la eliminará).
