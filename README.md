# SGE04Formulario

Se trata de realizar una página para gestionar la ficha del empleado en la empresa **Empresa S.A** con la
apariencia que se indica para dispositivos small y superiores, y en la siguiente para dispositivos extra
small. A partir de menos de 400px deben aparecer scrollers.

La fecha de la cabecera se corresponde con la fecha actual en que se muestre la página. Los campos
que se pueden introducir son los que se muestran con los siguientes requerimientos( en negrita
aparece el nombre del campo para el formulario):


* El campo **nif** tendrá una longitud de 9 caracteres y solo permitirá la introducción de números y letras mayúsculas, siendo estas letras las que pueden aparecer en un nif. Antes de enviar se comprobará que es un nif correcto. Es campo obligatorio.
* El **nombre** tendrá una longitud máxima de 30 caracteres y solo se permitirá la entrada de letras del alfabeto español. Es campo obligatorio.
* El campo **apellidos** tendrán una longitud máxima de 50 caracteres y solo se permitirá la entrada de letras del alfabeto español. Es campo obligatorio.
* El campo **telefono** tendrá una longitud de 9 dígitos (solo se aceptará la entrada de estos) y no es campo obilgatorio, pero si aparece ha de contener nueve dígitos.
* El campo **fechaAlta** tiene formato aaaa/mm/dd. Se podrá introducir un dígito o dos tanto en el día como en el mes. En el inicio aparecerá la fecha actual. Deberá ser una fecha válida y es campo obligatorio.
* El campo **eMail** tendrá una longitud máxima de 200 caracteres, de los cuales 50 serán visibles y se comprobará que sea un e-mail correcto sintácticamente, no que exista de verdad. No es campo obligatorio.
* El campo **sexo** del empleado se seleccionará de dos botones de opción marcados con V o Hque son los valores que se transmiten. El valor al cargar la página será V
* El **estadoCivil** de casado se seleccionará a través de un checkbox. Se enviará el valor C si está seleccionado
* El campo **numeroHijos** deberá tener valores entre 0 y 20. No es campo obligatorio.
* La *provincia* se seleccionará de una lista desplegable en la que aparecerán las provincias que componen Castilla y León que es donde está implantada la empresa, es decir, Ávila, Burgos, León, Palencia, Salamanca, Segovia, Soria, Valladolid y Zamora. Los valores que se envían son respectivamente 0,1... 9. La provincia seleccionada al incio será Salamanca
* La *localidad* se seleccionará de una lista desplegable en la que aparecerán las localidades que se refieren a continuación en función de la provincia seleccionada:
1. Ávila: Arévalo, Ávila, Arenas de San Pedro, Madrigal de las Altas Torres (0 a 3)
2. Burgos: Aranda de Duero, Briviesca, Burgos, Lerma (0 a 3)
3. León: Astorga, La Bañeza, León, Ponferrada, Valencia de Don Juan (0 a 4)
4. Palencia: Aguilar de Campoo, Palencia, Herrera de Pisuerga (0 a 2)
5. Salamanca: Alba de Tormes, Béjar, Ciudad Rodrigo, Ledesma, Peñaranda de Bracamonte, Salamanca, Tamames (0 a 6)
6. Segovia: Segovia (0)
7. Soria: Almazán y Soria (0 y 1)
8. Valladolid: Medina del Campo, Olmedo, Peñafiel, Simancas y Valladolid (0 a 4)
* La localidad seleccionada al inicio será Salamanca
* Los valores entre paréntesis son los valores que han de enviarse al servidor en función de la localidad seleccionada, es decir si se selecciona La Bañeza se enviará un 2 en el campo provincia y un 1 en el campo localidad.
* El campo **nombreBanco** tendrá una longitud máxima de 30 caracteres. No es campo obligatorio.
* El campo **nombreSucursal** tendrá también una longitud máxima de 30 caracteres. No es campo obligatorio.
* El campo **numeroCuenta** tendrá una longitud máxima de 23 caracteres y se corresponderá con el formato xxxx-xxxx-xx-xxxxxxxxxx siendo las x dígitos entre 0 y 9. No es campo obligatorio pero si se incluye ha de tener ese formato. Deberá comprobarse que es un número de cuenta válido.


Se realizará filtrado de carácter y filtrado de campo según los requerimientos anteriores. Se
personalizarán los mensajes de error y se hará uso de los nuevos atributos, métodos y propiedades
ofrecidos por HTML5 en cuanto a validación de campos.
Cuando se pulse el botón de enviar, en caso de superar tales comprobaciones se procederá el envío de
los mismos a la dirección [link](http://www.empresasa.es/fabrica/gestionFicha.php) mediante el método
post.
El contenido de las cajas quedará seleccionado de forma automática al coger el foco.
