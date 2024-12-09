# talento_tech

Proyecto integrador del curso de Front-End JS de Talento Tech para la comisión C24232.

En esta etapa se agregan funcionalidades JavaScript, un Carrousel de bootstrap y el consumo de una API(generada para este proyecto).

La API está hecha en PHP, la cual accede por método GET a los productos y sus imágenes de esta manera:
https://www.binariosistemas.com.ar/API_PHP/controller/producto.php?op=GetAllProd
El cual devuelve los productos, sus categorías, imágenes y precios en un JSON que tiene el siguiente formato:

    "id": "1",
    "titulo": "Abrigo 01",
    "descripcion": "Descubre nuestra selección de abrigos para hombres, diseñados para combinar estilo y funcionalidad en cualquier temporada. Encuentra desde elegantes abrigos clásicos para ocasiones formales hasta cómodas parkas y chaquetas casuales para el día a día.",
    "imagen": "https://www.binariosistemas.com.ar/API_PHP/views/img/abrigos/01.jpg",
    "categoria": {
        "nombre": "Abrigos",
        "id": "1"
    },
    "precio": "1000"

https://www.binariosistemas.com.ar/API_PHP/controller/categoria.php?op=GetAllCat
El cual devuelve las categorías en un JSON que tiene el siguiente formato:

{
    "id_categoria": "1",
    "nombre_categoria": "Abrigos"
  },

  
El proyecto también posee una página de carrito de compras que guarda los elementos en el LocalStore, el cual posee alertas con la librería SweetAlert2 y Toastify.

Acabo de realizar una actualización en la API y ahora también trae una descripción genérica del producto.
