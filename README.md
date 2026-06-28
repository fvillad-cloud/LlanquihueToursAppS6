# LlanquihueToursAppS6
Actividad Formativa Semana 6 

<h2>Sistema de Gestión de Servicios Turísticos - Llanquihue Tours</h2>

Este proyecto es una aplicación de consola en Java orientada a la gestión de las ofertas turísticas ofrecidas por la empresa LlanqihueTours. Sigue un enfoque clásico de Programación Orientada a Objetos (POO) estructurado mediante herencia, encapsulamiento y polimorfismo. 

<h2>Finalidad del Programa</h2>

El objetivo principal es modelar, instanciar y visualizar diferentes tipos de servicios turísticos disponibles. Centraliza la creación de experiencias (como rutas gastronómicas, paseos lacustres y excursiones culturales) a través de un gestor de datos ("GestorServicios") y despliega los detalles en pantalla utilizando el punto de entrada de la aplicación ("LlanquihueToursAppS6").

<h2>Estructura del Proyecto y Clases</h2>

El sistema se compone de los siguientes módulos y clases organizados por paquetes:

### Paquete `model` (Modelos de datos)
* `ServicioTuristico` (Clase Padre o Super Clase):** Modela la estructura general de cualquier servicio turístico. Contiene los atributos compartidos `nombre` y `duracionHoras`.
* `RutaGastronomica` (Clase Hija): Extiende de `ServicioTuristico`. Agrega el atributo específico `numeroDeParadas` para representar la cantidad de locales a visitar.
* `PaseoLacustre` (Clase Hija): Extiende de `ServicioTuristico`. Añade el atributo `tipoEmbarcacion` (ej: Catamarán, lancha) adaptado a recorridos acuáticos.
* `ExcursionCultural` (Clase Hija): Extiende de `ServicioTuristico`. Incorpora la propiedad `lugarHistorico` para definir el patrimonio o sitio arqueológico a recorrer.

### Paquete `data` (Persistencia de datos)
* **`GestorServicios`:** Actúa como una fábrica de servicios. Es la clase encargada de inicializar y retornar instancias preconfiguradas de cada una de las experiencias turísticas.

### Paquete `app` (Punto de entrada)
* **`LlanquihueToursAppS6`:** Contiene el método `main`. Inicializa el gestor, recupera los servicios turísticos creados y los imprime en consola llamando de forma implícita a sus métodos `toString()`.

##  Instrucciones de Ejecución

Descarga los archivos en sus respectivas carpetas y luego carga el proyecto en Netbeans.

