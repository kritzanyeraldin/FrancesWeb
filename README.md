# FrancesWeb

Entregrable Calificado 1 y 2

Integrantes:

- Armijo Ramos, Carlos
- Sullca Espinoza, Kritzan

  Prototipo 1: https://www.figma.com/file/JRPBJsXlBQzx9gRMo37Sp6/LearnFrench?type=design&node-id=0%3A1&mode=design&t=AZuRHh5yE6NCPbti-1
  Prototipo 2: https://app.visily.ai/projects/9802071b-98f4-4ca0-8137-57db25e879aa/boards/900418 

## Descripción de los usuarios potenciales

Los usuarios potenciales de tu aplicación de asistencia para el aprendizaje de un idioma extranjero son una audiencia diversa que incluye desde principiantes hasta estudiantes avanzados. Estos usuarios pueden tener diferentes motivaciones para aprender un nuevo idioma, desde viajar y trabajar en el extranjero hasta fines académicos o personales. Además, los usuarios pueden tener diferentes estilos de aprendizaje y preferencias en términos de interactividad, ritmo de estudio y contenido personalizado. La aplicación debe tener en cuenta toda esta variedad y diseñarse con esta en mente.

## Visión general de lo que los usuarios intentan lograr y lo que hará el sistema

- Los usuarios buscan ser usuarios más proficientes del idioma francés, con el objetivo de poder pasar alguno de los exámenes internaciones de idioma francés(como el DELF-DALF)
- El sistema proveerá herramientas que facilitarán el aprendizaje del idioma, como lecciones de gramática y vocabulario.

## Análisis de Tareas y Casos de Uso

1. Registro de usuario

   - Un usario debe poder registrarse en la aplicación para poder acceder a un contenido personalizado y además para que se guarde su progreso.
   - Casos de uso:
     - Un usuario nuevo se registra en la aplicación.
     - Un usuario existente inicia sesión en la aplicación para restaurar su progreso.

2. Exploración de contenido

   - Un usuario debe poder explorar y acceder a varios tipos de contenido, incluyendo lecciones interactivas, lecciones de gramática, y un vocabulario/diccionario con buscador.
     -Casos de uso: - Un usuario busca lecciones específicas utilizando filtros como nivel de dificultad, tema y tipo de contenido. - Un usuario genera material de lectura y/o conversaciones relacionado con su área de interés o nivel de competencia.

3. Pronunciación mediante interfaz de voz
Un usuario mediante lecciones puede hacer uso de la interfaz de voz que ofrece la aplicación para repetir la frase que ofrece el ejercicio.


4. Seguimiento del progreso y evaluación
   - Los usuarios deben poder realizar un seguimiento de su progreso de aprendizaje y recibir retroalimentación sobre su desempeño en diferentes áreas del idioma.
   - Casos de uso:
     - Un usuario consulta su tablero de progreso para ver estadísticas sobre su tiempo de estudio, puntajes de pruebas y áreas de fortaleza y debilidad.
     - Un usuario recibe retroalimentación inmediata después de completar actividades de aprendizaje, incluyendo correcciones automáticas y sugerencias para mejorar.

- Una descripción de las características importantes del contexto

## Análisis de Tareas y Casos de Uso

1. Definir Niveles y subniveles :

   - Un administrador necesita definir niveles para desarrollar el curso de aprendizaje del idioma francés y guardalas en una base de datos
   - Pasos:
     - Un administrador define en cuántos niveles se va a desarrollar el aprendizaje del idioma francés y cuántos subniveles va tener cada nivel a través de un prompt para que el LLM genere una respuesta. En caso de ser válida la respuesta el administrador guarda la respuesta en la base de datos, para que sea utilizada posteriormente, sino genera otro prompt hasta obtener la respuesta deseada.
   
2. Definir Capítulos y lecciones

   - Un administrador necesita definir cuántos capítulos tendrá cada subnivel. También necesita definir cuantas lecciones tendrá cada capítulo.
   - Pasos:
     - Un administrador define cuantos capítulos tendrá cada subnivel y cuantas lecciones tendrá cada capítulo. El administrador genera un prompt con las especificaciones que necesita (número de capítulos, nombre y número de lecciones) y el LLM procesa la solicitud y retorna una respuesta. En caso de ser válida la respuesta el administrador guarda la respuesta en la base de datos, para que sea utilizada posteriormente, sino genera otro prompt hasta obtener la respuesta deseada.

3. Definir Contenido de cada lección

   - Un administrador necesita definir el contenido que tendrá cada lección.
   - Pasos:
     -Un administrador define el tipo de preguntas que se va realizar en cada lección. El administrador genera un prompt con las especificaciones que necesita para generar las preguntas (pregunta, resultado, opciones). El LLM procesa el prompt ingresado y retorna una respuesta. EL administrador guarda la respuesta en la base de datos, en caso de ser válida sino genera otro prompt hasta obtener la respuesta deseada.

4. Definir Contenido para Gramática
   - Un administrador necesita definir el contenido que tendrá Gramatica.
   - Pasos:
     - Un administrador define la gramatica para aprender el idioma frances. El administrador genera un prompt con las especificaciones que necesita para generar la gramtica (temas y contenido).
       El LLM procesa el prompt ingresado y retorna una respuesta. EL administrador guarda la respuesta en la base de datos, en caso de ser válida sino genera otro prompt hasta obtener la respuesta deseada.

5. Definir Preguntas de clasificación
- Un administrador necesita definir el contenido que tendrá la clasificación.
   - Pasos:
     - Un administrador define las preguntas para clasificar un usuario de acuerdo a los niveles definidos anteriormente para aprender el idioma francés. El administrador genera un prompt con las especificaciones que necesita (preguntas, opciones, respuesta correcta).
       El LLM procesa el prompt ingresado y retorna una respuesta. EL administrador guarda la respuesta en la base de datos, en caso de ser válida sino genera otro prompt hasta obtener la respuesta deseada.


## Análisis del sistema usado

### Sistema: Curso de idiomas con lecciones tipo duolingo, diccionario integrado y lecciones de patrones de gramaticales con varios ejemplos.

- Puntos fuerte:

  - Interactividad: Las lecciones tipo Duolingo ofrecen una experiencia interactiva que involucra a los usuarios y los mantiene comprometidos con el aprendizaje del idioma.
  - Variedad de recursos: La integración de un diccionario facilita a los usuarios la búsqueda rápida de significados de palabras desconocidas y les permite expandir su vocabulario de manera efectiva.
  - Enfoque práctico: Las lecciones de patrones gramaticales con ejemplos proporcionan a los usuarios una comprensión práctica de la gramática del idioma, lo que les ayuda a aplicar los conceptos de manera efectiva en situaciones reales.
  - Adaptabilidad: Los usuarios pueden avanzar a su propio ritmo y elegir lecciones según sus necesidades y habilidades, lo que les proporciona flexibilidad en el proceso de aprendizaje.
  - Gamificación: La incorporación de elementos de gamificación, como puntajes, niveles y recompensas, motiva a los usuarios a seguir aprendiendo y progresando en su dominio del idioma.

- Deficiencias:
  - Limitaciones de profundidad: Aunque las lecciones tipo Duolingo son efectivas para introducir y reforzar conceptos básicos, pueden carecer de la profundidad necesaria para comprender aspectos gramaticales más complejos del idioma.
  - Dependencia del contexto digital: La efectividad del sistema depende de la disponibilidad de dispositivos digitales y una conexión a Internet estable, lo que puede excluir a aquellos que tienen acceso limitado a tecnología o recursos en línea.

## Lista de criterios de evaluación:

1. Facilidad de uso
   - La aplicación debe ser intuitiva y fácil de usar para los usuarios, con una navegación clara y funciones autoexplicativas.
   - Medición: Se puede medir mediante pruebas de usabilidad, donde los usuarios completan tareas específicas mientras se observan y registran sus interacciones y comentarios. Además, se pueden realizar encuestas de satisfacción del usuario para evaluar la percepción general de la facilidad de uso de la aplicación.
2. Eficiencia
   - La aplicación debe permitir a los usuarios completar tareas de manera rápida y con un mínimo esfuerzo.
   - Medición: Se puede medir mediante pruebas de tiempo, donde se registra el tiempo que los usuarios tardan en completar tareas específicas en la aplicación y se compara con benchmarks o estándares predefinidos.
3. Aprendizaje intuitivo
   - Los usuarios deben poder aprender a usar la aplicación sin la necesidad de instrucciones extensas o tutoriales.
   - Medición: Se puede medir mediante pruebas de usabilidad con usuarios que son nuevos en la aplicación y observar su capacidad para completar tareas sin ayuda o con una mínima orientación.
4. Satisfacción de usuario
   - Descripción: Los usuarios deben sentirse satisfechos con la experiencia general de uso de la aplicación.
   - Medición: Se puede medir mediante encuestas de satisfacción del usuario después de que los usuarios hayan interactuado con la aplicación, donde se les pide que evalúen diferentes aspectos de la experiencia, como la facilidad de uso, la utilidad y la estética.

## Como se recopiló la información anterior

- Análisis de sistemas existentes: Se examinaron sistemas existentes similares, tanto dentro como fuera del dominio del aprendizaje de idiomas, para identificar características comunes, puntos fuertes y deficiencias. Esto permitió comprender las tendencias actuales en el diseño de aplicaciones y evaluar qué aspectos podrían adaptarse o mejorarse en el contexto específico del proyecto.



## Análisis de Usuarios

1.  Diversidad de habilidades lingüísticas.
    - Implicaciones en el diseño: El diseño debe ser adaptable para atender a usuarios con diversos niveles de habilidades lingüísticas, desde principiantes hasta avanzados. Se pueden ofrecer funciones de personalización para ajustar el nivel de dificultad y el contenido según las necesidades individuales de cada usuario.
2.  Motivación y compromiso variados:
    - Implicaciones en el diseño: La aplicación debe incorporar elementos de gamificación, como puntajes, desafíos y recompensas, para motivar a los usuarios y mantener su compromiso con el aprendizaje. También se pueden incluir funciones de seguimiento del progreso y recordatorios para mantener a los usuarios comprometidos a lo largo del tiempo.
3.  Disponibilidad de tiempo variada:
    - Implicaciones en el diseño: La aplicación debe ser flexible y permitir a los usuarios estudiar en su propio tiempo y ritmo. Se pueden ofrecer lecciones cortas y actividades que se puedan completar en períodos de tiempo más cortos, así como funciones de guardado automático para que los usuarios puedan retomar su progreso en cualquier momento.

## Comparación con otras páginas web

### Primera Página a analizar: https://www.busuu.com/es

1. Beneficios

   1. Beneficios
      - Explora una extensa gama de cursos para dominar el idioma de su elección.
      - Adaptados a cada nivel, desde principiante hasta avanzado, asegurando un aprendizaje progresivo.
      - Cada curso está estructurado en capítulos temáticos, facilitando la comprensión y retención de conocimientos.
   2. Experiencia de Aprendizaje Interactiva
      - Ofrece un entorno de aprendizaje dinámico y atractivo mediante lecciones interactivas.
      - Ofrece una experiencia similar a un juego, fomentando el interés y la motivación.
   3. Interfaz Intuitiva y cómoda.
      - Ofrece una navegabilidad con facilidad a través de una interfaz amigable y accesible.
      - Ofrece una experiencia de aprendizaje fluida y agradable.

2. Deficiencias
   - Evaluación del Progreso: La evaluación del progreso no es tan personalizada o detallada como en otros métodos de aprendizaje.

#### Segunda Página a analizar: https://app.mondly.com/home

1. Beneficios

- Categorías de Aprendizaje:

  - La plataforma brinda la posibilidad de enfocarse en categorías específicas del idioma, tales como: Empresarial, Conversacional cotidiano, Viajes,etc. Entre otras de acuerdo a las necesidades e intereses del usuario.

  - El usuario tiene la capacidad de medir su progreso de forma diaria.

  - Se fomenta un entorno de aprendizaje interactivo que hace del proceso algo más: agradable y dinámico.

2. Deficiencias

   - La interfaz de la plataforma presenta características positivas en términos de interactividad y dinamismo. Sin embargo, puede llegar un poco confusa si es que se quiere ingresar a algún módulo que ofrece.

### ¿Como influyó este análisis en el diseño de nuestra página?

Nuestra aplicación está orientada para cualquier usuario que desee aprender el idioma francés, el usuario podrá comenzar el curso desde el nivel básico, sin embargo si este posee conocimientos en el lenguaje, podrá realizar un test de clasificación. Cada nivel tiene diferentes subniveles de esta forma se asegura que el aprendizaje sea más profundo. El aprendizaje del idioma se da a través de lecciones interactivas. El usuario también podrá visualizar su progreso y un cuadro de estadísticas que refleja su aprendizaje.

El manejo de niveles, subniveles, lecciones, gramática y vocabulario se maneja a través de LLM. Este proveerá todo el contenido que será usado en la aplicación para el aprendizaje del idioma francés. También se hace uso de una interfaz de voz, se utiliza para que el usuario pueda practicar su pronunciación en una lección.
