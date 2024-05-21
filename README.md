¿Qué es un Coding Dojo?
	Los Coding Dojos son reuniones que permiten a los programadores no solo divertirse si no también mejorar sus habilidades realizando diversos desafíos de programación.
	Las características clave de un Coding Dojo incluyen un ambiente no competitivo y colaborativo donde todos los niveles de habilidad son bienvenidos y se fomenta la experimentación sin miedo al fracaso. Esto crea un espacio seguro y enriquecedor para el aprendizaje.
	Para llevar a cabo un Coding Dojo, se necesita una sala de reuniones con suficientes asientos (para entre 5 y 20 personas), al menos una computadora y un proyector digital. La duración de estas sesiones varía entre 2 horas y 30 minutos a 3 horas.
  Existen 2 tipos de Coding Dojos:
		PreparedKata: Un presentador muestra cómo resolver el desafío paso a paso. 
		RandoriKata: El desafío se resuelve en parejas con rotación de roles.

Diferencia entre Requerimientos, Criterios de Aceptación y Escenarios de Prueba.
  •	Requerimiento: Propiedad que debe tener algo para resolver un problema.
  •	Criterios de Aceptación: Reglas que verifican que se cumple el requerimiento.
  •	Escenarios de Prueba: Ejemplos para validad los Criterios de Aceptación.
	
Ejemplo: Bloc de Notas	
Requerimientos:
  •	Req-1: Debe permitir la creación de una nota.
  •	Req-2: Debe permitir la entrada de texto.
  •	Req-3: Debe permitir el guardado de la nota.
  •	Req-4: Debe permitir eliminar una nota.	
Criterios de Aceptación: 
  •	Cri-1-1: Se puede crear el archivo txt fuera de la aplicación.
  •	Cri-2-1: Máximo de 2000 caracteres por nota.
  •	Cri-3-1: Se pregunta al usuario dónde desea guardar la nota.
  •	Cri-4-1: Se debe confirmar la decisión del usuario.
  
Escenario de Pruebas:
  Sce-1-1-1:
    •	Dado que el usuario está en la aplicación de notas.
    •	Cuando el usuario selecciona la opción para crear una nueva nota.
    •	Entonces se debe mostrar una interfaz para ingresar texto.
  Sce-2-1-1: 
    •	Dado que el usuario ha creado una nueva nota.
    •	Cuando el usuario ingresa texto en la nota.
    •	Entonces el texto debe ser visible en la interfaz de la nota.
  Sce-2-2-2:
    •	Dado que el usuario está ingresando texto en una nota,
    •	Cuando el texto ingresado excede los 2000 caracteres,
    •	Entonces la aplicación debe evitar la entrada adicional de texto y mostrar un mensaje de error.

De dos ejemplos de requerimientos no-funcionales, y especifique cuál es su categoría. 
ReqNF-1: 
	La aplicación debe encriptar todas las notas guardadas para asegurar la 	confidencialidad de la información del usuario.
	Categoría: Seguridad
ReqNF-2:
	La aplicación debe responder a cualquier acción del usuario en menos de 2 segundos.
	Categoría: Rendimiento
 
¿Qué es TDD?
  Test Driven Development. es una práctica de desarrollo de software que se enfoca en crear casos de prueba unitarios antes de desarrollar el código real. Es un enfoque iterativo que combina programación, creación de pruebas unitarias y refactorización.
  •	El enfoque TDD se origina en los principios del manifiesto ágil y la programación extrema.
  •	Como su nombre sugiere, el proceso de prueba impulsa el desarrollo de software.
  •	Además, es una práctica estructurada que permite a los desarrolladores y probadores obtener un código optimizado que demuestra ser resistente a largo plazo.
  •	En TDD, los desarrolladores crean pequeños casos de prueba para cada característica basados en su entendimiento inicial. La intención principal de esta técnica es modificar o escribir nuevo código solo si las pruebas fallan. Esto evita la duplicación de scripts de prueba.

¿Que son pruebas unitarias automatizadas?
  Las pruebas unitarias automatizadas son un tipo de prueba en el desarrollo de software donde se examinan unidades individuales o componentes de código para garantizar que funcionen como se espera. Estas unidades pueden ser funciones, métodos o clases. La automatización implica escribir scripts o programas que ejecutan estas pruebas de forma sistemática y repetible, lo que permite detectar errores o problemas en el código de manera rápida y eficiente. 
  Las pruebas unitarias son parte integral de las metodologías de desarrollo ágil y ayudan a mejorar la calidad del software al identificar y corregir problemas en etapas tempranas del ciclo de desarrollo.

¿Cuál fue el 1er framework de pruebas unitarias y para cual lenguaje fue creado?
  Xunit creado por Henk Benk para Smalltalk en 1969 

Describa los componentes de la arquitectura xUnit
  La arquitectura xUnit es un conjunto de principios y patrones utilizados para crear frameworks de pruebas unitarias. Aunque puede haber variaciones entre diferentes implementaciones, los componentes principales de la arquitectura xUnit son:

Clase de prueba (Test Class):
  •	Representa una colección de pruebas relacionadas.
  •	Contiene métodos de prueba que verifican el comportamiento de unidades específicas de código.
  •	Cada método de prueba generalmente corresponde a una condición o aspecto particular que se está probando.
  
Métodos de prueba (Test Methods):
•	Son los métodos dentro de la clase de prueba que realizan las pruebas unitarias.
•	Cada método de prueba debe ser independiente y probar una sola unidad de funcionalidad del código.
•	Utilizan aserciones para verificar si el comportamiento observado coincide con el esperado.

Fixture
•	Representa el entorno necesario para ejecutar las pruebas.
•	Puede incluir la inicialización de objetos, la configuración de parámetros, la conexión a bases de datos, entre otros.
•	Los fixtures pueden ser compartidos entre múltiples pruebas o pueden ser específicos para cada prueba.

Aserciones (Assertions):
•	Son declaraciones dentro de los métodos de prueba que verifican que un resultado esperado es igual al resultado real producido por el código bajo prueba.
•	Si una aserción falla, la prueba correspondiente se considera fallida.

Suite de pruebas (Test Suite):
•	Agrupa un conjunto de pruebas relacionadas.
•	Puede ser una colección de clases de prueba, métodos de prueba o incluso otras suites de pruebas.

Runner (Ejecutador):
•	Es responsable de ejecutar las pruebas definidas en las clases de prueba.
•	Controla el flujo de ejecución, informa sobre el estado de las pruebas (éxito, falla, etc.) y recopila los resultados de la ejecución.

Framework (Marco de trabajo):
•	Proporciona la infraestructura necesaria para escribir, organizar y ejecutar pruebas unitarias.
•	Define la estructura y las reglas para la creación de pruebas.
•	Ejemplos populares de frameworks xUnit incluyen JUnit (para Java), NUnit (para .NET), PHPUnit (para PHP) y pytest (para Python).

Indique al menos tres desventajas de las pruebas unitarias automatizadas
•	Coste y tiempo de inversión inicial
•	Mantenimiento

Indique al menos tres ventajas de las pruebas unitarias automatizadas
•	Detección temprana de errores
•	Ejecución rápida y repetible
•	Mejorar la calidad del código
