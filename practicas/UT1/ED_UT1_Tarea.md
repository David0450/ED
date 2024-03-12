# Especificación de Requisitos Software
En la actualidad existen una gran variedad de aplicaciones de compra online con efectivos sistemas de búsqueda, el problema reside en los pequeños negocios, que se ven opacados en estos sistemas de búsqueda. Es por esto que vamos a desarrollar un software específico para SmallStore que ayude a este tipo de comercios, un sistema de búsqueda.

## Alternativas existentes

### Amazon
#### *Puntos fuertes:*
- **Opción Amazon:** Los productos tienen un sello de Amazon que garantiza la calidad del producto.
- **Pequeños negocios:** Los productos provenientes de pequeños negocios vienen etiquetados como tal.
  
#### *Puntos débiles:*
- **Nombres de productos saturados:** Los características de los productos están en su mayoría en el propio nombre de este.
- **Etiquetas:** En algunas búsquedas no hay posibilidad de especificar más con etiquetas. Existe este problema por ejemplo al buscar "mando", el buscador te mostrará mandos de consola y no hay alguna etiqueta que te permita buscar otro tipo de mando.
  
### Shein
#### *Puntos fuertes:*
- **Variedad de etiquetas:** A la hora de buscar un producto existe una gran variedad de etiquetas que ayudan a especificar más la búsqueda.
- **Recomendaciones:** El software tiene apartados con productos recomendados para el usuario en función de sus compras previas, incluso le ofrece descuentos para estos productos.

#### *Puntos débiles:*
- **Sistema de tallas irregular:** En la aplicación se utilizan varios sistemas de tallas para un mismo tipo de producto e incluso la talla real puede no llegar a concordar con la especificada.
- **Sello de calidad:** No existe un sello de calidad Shein.
- **Recogida de productos:** No hay posibilidad de ir al negocio que vende el producto para comprarlo.

## Descripción del Software

Se trata de un sistema de búsqueda de productos para la aplicación SmallStore donde el usuario podrá buscar el producto deseado dentro de una lista de tiendas, consultar la información y reseñas sobre el producto y la tienda y programar pedidos para su recogida en tienda.

En nuestro software, los negocios podrán registrarse y dar a conocer su oferta de productos, recibir feedback sobre sus servicios y métricas que los ayuden conocer mejor su desempeño en la app.

## Lista Inicial de Requisitos

### Requisitos Funcionales

- **RF-1 Gestión de búsquedas**
  - RF-1.1. Filtros: los resultados han de poder ser filtrados por nombre, categoría, precio, calificación de la tienda y distancia desde la ubicación del usuario.

- **RF-2 Gestión de pedidos**
  - RF-2.1. Programación: deberá ser posible programar la recogida de un producto en la tienda deseada.
  - RF-2.2. Pagos: a la hora de pedir, los pedidos podrán ser pagados por adelantado dentro de la aplicación.

- **RF-3 Gestión de productos**
  - RF-3.1. Disponibilidad: el usuario podrá pedir que se le notifique cuando un producto esté disponible en la tienda que seleccione.
  - RF-3.2. Lista de favoritos: los productos pueden ser añadidos a una lista de favoritos del usuario para futuras compras.

- **RF-4 Gestión del negocio**
  - RF-4.1. Registro: los negocios podrán registrarse dentro de la aplicación.
  - RF-4.2. Estadística: los negocios han de poder consultar métricas y estadísticas sobre el rendimiento de este.
  - RF-4.3. Dirección: los usuarios podrán obtener direcciones y mapas para llegar a la tienda seleccionada.

- **RF-5 Gestión de reseñas**
  - RF-5.1. Comentarios: los usuarios tendrán la posibilidad de opinar y consultar las opiniones de un producto a modo de comentarios y calificaciones.
    - RF-5.1.1. Respuesta: los comentarios y reseñas podrán ser contestados tanto por usuarios como por negocios.

- **RF-6 Gestión de usuario**
  - RF-6.1. Registro: los usuarios podrán registrar su perfil con sus datos personales (nombre, apellidos, teléfono, correo y contraseña) y, si lo desean, sus datos bancarios.
  - RF-6.2. Modificación: los datos del perfil del usuario podrán ser editados por este.
  - RF-6.3. Eliminación: los usuarios tendrán la posibilidad de eliminar su perfil.

### Requisitos No Funcionales

- **RNF-1. Seguridad**
  - RNF-1.1. Se requerirá un teléfono para registrar una cuenta.
  - RNF-1.2. El usuario no podrá registrar dos cuentas con un mismo teléfono.
  - RNF-1.3. Si se detecta un inicio de sesión en otro dispositivo se notificará al usuario mediante correo electrónico.
  - RNF-1.4. El sistema debe proteger la información confidencial de los usuarios y garantizar la integridad de los datos.

- **RNF-2. Rendimiento**
  - RNF-2.1. El volumen de usuarios y consultas simultáneas no debe afectar al rendimiento del software.
  - RNF-2.2. Las búsquedas deben ser rápidas y eficientes, sin demoras significativas.
  - RNF-2.3. El software debe estar disponible 24/7.
  - RNF-2.4. El sistema debe poder utilizarse en distintos dispositivos y navegadores web.

- **RNF-3. Interfaz**
  - RNF-3.1. El software debe tener una amplia variedad de opciones de lenguaje.
  - RNF-3.2. La interfaz debe ser fácil de usar para los usuarios.
  - RNF-3.3. Los menús deben poder ser claramente legibles, sin una saturación de elementos.

### Requisitos de Información

- **RI-1. Usuario**
  - Nombre
  - Apellidos
  - Correo
  - Contraseña
  - Ubicación
  - Datos bancarios
  - Teléfono

- **RI-2. Producto**
  - Descripción
  - Foto
  - Tiendas con stock
  - Reseñas
  - Características
  - Etiquetas

- **RI-3. Reseña**
  - Autor
  - Fecha de publicación
  - Likes
  - Producto/tienda referido

- **RI-3. Tienda** 
  - Nombre
  - Inventario
  - Estadísticas
  - Reseñas
  - Dirección
  - Foto

## Glosario de términos
- **Etiquetas:** Clave asignada a un dato almacenado en un repositorio.
- **Software:** Conjunto de programas y rutinas que permite al ordenador realizar determinadas tareas.
- **Requisitos funcionales:** Define las funciones del sistema de software o sus componentes.
- **Requisitos no funcionales:** 
- **Requisitos de información:** Lista todos los datos que han de saberse sobre un apartado del software.
- **Mando:** Dispositivo que se utiliza para controlar o manejar un aparato electrónico o un sistema
- **Consola:** Dispositivo electrónico diseñado específicamente para jugar videojuegos.
- **Sello de calidad:** Los sellos de calidad ofrecen cierta garantía a los clientes de que los productos cumplen con unos estándares mínimos de calidad.
- **Reseña:** Pequeño comentario valorativo de un producto, servicio, libro, película u otro tipo de contenido.
- **Filtro:** Característica o criterio específico utilizado para seleccionar, evaluar o categorizar un producto.
- **Métricas:** Datos que responden a diversos parámetros y sirven para analizar algo.