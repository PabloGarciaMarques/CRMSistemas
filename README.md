Python - CRM (Customer Relationship Management)
Objetivos
• Afianzar y profundizar los conocimientos de programación en general y de programación en
Python en particular.
• Profundizar conocimientos en los softwares ERP (Enterprise Resource Planning), y
concretamente en el módulo CRM (Customer Relationship Management) de los mismos.

Consideraciones iniciales:
• Para la interfaz gráfica debes utilizar la librería TKinter (vista en clase). También puedes
utilizar PyQt, que es una adaptación de la biblioteca gráfica Qt para el lenguaje de
programación Python.
• Para implementar la base de datos puedes utilizar SQLite, MySql, PostgreSQL, etc, aquella
con la que más cómodo te sientas trabajando y/o te permita una mayor funcionalidad según
tus necesidades.
• El programa debe contar con una base de datos donde esté recogida la información de las
empresas que van a utilizar el CRM (nombre de empresa, correo electrónico y contraseña),
de tal manera, que por cada empresa que demos de alta en esta base de datos, se debe
crear una nueva base de datos, así logramos que cada empresa que implemente el CRM
tenga todos sus datos (los suyos propios y los de sus clientes) en su propia base de datos.

Funcionalidad del CRM
Deberás implementar un CRM (Customer Relationship Management) en Python con las
siguientes funciones y características:
1. Inicialmente, el programa presentará una pantalla para loguearse. Aquí se pedirá un nombre
de empresa, correo electrónico y una contraseña (habrá que confirmar la contraseña). Se
debe generar una nueva base de datos por cada registro que se cree en esta base de datos
inicial (base de datos con las diferentes empresas que poseen el CRM), así, cada empresa
utilizará su propia base de datos cuando acceda al CRM.
2. Una vez creada la empresa/empresas en la primera base de datos, cada empresa accederá
a su propia base de datos mediante el nombre de usuario y contraseña, y nos aparecerá el
CRM de la misma. En el CRM:
2.1. Inicialmente, nos debe aparecer un PIPELINE con al menos 4 fases para los productos
(NUEVO, CALIFICADO, PROPUESTA, GANADO), en el que nos aparezcan las distintas
oportunidades que se hayan generado en la empresa hasta ese momento en su estado
correspondiente. Además, desde el pipeline, como mínimo podremos:
2.1.1. Crear nuevos contactos (que serán clientes potenciales para nuestra empresa,
pudiéndose tratar también de otras empresas). Los campos mínimos para los
clientes serán: IDENTIFICADOR, NOMBRE, DIRECCIÓN (CALLE, CODIGO POSTAL,
CIUDAD, PAIS), TELÉFONO, PERSONA DE CONTACTO, CORREO ELECTRÓNICO Y
PORCENTAJE DE IVA (en el caso de que fuese un país extranjero).

2o CFGS Desarrollo de Aplicaciones Multiplataforma
Sistemas de gestión empresarial - Curso 2023-24 - Actividad 2o trimestre
Profesor: José María Martínez Tejero

A c t i v i d a d C R M - P y t h o n 2 T - S G E - P á g i n a 2 | 3
2.1.2. Crear nuevas oportunidades con los campos: ORGANIZACIÓN/CONTACTO,
OPORTUNIDAD, CORREO ELECTRÓNICO, TELÉFONO, INGRESO ESPERADO y
ESTADO para esa oportunidad. Asimismo, se podrá cambiar el estado de las
distintas oportunidades desde el PIPELINE.
2.1.3. Dentro de cada oportunidad podremos crear nuevos presupuestos para nuestros
clientes o utilizar los ya creados. Al crear los presupuestos, si no existiese el cliente
o el producto deberemos poder crear los mismos (clientes y productos) desde el
presupuesto. Los campos mínimos para el presupuesto serán: IDENTIFICADOR,
CLIENTE, FECHA DE CREACIÓN, FECHA DE EXPIRACIÓN, PEDIDO. En pedido u oferta
es donde iremos ubicando los distintos productos del presupuesto. Además,
deberemos contar con dos campos más, SUBTOTAL (con la suma de los distintos
productos) y PLAZO DE ENTREGA del presupuesto.
NOTA: Un presupuesto podrá admitir uno o varios pedidos, dependiendo de cómo
diseñes la base de datos, y en un pedido podrá haber uno o varios artículos.
2.1.4. Debe existir también un inventario donde poder crear y/o modificar productos
para podérselos ofrecer a nuestros clientes. Los campos mínimos para los
productos serán: IDENTIFICADOR, PRODUCTO, DESCRIPCIÓN, STOCK, PRECIO
UNITARIO.

3. Todo (los datos de la empresa, clientes, artículos, pedidos, etc) deberán ser editables y
poderse modificar.

Presentación de la tarea
a) Debes realizar un informe en PDF de la práctica en el que deberás recoger todos los aspectos
del programa, como son las distintas fases del mismo (análisis, diseño y desarrollo). En estas
fases explicarás don detalle las distintas soluciones adoptadas (creación de la interfaz
gráfica, creación de la BBDD y su modelo relacional, etc). Respecto a la programación, es
indispensable utilizar clases y objetos y tener el código comentado. En el mismo informe,
en un anexo, debes recoger un pequeño manual de usuario de tu programa.
b) Debes realizar una defensa en clase de tu programa, por lo que deberás preparar una
presentación y demostración del mismo de 20 minutos de duración como máximo. Es
aconsejable que para esta tarea te apoyes en una presentación PowerPoint o similar.

Calificación
• Para que la práctica esté aprobada (un 5 / 10) deberán de funcionar todos los aspectos
anteriormente citados. A partir de ahí, la nota se complementará con el informe, la
presentación y las mejoras introducidas en la misma. Si el programa no funcionase en
alguno de los aspectos básicos anteriormente citados, la práctica se consideraría
SUSPENSA y el trimestre también.
• La nota de esta actividad corresponderá al 90 % de la evaluación, dejando un 5% a la
evaluación de la tarea CRUD y el 5 % a la evaluación de las distintas competencias
transversales y/o blandas.

2o CFGS Desarrollo de Aplicaciones Multiplataforma
Sistemas de gestión empresarial - Curso 2023-24 - Actividad 2o trimestre
Profesor: José María Martínez Tejero

A c t i v i d a d C R M - P y t h o n 2 T - S G E - P á g i n a 3 | 3

Posibles mejoras
• Introducir un logo en la base de datos de las empresas para que éste aparezca en el CRM de
las mismas.
• Posibilidad de mandar emails a contactos existentes y a otros posibles/futuros clientes.
• Al realizar un pedido u oferta, el programa deberá ser capaz de generar un documento de
texto en formato PDF con el pedido u oferta realizada para poder enviarlo a los clientes.
• Posibilidad de generar gráficos estadísticos de nuestras oportunidades, productos, clientes,
etc.
• Implementar una base de datos que estará alojada en un servidor Ubuntu (Ubuntu 20.04) a
la que deberás acceder desde el CRM.
• Etc.
