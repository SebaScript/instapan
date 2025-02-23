# Instapan ©

## Implementación menú horizontal - Juan Sebastian García - Desarrollo Web Grupo 61

## Detalles del HTML (index.html)

1. **Head**: Se utiliza el head por defecto y se vincula con el archivo css "styles.css".

2. **Barra de Navegación**
   - Se divide en tres secciones:
     - **Izquierda**: Contiene el logo y el título "Instapan ©".
     - **Centro**: Contiene el menú de navegación.
     - **Derecha**: Contiene un ícono de usuario en SVG.

3. **Contenido Principal**
   - La sección `<main>` simplemente contiene el logo de Instapan ©.

## Detalles del CSS (styles.css)

1. **Reset Global y Fuente**
   - Se reinician márgenes y padding para todos los elementos, y se establece `box-sizing: border-box` (Lo aprendí hace tiempo y ya lo hago siempre).
   - Se aplica la fuente **Comic Sans** para todo el documento en el `body`.

2. **Barra de Navegación**
   - La clase `.navbar` se define como un contenedor flex con `justify-content: space-between` para distribuir los elementos con un espaciado uniforme entre ellos.
   - Se le da un width del 33% a cada uno de los 3 contenedores (left, center y right) para que cada uno ocupe el mismo espacio dentro del contenedor navbar.
   - Al left, se le asigna la propiedad display: flex para que el logo y el título se muestren uno al lado del otro.
   - Al center, se le asigna la propiedad display: flex para aplicarle justify-content: center para que el contenedor interno (menu) quede centrado. Al ul dentro del contenedor menu, se le aplica display: flex para que los elementos de la lista se muestren uno al lado del otro.
   - Al right, se le aplica display: flex para aplicarle justify-content: flex-end, ya que por defecto, el ícono que está dentro del contenedor, se alinea a la izquierda, entonces con flex-end, se alinea a la derecha.
   - De resto, son estilos más estéticos, como el hover en los elementos de la lista, los padding, etc.

3. **Contenido Principal**
   - La clase `.content` utiliza Flex para centrar la imagen de pan tanto horizontal como verticalmente y se le asigna que ocupe todo el tamaño de la pantalla.
