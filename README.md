## ANALISIS DEL REPOSITORIO
**Estructura del repositorio**

En la carpeta 'src' contiene una carpeta llamada components, la cual tiene los siguientes archivos:

Alert.jsx, AnimalCard.jsx, AnimalForm.jsx, AnimalList.jsx, DarkModeToggle.jsx, Layout.jsx, Loader.jsx.

Tambien contiene un HOOK, el cual tiene un archivo javascript: useFetchAnimal.js
tiene una carpeta Pages, que contiene el archivo farm.jsx, tiene otra carpeta llamada services que tiene un archivo javascript: animalsApi.js
y ya por ultimo tiene los archivos app.css, app.jsx, index.css, main.jsx.

**manejo del useeffect y usestate**

Lo que se hace en el proyecto es que se usan para conectar el API de mockapi, tambien para los filtros de busqueda ya que se renderizan y se validan

**implementacion tailwindcss**

Lo que hace tailwind en el proyecto es darle un diseño y una personalizacion muy profunda para que se vea atractiva.

## Cuestionario de 10 preguntas

**1.¿Cuál es la diferencia entre un componente presentacional y un componente de página en React?**

Bueno en la diferencia que tienen los dos es que uno se encarga en la parte estetica o apariencia e interaccion con el usuario es decir no tiene nada de logica y solo renderiza lo que es una interaccion con el usuario: un ejemplo puede ser: AnimalCard.jsx, Alert.jsx. En cambio el componente de la pagina tiene mas logica ya que se encarga de  obtener datos y manejar un estado global ya que tiene estados, ejemplos es que renderiza: loader.jsx, AnimalForm.jsx, AnimalList.jsx, etc.

**2. ¿Para qué se utiliza useState en el proyecto?**

El useState en el proyecto se utiliza es para que almacene valores mientras va cambiando la pagina con interacciones de usuario, por ejemplo se usa en animals y isLoadin que esta en el archivo Farm.jsx

**3. ¿Cómo se usa useEffect para cargar datos desde MockAPI al inicio?**

El useEffect se usa en farm.jsx, ya que se crea y se monta en el dom, despues se llama getanimals() en animalsApi.js, despues se mira si sale correcto todo o hay un error.

**4.¿Cómo maneja el proyecto los estados de loading, error y lista vacía? ¿Qué se muestra al usuario en cada caso?**

En el loading aparece: `<Alert variant="info">Cargando animales...</Alert>`

error: `<Alert variant="error">`

lista vacia: aparece no hay animales en la granja, ya que no tiene registrado obviamente

**5. ¿Qué significa que un formulario sea controlado en React?**

Significa que el valor de un input proviene de un useState, y que cualquier cambio que interactive con el usuario el onChange va a actualizarlo, esto se ve en farm.jsx con name, age y weight que son inputs.

**6. ¿Por qué es buena práctica separar la lógica de datos en archivos como animalsApi.js en vez de hacer peticiones dentro de los componentes?**

Es bueno ya que primero pues evita un duplicacion de codigo, se entiende mucho mejor el codigo y que los componentes se encargan de los datos.

**7. ¿Qué hace que AnimalCard sea un componente reutilizable? ¿Cómo se podría usar una tarjeta similar en otro contexto?**

Lo que lo hace reutilizable es que no pide peticiones, no acepta objetos fijos y lo mas viable para utilizarlo en otros proyectos seria en una veterinaria que es mas viable.

**8. ¿Qué elementos del proyecto contribuyen a la accesibilidad?**

los 3 elementos que contribuyen, seria: title en los buttons de text, el arial label que es para cerrar las alertas y el arial live que es para avisar errores

**9.Antes de agregar una funcionalidad nueva, ¿qué pasos debes pensar según la filosofía de React?**

saber que datos necesito, mirar que componente me queda mejor, ver que componentes van a mostrar la informacion, como va a hacer la informacion, si necesito efectos (useEffect). 

**10.¿Qué conceptos de React aprendidos en este proyecto podrías reutilizar en otro tipo de aplicación?**

Componentes como AnimalCard, Alert, Loader.
useState para los formularios, filtros o contadores.
useEffect para cargar los API.
y la actualizacion de ui 
