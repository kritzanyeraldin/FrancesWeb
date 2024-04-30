# FrancesWeb

Entregrable Calificado 1 y 2

Integrantes:

- Armijo Ramos, Carlos
- Sullca Espinoza, Kritzan

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

3. Seguimiento del progreso y evaluación
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
