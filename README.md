# Descripción
Codeando Monterrey es parte de un **movimiento a nivel nacional** llamado **Codeando México**,
nuestro objetivo es propiciar que se genere tecnología que pueda responder
de manera puntual a los problemas y retos del entorno social en que vivimos.

> Me gustaría ver a Codeando Monterrey como un colectivo de hackers,
> autogestionable y remoto, que aporte o genere proyectos open source de
> índole social/cívico que puedan ser replicables, reproducibles y tengan
> la documentación necesaria para entender el contexto en el que se
> desarrolló el problema y la solución.

![logo](https://avatars1.githubusercontent.com/u/7444874?v=3&s=200)
*logo por: [luismnzr](http://www.luismanzur.com/)*

El motivo de este documento, es proveer de información para que los proyectos
se ejecuten de manera consistente, y ayude a ser viable la manutención de los mismos.

**Este documento está en BETA y abierto a modificaciones.**

`༼ つ ◕_◕ ༽つ Give me your Pull Request`

## Glosario
Para evitar problemas de comunicaión, describiré brevemente los
terminos que utilizé para definir la visión:

  - **Colectivo**: Un grupo de personas con objetivos similares.

  - **Hacker**: Alguien entusiasta por el conocimiento, un pensador,
  artesano, solucionador de problemas, [*shoshin*](https://en.wikipedia.org/wiki/Shoshin).

  - **Autogestionable**: Cuando la entidad misma genera y hace
  uso de recursos y convenciones para eliminar la necesidad
  de un agente externo dentro del flujo de trabajo.

  - **Remoto**: Cuando todas las interacciones implicadas por el flujo
  de trabajo pueden suceder *on-line*. (En la parte técnica)

  - **Open Source**: Que sea **accessible** para quien quiera aprender
  del proyecto, enfocándose en la **transparencia** de sus elementos.

  - **Social/Cívico**: Engloba al gobierno y el entorno del día a día,
  temas como: salud, transparencia, medio ambiente, movilidad, justicia, etc.

  - **Replicable**: Que se puedan realizar copias y sea trasladable
  (as in Euclidian geometry).

  - **Reproducible**: Que alguien más, utilizando los componentes
  necesarios, pueda generar una instancia del proyecto.

  - **Documentación**: Compendio de información.

*Nótese que estas definiciones no se reducen al ámbito de la
programación, aún así, el enfoque que se le dará al documento
será relacionado directamente con proyectos que impliquen
código de por medio.*


## Nanos gigantum humeris insidentes
Estos fueron algunos los recursos que influenciaron de alguna
manera este documento:
  - [Twelve Factor](http://12factor.net/)
  - [DWYL](http://www.dwyl.io/)
  - [Code for America](https://www.codeforamerica.org/)
  - [GovLab Academy](http://govlabacademy.org/)
  - [Free Code Camp](https://www.freecodecamp.com/)
  - [Codendo México](https://codeandomexico.org/)
  - [The Cathedral and the Bazaar](https://en.wikipedia.org/wiki/The_Cathedral_and_the_Bazaar)
  - [GitHub](https://github.com/)


# ¿Cómo trabajar en proyectos?
Algo que puede generar **conflicto** en el colectivo, son en las prácticas para
desarrollar un proyecto. **No todos los partícipes comparten las
mismas metodologías de desarrollo**.

Propongo ser algo extrictos e ir clarificando qué elementos
tiene que tener un proyecto para que sea aceptado por el colectivo, y enlistar
algunas metodologías y herramientas opcionales.


## Elementos de un proyecto
  - **Sistema de control de versiones**: No hagas nada que no puedas deshacer.

  - **Host del proyecto**: Lugar dedicado para almacenar y consultar
  el código del proyecto. (Lo que permite que sea Open Source)

  - **Issue/Bug tracking**: Lugar para reportar problemas con el proyecto,
  con fin de que los desarrolladores puedan dar seguimiento.

  - **Roadmap**: Un plan de metas a corto y largo plazo del proyecto,
  con el fin de facilitar la colaboración y dar contexto al desarrollo.

  - **Task tracking**: Seguimiento de tareas. Lugar donde se pueda ver qué
  es lo que está pendiente de implementar, con fin de facilitar la
  colaboración.

  - **Documentación**: Lo que sea necesario para entender el proyecto,
  incluyendo desde la implementación hasta su contexto.

  - **Pruebas**: Asegurarse de que lo que "funcione", funcione.

  - **Publicidad**: ¿Si cae un árbol en un bosque, y nadie lo escucha...

  - **Bitácora de desarrollo**: Facilita la replicabilidad, lo hace
  accessible y transparente. Si se conoce el pasado, se puede aprender de él.

*NOTA: Puede que sea un overkill para algunos proyectos; tómese a concideración.*

--------------------------------------------------------------------------------

Recomendaciones y sugerencias para cumplir con cada uno de los puntos.

### Sistema de control de versiones
[Git](https://git-scm.com/) es el más famoso y con más documentación y guías.
Tiene soporte para la mayoría de los hosts de código.

Para los powerusers que les interesa tener un workflow y branching model limpio,
les recomiendo [gitreflow](https://github.com/reenhanced/gitreflow).

**Tutorial**: *En inglés (se busca traducción)*, para aprender Git. [learn-git](https://github.com/oelizondo/learn-git)

**Requisitos:** Con que puedan hacer rollback en su código, todo está bien.


### Host del proyecto
GitHub es donde ocurre casi toda la acción. Muchos de los proyectos más grandes
de código abierto están en GitHub. La comunidad es muy activa y tiene buenas
features.

**Tutorial:** [Disculpe... ¿Tiene un minuto para hablar de GitHub?](https://github.com/CodeandoMonterrey/GitHub-Simple)

**Requisitos:** Mientras la gente pueda ver el código y bajarlo, está bien.


### Issue/Bug tracking
Si tu código vive en GitHub, GitLab, o BitBucket, puedes utilizar las
herramientas que te brindan.

Muchos usan [JIRA](https://www.atlassian.com/software/jira/comparison/jira-vs-github),
pero puedes utilizar hasta Evernote o un Google Spread Sheet.

**Recursos**: [Open-Source template](https://www.talater.com/open-source-templates/#/), [Github issues](https://github.com/blog/2111-issue-and-pull-request-templates)

**Requisitos**: Que se pueda dar seguimiento a las áreas de oportunidad del proyecto.


### Roadmap
Puede ser a través de las herramientas que ofrece GitHub, (los milestones).
**Recursos**: [¿Qué es un Roadmap?](https://es.wikipedia.org/wiki/Roadmap)

**Requisitos**: Que se pueda saber hacia dónde va el projecto.


### Task tracking
Para no duplicar esfuerzos, es necesario llevar control de **­¿Quién hace qué?**

Depende mucho del proyecto, en lo personal, uso los issues de GitHub como
un task tracking, y utilizo [Waffle](https://waffle.io/) para visualizar los
issues como si fuesen un Kanban board.

También está [Trello](https://trello.com/) y [Asana](http://asana.com)

**Requisitos**: Mientras se pueda conocer las tareas del proyecto y quién las
está llevando acabo, lo que sea está bien.


### Documentación
Este es un tema muy extenso, pero creo que se puede resumir en brindar lo
necesario para entender la implementación y el contexto en el que se desarrolla
el proyecto.

Normalmente incluye:
- **descripción del proyecto** _(objetivos, por qué, cómo...)_.
- Guía de uso
- Licencia de uso
- Guía de contribución
- Mucho contexto acerca de la problemática que se quiere resolver

Yo me la fleto (@MrOutis), igual, si me quieren apoyar, denle.
Website
Visit the Wiki
Google Group for discussion

**Recomendaciones**: GitHub ofrece una herramienta llama Wiki, donde puedes
poner información del proyecto. Y también pone como portada del repositorio
un README.

**Tutariales**: Puedes checar la sección de documentación en: [GitHub Simple](https://github.com/CodeandoMonterrey/GitHub-Simple].

**Requisitos**: Que alguien ajeno al proyecto pueda empatizar y entender con
el problema y la solución.


### Pruebas
> The definition of "legacy code" can be described simply as
> "code that doesn't have tests."
> Code you just wrote, 5 minutes ago? Legacy code.
> Code that can't be refactored, but only changed.
>
> How do we prevent the mountain of legacy code that most projects become?
> A solid testing strategy.

Con pruebas me refiero a que chequen dos veces que lo que implementan
cumple con su cometido, lógicamente y que sea de utilidad.

Para esto existen muchas metodologías y herramientas.

Una estrategia para desarrollar código a la par de las pruebas es [*Test Driven Development*](https://en.wikipedia.org/wiki/Test-driven_development).

Es importante conocer a los usuarios de la aplicación, y estar en constante
retroalimentación de que lo que se implemente les servia.
Para esto, muchos hacen [*Pruebas de usabilidad*](https://en.wikipedia.org/wiki/Usability_testing).

**Tutoriales**: [Aprende TDD](https://github.com/dwyl/learn-tdd))

**Requisitos**: Tener un respaldo para el argumento de "esto que implementé, funciona".


### Publicidad
Hacker News, reddit, twitter, facebook... depende mucho del usuario.

Es importante llegar a los grupos que se quiere impactar.
Un buen *hack* para lograr esta, es asociarse desde el principio
con un colectivo u organización que trabajen la problemática del proyecto.
**Los colectivos ya tienen un user-base**

**Requisitos**: Hacerles llegar el proyecto a tus usuarios y/o personas interesadas.


### Bitácora de desarrollo
Un buen `git log` está de lujo, pero si quieren complementar con algún blog,
o lo que sea.

También puede ser algo así como el logbook que hacen en Dragons and Dungeons,
para cuando alguien se quiere unir a una historia que ya está empezada
puedan ver qué se ha hecho y adaptarse.

**Requisitos:** Que la gente pueda saber cómo empezó y por qué
se tomaron las deciciones que se tomaron.
