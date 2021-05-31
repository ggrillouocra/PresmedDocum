<!-- @format -->

# TECNOLOGIA DE LA INFORMACION OSPECON - Propuesta Organizativa

<br>

## **Introducción**


<br>

### **Nuestro sector se encuentra en un punto de inflexión en donde es necesario tomar una decisión**

Los servicios que brindamos, si bien han sido de gran utilidad para la organización, van quedando desactualizados tanto tecnologicamente como en términos de negocio.  
Algunos servicios mas temprano que tarde quedarán inutilizables debido a la falta de soporte de nuestros proveedores.  
Seguir haciendo lo que hacemos hoy parece no ser viable, reparar y actualizar lo que tenemos al tiempo que creamos nuevos servicios sin seguir un plan de modernización nos cuesta cada vaz mas recursos, al tiempo que nos hace mas dependientes de la suerte y menos de nuestra capacidad.  
Nuestras aplicaciones son programador-dependiente lo que implica que cada desarrollador es el único experto en el mantenimiento y actualización de las aplicaciones que desarrolló.
Esto lleva a que cada desarrollador se vea cada vez mas y mas ocupado. Sumado a los nuevos desarrollos tiene que mantener los anteriores.  
Como se puede intuir, aunque tengamos la suerte de contar siempre en tiempo y forma con todos los recursos humanos de manera incondicional, esta forma de trabajo tiene un límite.  
Hay mucho trabajo por delante,debemos migrar aplicaciones existentes y continuar con el desarrollo de nuevos servicios, tomar una decisión es urgente.

<br>

### **Una nueva forma de trabajo es posible**

Podemos ver esta situación como una oportunidad para poner en valor nuestro sector.  
No somos los primeros en esta situación, hay muchas empresas en nuestro país y el exterior que tuvieron que hacer este cambio.  
La propuesta que presentamos en este documento no es mas que mostrar el camino a seguir basado en la experiencia de empresas que ya lo caminaron y nos enseñan como hacerlo.

<br>
<br>

### **Objetivos del Cambio**

-   Mejorar la calidad de los datos y servicios ofrecidos a la organización.
-   Optimizar recursos tanto humanos como tecnológicos.
-   Mejorar la escalabilidad de los recursos.
-   Mejorar la seguridad de los procesos.
-   Disminuir errores.
-   Mejorar la satisfacción personal de los integrantes de TI.
-   Promover la cultura del mejoramiento continuo.

<br>
<br>

### **¿Cómo lo hacemos?**

Una vez convencidos que queremos dar el paso adelante, debemos determinar cómo vamos a llegar a los objetivos propuestos.  
Existen numerosas estrategias para llevar un area de TI adelante de manera ágil y dinámica. Hemos elegido algunas que demostraron dar resultados satisfactorios.

<br>

#### **Arquitectura de Microservicios**

Utilizaremos la Arquitectura de Microservicios. Esto quiere decir que dividiremos la solución en varios servicios independientes que puedan ponerse en linea rápidamente.  
Cada servicio debería especializarse en un área concreta de la solución y debería correr en su propio proceso, de tal forma que aporte valor rápidamente.

<br>
Los beneficios con respecto a la solución monolítica:

-   Al ser pequeño y resolver un subconjunto concreto de problemas se torna mas simple la comprensión, desarrollo y mantenimiento.
-   Por correr en procesos separados el escaldo es mas simple.
-   Aumenta la eficiencia del equipo por el desarrollo progresivo y en paralelo.
-   Posibilidad de utilizar diferentes lenguajes de programación.
-   Posibilidad de persistir datos bajo diferentes tecnologías.
-   Aprovechamiento de tecnologías desarrolladas en otras plataformas.
-   Automatizar el testeo y despliegue.

Las desventajas con respecto a la solución monolítica:

-   Mayor complejidad en la comunicación entre servicios.
-   Necesidad de una infraestructura especial para montar los servicios.
-   Mayor complejidad en las transacciones que implican varios servicios.

<br>
Aquí vemos un esquema que representa la versión monolítica de nuestras soluciones actuales versus la versión de microservicios.

![./images/monolithic-vs-microservices.png](./images/monolithic-vs-microservices.png)

<br>
<br>

#### **Arquitectura Hexagonal**

Es una estrategia que nos propone separar los servicios por capas. Cada capa representa una responsabilidad con limites bien claros.  
Separaremos nuestros servicio en tres capas: Dominio, Aplicación e Infraestructura.  
El Dominio es una capa de código de alto nivel donde se modela el negocio y es agnóstico del resto de las capas. Lo modelaremos usando principios DDD del cual hablaremos mas adelante.  
La Aplicación es la capa que conecta el dominio con el mundo exterior. Contiene una serie de puertos y adaptadores que conectan por una lado con las UI, apis de mensajería, etc., y por otro con la base de datos, servicio de mails,etc.  
La Infraestructura son todos aquellos servicios externos al nuestro. Por ejemplo para persistir los datos, mandar mails, enviar mensajes a otros servicios, etc.  
El separar las capas de esta manera nos da la libertad de adaptarnos rápidamente a cambios en la tecnología o el negocio, testear nuestro código y escalarlo rápidamente.

![./images/hexagonal.png](./images/Hexagonal.png)

<br>
<br>

### **Los Roles**

<br>

> Any organization that designs a system (defined broadly) will produce a design whose structure is a copy of the organization's communication structure.
>
> -- Melvin Conway, 1968

<br>

Si queremos cambiar el diseño de nuestros sistemas debemos cambiar la estructura comunicacional de nuestro área.  
La migración de los sistemas existentes a la nuevas tecnologías no se podría hacer si cada uno de nosotros no conoce y domina primero las nuevas tecnologías.  
Necesitamos ir migrando nuestra forma de pensar y trabajar a medida que migramos nuestros sistemas.
Para ello tenemos que crear nuevos roles, redefinir los existentes y organizar equipos que reflejen la estructura final de nuestros sistemas.  
Los roles serán ocupados por integrantes del equipo que hoy día ocupan roles relacionados.  
Esto nos dará un doble beneficio: contar con integrantes que conocen profundamente los actuales sistemas, infraestructuras y metodologías mientras se transforman para crear las nuevas.  
Al mismo tiempo los nuevos integrantes que se vayan sumando se tornaran productivos rápidamente ya que el campo en el que se deberán desenvolver sera mas acotado.

<br>
<br>

![Equipos aislados](./images/conways-law.png)  
![Equipos inter-funcionales](./images/PreferFunctionalStaffOrganization.png)

<br>
<br>

| Rol                       | Resumen de Funciones (simplificado)                                                                  | Ejemplo de la vida real                                                                                                                | Capa de Servicio                     |
| ------------------------- | ---------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| Analista                  | Es el que tiene contacto con el cliente. Descubre y documenta los problemas/soluciones.              | Se reúne con el sector de contable para tratar el tema de una nueva forma de pago, documenta los cambios, crea tickets para desarrollo | Dominio                              |
| Arquitecto                | Diseña el espacio técnico donde se va a resolver la solución.                                        | Define que se van a crear microservicios alojados en docker y una PWA disponible en la nube.                                           | Dominio, Aplicación, Infraestructura |
| Desarrollador back-end    | Modela el dominio, aplicación e infraestructura.                                                     | Programa el modelo de dominio, una web api y la estructura de tablas en la base de datos.                                              | Dominio, Aplicación, infraestructura |
| Diseñador                 | Crea la interfaz de usuario.                                                                         | Diseña una UI en Figma para darle al desarrollador de front-end                                                                        | Infraestructura                      |
| Desarrollador front-end   | Crea la aplicación para el usuario final.                                                            | Crea una PWA siguiendo el diseño de UI y usando las apis que creo el desarrollador back-end                                            | Aplicación, Infraestructura          |
| Tester                    | Testea las aplicaciones y crea la documentación para el usuario final.                               | Prueba la interfaz de usuario, genera tickets en caso de bugs, y actualiza el manual de usuarios.                                      | Infraestructura                      |
| Administrador de sistemas | Administra la infraestructura.                                                                       | Contrata mas recursos de servidor y un nuevo servicio de correo en la nube.                                                            | Infraestructura                      |
| DevOp                     | Es el nexo entre desarrolladores y operaciones. Se encarga de montar las aplicaciones en producción. | Instala la aplicación en la nube para producción y aumenta la cantidad de microservicios para atender mas usuarios                     | Infraestructura                      |
| Atención a Usuario        | Atiende requerimientos del usuario final.                                                            | Recibe un llamado, detecta un bug y crea un ticket para desarrollo.                                                                    | Infraestructura                      |

<br>

Cada integrante de TI puede estar ocupando uno o mas roles.  
Podría estar desempeñando un rol en un equipo mientras ocupa otro en otro equipo para otro desarrollo.  
Un desarrollador back-end podría hacer análisis o desarrollar algo del front-end, un integrante de atención a usuarios podría dedicarse al testing, etc.  
A medida que avancemos en la migración de los sistemas iremos descubriendo como naturalmente cada integrante se va adaptando al rol en el que mejor se siente y desempeña.

<br>
<br>

## **Conclusión**

Es momento de cambiar para llevar adelante una area de TI mas eficiente y moderna.  
Los herramientas propuestas para este cambio ya han sido validadas por otras empresas y llevan un tiempo razonable siendo usadas con éxito.  
La migración de nuestros sistemas y al mismo tiempo de nuestras capacidades comunicacionales es ineludible.  
El resultado sera beneficioso tanto para nuestra organización como para cada uno de nosotros en lo personal y profesional.

<br>
<br>

## **Links de interés**

[Arquitectura de Microservicios definición (Wikipedia)](https://en.wikipedia.org/wiki/Microservices)

[Arquitectura de Microservicios teoría (James Lewis, Martin Flower)](https://martinfowler.com/articles/microservices.html)

[Arquitectura de Microservicios y DDD teoría y práctica (Microsoft)](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/)

[Arquitectura Hexagonal en (Wikipedia)](<https://en.wikipedia.org/wiki/Hexagonal_architecture_(software)>)