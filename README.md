**Agregar en el README el proceso que seguiste para resolver la práctica y respuesta a preguntas, se está evaluando como abordas problemas similares a los que se presentarán en la posición.**
Investigué sobre el las GitHub Actions, realicé varias practicas hasta entender su funcionamiento, vi tutoriales, leí documentación, etc.
Preparé el hambiente, instalando las herramientas necesarias, cloné el código, ejecuté el comando de "mvn verify", si es exitosa se compila y permite el merge a la rama main
En dicha rama agregue un regla de protección

**¿Consideras útil agrega la acción de caché al workflow? Si consideras que sí, agrégala.**
Sí, porque puede acelerar el flujo del trabajo

**Hasta ahora solo se ha construido y publicado el código en Github Packages y aún no se ha definido la plataforma sobre la que se ejecutará el servicio. ¿Es posible desplegar automáticamente el artefacto guardado en Packages con Github Actions? Si consideras que sí, incluye el despliegue automático (no necesariamente debe realizar un despliegue real a una plataforma, puedes simularlo imprimiendo en consola el mensaje “Despliegue en curso” pues aún no se conoce en dónde se ejecutará)**
Sí es posible, existe un actions para conectarse a un servidor remoto y ejecutar comandos

**El equipo de Arquitectura define que el API se desplegará en una plataforma basada en contenedores, pero aún están evaluando cuál será esta plataforma, se encuentran revisando Kubernetes, ECS y App Runner. Quieren conocer la opinión del equipo de DevOps sobre que modificaciones se tendrían que hacer al pipeline y a la estructura del proyecto (archivos y carpetas en el repositorio). ¿Qué modificaciones consideras que se tendrían que realizar a los workflows para trabajar con imágenes de contenedores, siguiendo las mejores prácticas que conozcas?**
Se deberá crear un Dockerfile para realizar los procesos de compilado, en caso de que el test sea exitoso. Debemos ejecutar los comandos de docker dentro del pipeline del workflow

**El equipo de Arquitectura define que se utilizará ECS con Fargate y el equipo de AWS comparte el siguiente repositorio con plantillas de Cloudformation de ejemplo. ¿Qué pasos y/o herramientas utilizarías para entender las plantillas de Cloudformation y evaluar que ajustes se tendrían que realizar a la etapa de despliegue? (La pregunta está orientada a entender cómo abordarías el problema, no es necesario implementar una etapa en tú repositorio de la práctica).**
Primero debo conocer el funcionamiento, leer la documentación, mirar videos, realizar pruebas, etc.
Para luego realizar los ajustes necesarios, mediante prueba y error
