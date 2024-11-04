# Store API

## Descripción
Esta API permite realizar operaciones de consulta sobre productos de una tienda. Los usuarios pueden filtrar, ordenar y paginar los productos según varias propiedades.

## Tecnologías utilizadas
- **Node.js, Express, MongoDB, Mongoose**

## Funcionalidades
- GET /products
Ruta dinámica que permite filtrar y ordenar productos usando parámetros de consulta.

## Parámetros de consulta
- featured
      .Filtra productos destacados.
      .Ejemplo: ?featured=true
- company
      .Filtra los productos por la compañía fabricante.
      .Ejemplo: ?company=ikea
- name
      .Filtra los productos cuyo nombre contiene una palabra específica, sin importar mayúsculas o minúsculas.
      .Ejemplo: ?name=shelf
- sort
      .Ordena los productos por las propiedades especificadas (por ejemplo, price, name). Se pueden especificar múltiples campos separados por comas.
      .Ejemplo: ?sort=price,name
- fields
      .Permite seleccionar campos específicos que se mostrarán en los resultados.
      .Ejemplo: ?fields=name,price
- numericFilters
      .Filtra los productos por rangos en propiedades numéricas como price y rating. Usa operadores (>, >=, <, <=, =) y combina filtros con comas.
      .Ejemplo: ?numericFilters=price>30,rating>=4
- page y limit
      .Paginación de resultados. page especifica la página y limit la cantidad de resultados por página.
      .Ejemplo: ?page=2&limit=10
  

## Instalación

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/DiegoBottegoni/store-api.git

2. Instalar las dependencias:

   ```bash
   npm install
   
3. Iniciar el servidor:

   ```bash
   npm run dev
   
