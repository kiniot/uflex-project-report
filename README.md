<div style="text-align: center;">
  <img src="./assets/logos/upc-logo.png" alt="UPC Logo" style="width: 250px; height: auto;">
</div>

<h2 style="text-align: center;"> Universidad Peruana de Ciencias Aplicadas </h2>

<h4 style="text-align: center"> Ingeniería de Software </h4>

<h4 style="text-align: center"> Periodo: 202610 </h4>

<h4 style="text-align: center"> 1ASI0572 | Desarrollo de Soluciones IOT </h4>

<h4 style="text-align: center"> NRC: 17755  </h4>

<h4 style="text-align: center"> Docente: Marco Antonio León Baca </h4>

<h3 style="text-align: center;"> Informe del Trabajo Final </h3>

<h4 style="text-align: center"> Startup: KinIoT </h4>

<h4 style="text-align: center"> Producto: uFlex </h4>

<h4 style="text-align: center">Integrantes:</h4>

<div style="text-align:center; margin-top: 10px; font-size: 90%; line-height: 1.6;">
   <table style="margin-left: auto; margin-right: auto;">
      <tr>
         <th>Código</th>
         <th>Apellidos y Nombres</th>
      </tr>
      <tr>
         <td>U20221G120</td>
         <td>Crispín Ramos, Daniel Franco</td>
      </tr>
      <tr>
         <td>U20201E843</td>
         <td>Ramirez Mestanza, Salim Ignacio</td>
      </tr>
      <tr>
         <td>U202312222</td>
         <td>Rivera Sosa, Eduardo Gael</td>
      </tr>
      <tr>
         <td>U20221C486</td>
         <td>Sulca Gonzales, Paúl Fernando</td>
      </tr>
      <tr>
         <td>U202312222</td>
         <td>Varela Bustinza, Marcelo Alessandro</td>
      </tr>
   </table>
</div>

<br>

<h5 style="text-align: center; font-style: italic;"> Abril 2026 </h5>

<hr class="page-break">

# Registro de Versiones del Informe

| Version | Fecha | Autor | Descripción de modificación |
|---------|-------|-------|-----------------------------|

<hr class="page-break">

# Project Report Collaboration Insights

En esta sección se presenta un resumen de las actividades de colaboración realizadas para la elaboración del informe del proyecto.

Se utilizó **GitHub** como plataforma de control de versiones y colaboración en equipo. Se incluye enlace para acceder al repositorio para el reporte del proyecto. [Ver en Github](https://github.com/kiniot/uflex-project-report)

Los integrantes del equipo y sus nombres de usuario en GitHub son los siguientes:

| Integrantes                         | Nombre en GitHub |
|-------------------------------------|------------------|
| Crispin Ramos, Daniel Franco        | `danielcr04`     |
| Ramirez Mestanza, Salim Ignacio     | `salimramirez`   |
| Sulca Gonzales, Paúl Fernando       | `Kyrubi`         |
| Rivera Sosa, Eduardo Gael           | `gael-rs`        |
| Varela Bustinza, Marcelo Alessandro | `VarBus`         |

Se usó el flujo de trabajo **GitFlow**, que incluye las siguientes ramas principales:

- **main:** Rama principal que contiene la versión estable y consolidada del documento.
- **develop:** Rama de integración utilizada para fusionar los cambios realizados en las ramas de características.
- **feature/feature-name:** Ramas de características utilizadas para desarrollar secciones específicas del informe, como "feature/introduccion", "feature-requirements", etc.
- **release/vX.X.X:** Rama creada para preparar versiones candidatas al reporte final, siguiendo *Semantic Versioning 2.0.0*. En esta rama se realizan ajustes finales como correcciones menores y revisiones antes de integrarla a `main`.
- **hotfix/fix-name:** Rama utilizada para aplicar correcciones críticas directamente sobre `main`, asegurando la estabilidad de la versión publicada.

## TB1

**Tareas**

Para el desarrollo del TB1, cada participante del equipo realizó las siguientes tareas:

| Integrantes                      | Tarea asignada                                                                                                                                                                                                                                                                 |
|----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

**GitHub Collaboration Insights**

En GitHub se presenta un timeline de las principales ramas creadas por cada integrante del equipo, así como los procesos de merge realizados.  
Todas las ramas fueron gestionadas siguiendo el flujo de trabajo **GitFlow**, adaptado para una organización que utiliza un sistema de control de versiones.

<div style="text-align: center; margin-top: 1rem; margin-bottom: 1rem;">

Gráfico de red (*network graph*) de ramas en el repositorio de GitHub.

![Insights - Network Graph](./assets/images/screenshots/insights-network-graph.png)

</div>

A continuación, se presentan los gráficos que muestran el análisis de los commits en el repositorio correspondiente al informe.  
Estos gráficos detallan la cantidad de líneas de código añadidas por cada miembro del equipo y la actividad de commits registrada.

<div style="text-align: center; margin-top: 1rem; margin-bottom: 1rem;">

Análisis de líneas de código añadidas por contribuyente.

![Insights - Contributors](./assets/images/screenshots/insights-contributor.png)

</div>

El siguiente gráfico muestra la cantidad de commits realizados en la semana con mayor actividad en el proyecto.

<div style="text-align: center; margin-top: 1rem; margin-bottom: 1rem;">

Análisis de cantidad de commits realizados por semana.

![Insights - Commits](./assets/images/screenshots/insights-commits.png)

</div>

<hr class="page-break">

# Contenido

- [Capítulo I: Introducción](#capítulo-i-introducción)
   - [1.1. Startup Profile](#11-startup-profile)
      - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
      - [1.1.2. Perfiles de los integrantes del equipo](#112-perfiles-de-los-integrantes-del-equipo)
   - [1.2. Solution Profile](#12-solution-profile)
      - [1.2.1. Antecedentes y problemática](#121-antecedentes-y-problemática)
      - [1.2.2. Lean UX Process](#122-lean-ux-process)
         - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
         - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
         - [1.2.2.3. Lean UX Hypothesis](#1223-lean-ux-hypothesis-statements)
         - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
   - [1.3. Segmentos objetivo](#13-segmentos-objetivo)

- [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
   - [2.1. Competidores](#21-competidores)
      - [2.1.1. Análisis competitivo](#211-análisis-competitivo)
      - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
   - [2.2. Entrevistas](#22-entrevistas)
      - [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)
      - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
      - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
   - [2.3. Needfinding](#23-needfinding)
      - [2.3.1. User Personas](#231-user-personas)
      - [2.3.2. User Task Matrix](#232-user-task-matrix)
      - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
      - [2.3.4. Empathy Mapping](#234-empathy-mapping)
   - [2.4. Big Picture EventStorming](#24-big-picture-eventstorming)
   - [2.5. Ubiquitous Language](#25-ubiquitous-language)

- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
   - [3.1. User Stories](#31-user-stories)
   - [3.2. Impact Mapping](#32-impact-mapping)
   - [3.3. Product Backlog](#33-product-backlog)

- [Capítulo IV: Solution Software Design](#capítulo-iv-solution-software-design)
   - [4.1. Strategic-Level Domain-Driven Design](#41-strategic-level-domain-driven-design)
      - [4.1.1. Design-Level EventStorming](#411-design-level-eventstorming)
         - [4.1.1.1. Candidate Context Discovery](#4111-candidate-context-discovery)
         - [4.1.1.2. Domain Message Flows Modeling](#4112-domain-message-flows-modeling)
         - [4.1.1.3. Bounded Context Canvases](#4113-bounded-context-canvases)
      - [4.1.2. Context Mapping](#412-context-mapping)
      - [4.1.3. Software Architecture](#413-software-architecture)
         - [4,1.3.1. Software Architecture System Landscape Diagram](#4131-software-architecture-system-landscape-diagram)
         - [4,1.3.2. Software Architecture Context Level Diagrams](#4132-software-architecture-context-level-diagrams)
         - [4.1.3.3. Software Architecture Container Level Diagrams](#4133-software-architecture-container-level-diagrams)
         - [4.1.3.4. Software Architecture Deployment Diagrams](#4134-software-architecture-deployment-diagrams)
   - [4.2. Tactical-Level Domain-Driven Design](#42-tactical-level-domain-driven-design)
      - [4.2.X. Bounded Context: <Bounded Context Name>](#42X-bounded-context-bounded-context-name)
         - [4.2.X.1. Domain Layer](#4211-domain-layer)
         - [4.2.X.2. Interface Layer](#4212-interface-layer)
         - [4.2.X.3. Application Layer](#4213-application-layer)
         - [4.2.X.4. Infrastructure Layer](#4214-infrastructure-layer)
         - [4.2.X.5. Bounded Context Software Architecture Component Level Diagrams](#4215-bounded-context-software-architecture-component-level-diagrams)
         - [4.2.X.6. Bounded Context Software Architecture Code Level Diagrams](#4216-bounded-context-software-architecture-code-level-diagrams)
            - [4.2.X.6.1. Bounded Context Domain Layer Class Diagrams](#42161-bounded-context-domain-layer-class-diagrams)
            - [4.2.X.6.2. Bounded Context Database Design Diagram](#42162-bounded-context-database-design-diagram)

- [Conclusiones](#conclusiones)
   - [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)
- [Bibliografía](#bibliografía)

<hr class="page-break">

# Student Outcome

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 5

<table>
  <thead>
    <tr>
      <th>Criterio específico</th>
      <th>Acciones realizadas</th>
      <th>Conclusiones</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="5"><strong>Trabaja en equipo para proporcionar liderazgo en forma conjunta</strong></td>
      <td><strong>Crispin Ramos, Daniel Franco</strong><br><b>TB1:</b></td>
      <td rowspan="5"><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Ramirez Mestanza, Salim Ignacio</strong><br><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Rivera Sosa, Eduardo Gael</strong><br><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Sulca Gonzales, Paúl Fernando</strong><br><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Varela Bustinza, Marcelo Alessandro</strong><br><b>TB1:</b></td>
    </tr>
    <tr>
      <td rowspan="5"><strong>Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos</strong></td>
      <td><strong>Crispin Ramos, Daniel Franco</strong><br><b>TB1:</b></td>
      <td rowspan="5"><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Ramirez Mestanza, Salim Ignacio</strong><br><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Rivera Sosa, Eduardo Gael</strong><br><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Sulca Gonzales, Paúl Fernando</strong><br><b>TB1:</b></td>
    </tr>
    <tr>
      <td><strong>Varela Bustinza, Marcelo Alessandro</strong><br><b>TB1:</b></td>
    </tr>
  </tbody>
</table>

<hr class="page-break">

# Capítulo I: Introducción

## 1.1. Startup Profile
KinIoT es una startup peruana conformada por estudiantes de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC). Nuestra organización nace con el propósito de cerrar la brecha tecnológica en el sector salud, específicamente en el área de la medicina física y rehabilitación. Nos especializamos en el desarrollo de ecosistemas de Internet de las Cosas (IoT) y soluciones SaaS (Software as a Service) que transforman procesos terapéuticos convencionales en experiencias digitales precisas, seguras y monitoreadas.

Nuestro producto principal, uFlex, es una solución integral diseñada para la telerehabilitación de lesiones en el complejo articular de miembro superior. Mediante el uso de sensores vestibles de alta precisión y una plataforma cloud multitenant, permitimos que las clínicas y centros de salud extiendan su capacidad de atención al hogar del paciente, garantizando que cada movimiento sea auditado por especialistas y ejecutado correctamente por el usuario.

### Misión

Empoderar a pacientes y especialistas en rehabilitación mediante soluciones IoT innovadoras que garanticen la precisión clínica en el hogar, reduciendo los tiempos de recuperación y eliminando la incertidumbre en las terapias remotas.

### Visión

Ser reconocidos en el 2030 como la startup líder en telemonitoreo biomecánico en Latinoamérica, destacando por la integración de hardware de bajo costo y software de alta fidelidad para la salud articular.

### Valores

Integridad de datos: Nos comprometemos a que la información capturada por nuestros sensores sea un reflejo fiel del progreso del paciente.
Accesibilidad: Diseñamos tecnología compleja que sea fácil de usar para cualquier paciente, sin importar su experiencia técnica.
Enfoque en el paciente: Cada línea de código y cada componente de hardware tiene como fin último una recuperación sin secuelas.
Innovación constante: Buscamos optimizar continuamente nuestros algoritmos de procesamiento para ofrecer métricas cada vez más exactas.

### 1.1.1. Descripción de la Startup



### 1.1.2. Perfiles de los integrantes del equipo

<table>
  <thead>
    <tr>
      <th>Perfil</th>
      <th>Foto</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Rivera Sosa, Eduardo Gael</strong><br> Soy Gael, desarrollador Full Stack con enfoque en IA. Me gusta construir productos que realmente funcionen y aprender rápido lo que sea necesario para lograrlo. Soy proactivo, me adapto bien al trabajo en equipo y disfruto resolver problemas desde la raíz. Cuando algo se puede hacer mejor, lo digo.</td>
      <td><img src="assets/images/photos/gael-photo.jpg" alt="gael image" width="200"></td>
    </tr>
    <tr>
      <td><strong>[COMPLETAR: Apellidos, Nombres]</strong><br> [COMPLETAR: descripción]</td>
      <td><img src="img/[COMPLETAR].jpg" alt="[COMPLETAR]" width="200"></td>
    </tr>
    <tr>
      <td><strong>[COMPLETAR: Apellidos, Nombres]</strong><br> [COMPLETAR: descripción]</td>
      <td><img src="img/[COMPLETAR].jpg" alt="[COMPLETAR]" width="200"></td>
    </tr>
    <tr>
      <td><strong>[COMPLETAR: Apellidos, Nombres]</strong><br> [COMPLETAR: descripción]</td>
      <td><img src="img/[COMPLETAR].jpg" alt="[COMPLETAR]" width="200"></td>
    </tr>
    <tr>
      <td><strong>Varela Bustinza, Marcelo Alessandro</strong><br> Mi nombre es Marcelo Varela. Soy un estudiante de la carrera de Ingeniería De Software, tengo 21 años y actualmente me encuentro cursando el octavo ciclo de la carrera. Me caracterizo por ser una persona responsable, resiliente y proactiva, al cual le gusta aprender sobre tecnología y el desarrollo de software. Mi compromiso como miembro de este equipo es brindar mi apoyo y participación para enfrentar lo desafíos así como dar lo mejor de mí para el éxito de este proyecto.</td>
      <td><img src="img/[COMPLETAR].jpg" alt="[COMPLETAR]" width="200"></td>
    </tr>
  </tbody>
</table>

<hr class="page-break">

## 1.2. Solution Profile



### 1.2.1 Antecedentes y problemática

#### WHAT (Qué)

El principal problema es la falta de seguimiento preciso y continuo de la rehabilitación de fracturas de miembro superior en el domicilio del paciente, lo que genera riesgo de mala ejecución de ejercicios, recaídas, secuelas funcionales y prolongación de los tiempos de recuperación (Carbajal Galarza et al., 2021).
Muchos centros de rehabilitación en el Perú aún dependen de controles presenciales periódicos, dejando grandes lapsos de tiempo sin supervisión clínica efectiva entre sesiones, lo que limita la optimización del proceso terapéutico (MINSA, 2025b).

#### WHEN (Cuándo)

El problema se presenta principalmente durante la fase post‑operatoria o post‑inmovilización, cuando el paciente inicia una rutina de ejercicios diarios de forma autónoma en el domicilio, muchas veces sin supervisión directa del fisioterapeuta (Carbajal Galarza et al., 2021).
Es más evidente en pacientes que requieren terapias prolongadas (semanas o meses) y que, por limitaciones de movilidad, trabajo o distancia, acuden con menor frecuencia a los centros de rehabilitación, incrementando la probabilidad de técnicas incorrectas o de abandono parcial de la rutina (Andina, 2023).
El Instituto Nacional de Rehabilitación indica que el seguimiento del dolor, la inflamación y la progresión de los arcos de movilidad es crítico durante los primeros meses posteriores a la lesión, casi en forma continua, pero se pierde el control cuando el paciente no está en la clínica (INR, 2025).

#### WHERE (Dónde)

La problemática surge sobre todo en los hogares de los pacientes, especialmente en entornos urbanos como Lima Metropolitana, donde las barreras arquitectónicas y los tiempos de traslado dificultan la asistencia presencial frecuente a centros de rehabilitación (MVCS, 2022).
El problema también se origina en la brecha entre el instrumental clínico (goniómetros, plataformas de evaluación funcional) y el entorno domiciliario, donde la medición del movimiento se vuelve subjetiva o inexistente (León, 2023).
Además, la creciente demanda de telerehabilitación en el país muestra que más de 3 000 sesiones de terapia física se han realizado de forma remota en 2023 mediante el Centro Nacional de Telemedicina, evidenciando que la atención a distancia ya es un canal relevante pero aún sin sistemas de monitoreo biomecánico en tiempo real (Fernandez Agurto et al., 2025).

#### WHO (Quién)

El problema afecta principalmente a pacientes con lesiones de miembro superior que requieren rehabilitación prolongada, así como a fisioterapeutas que deben tomar decisiones clínicas sin datos objetivos entre sesiones presenciales. Según el MINSA (2019), en el Perú existen alrededor de 900 000 personas que presentan limitaciones de movilidad para usar brazos o piernas, lo que evidencia un grupo poblacional significativo que se vería beneficiado por sistemas de monitoreo remoto y estructurado.
Además, según Arias Tolentino (2022), las fracturas de extremidades son muy frecuentes en el Perú y representan más de la mitad de los pacientes con trauma, lo que implica que una alta proporción de rehabilitados requiere manejo cuidadoso de la función del miembro superior.

#### WHY (Por qué)

El problema se origina en la limitada adopción de tecnologías IoT y soluciones de telerehabilitación en el sistema de salud peruano, tanto público como privado, para el seguimiento continuo de la rehabilitación. Además, la falta de metodologías híbridas que integren de forma robusta la atención presencial con el monitoreo remoto hace que muchos programas dependan de reportes verbales o autoinformes del paciente, lo que reduce la precisión y la posibilidad de ajustar de forma oportuna la terapia (Carbajal Galarza et al., 2021).

#### HOW (Cómo)

El problema se diferencia del estado óptimo porque, en la práctica, la información sobre la rehabilitación domiciliaria se basa en la subjetividad del paciente, sin medición objetiva de rangos de movimiento, velocidad, repetición o patrones compensatorios (Carbajal Galarza et al., 2021).
Según explica Castro Villanueva (2023), el uso de sensores de carga y movimiento mejora de forma significativa la adherencia y la ejecución correcta de los ejercicios, lo que contrasta con la tendencia actual de sobrecargar el hombro o compensar movimientos de codo.
La tendencia no es aleatoria: se repite de forma sistemática en cada paciente que inicia una fase de rehabilitación domiciliaria prolongada sin herramientas de retroalimentación en tiempo real ni supervisión clínica continua (INR, 2025)

#### HOW MUCH (Cuánto)

El MINSA (2019) estima que más de 900 mil peruanos presentan limitaciones permanentes para mover brazos o piernas, lo que implica que una proporción importante de la población podría requerir rehabilitación de miembro superior y, por ende, seguimiento domiciliario.
A nivel macro, el sector de rehabilitación en Perú atiende cientos de miles de terapias al año, con un 68% de las atenciones cubiertas por el Seguro Integral de Salud, lo que refleja un volumen alto de pacientes que podrían beneficiarse de un sistema de seguimiento continuo (MINSA, 2025b).
En el caso de fracturas de extremidades, el INR (2020) señala que la rehabilitación debe ser continua y supervisada durante semanas o meses, lo que, a nivel de semanas por paciente, se traduce en cientos de miles de sesiones de ejercicio en casa que hoy se realizan sin medición objetiva ni registro centralizado.
Económicamente, una sesión de terapia individual cuesta entre S/ 100 y S/ 200 (Fisiofix, 2025). El incumplimiento de la terapia por falta de supervisión puede duplicar el tiempo de recuperación, incrementando los costos familiares en miles de soles anuales por complicaciones médicas mayores.


### 1.2.2 Lean UX Process

El Lean UX Process es una metodología ágil que prioriza el aprendizaje validado y la colaboración multidisciplinaria sobre la documentación exhaustiva. En el desarrollo de uFlex, aplicamos este enfoque para iterar rápidamente sobre la integración de hardware IoT y software, centrando el diseño en la reducción de la incertidumbre clínica y operativa mediante ciclos continuos de retroalimentación entre el paciente y el especialista.


#### 1.2.2.1. Lean UX Problem Statements

Nuestro servicio tiene como objetivo ofrecer un ecosistema de gestión y acompañamiento para la rehabilitación física traumatológica, permitiendo que las clínicas especializadas y sus pacientes mantengan una continuidad terapéutica eficiente fuera del entorno hospitalario. A través de nuestra plataforma, buscamos que los especialistas puedan supervisar el progreso biomecánico de sus pacientes de forma remota, asegurando que se cumplan los protocolos de recuperación establecidos para el miembro superior.
Hemos observado que un factor crítico que afecta el éxito de la rehabilitación y la eficiencia operativa de los centros de salud es la falta de datos objetivos y supervisión técnica durante los ejercicios realizados en el domicilio. Actualmente, existe una alta tasa de abandono de la terapia y una incidencia significativa de recuperaciones incompletas o erróneas, debido a que la información sobre el progreso del paciente se basa exclusivamente en reportes subjetivos y evaluaciones presenciales esporádicas. Esto impide que el tratamiento sea dinámico y preciso, generando incertidumbre tanto en el personal médico como en el usuario final.
¿Cómo podríamos mejorar la trazabilidad y la eficacia de las terapias remotas de miembro superior, logrando que los centros de salud y los pacientes cumplan sus objetivos de recuperación de manera informada y satisfactoria?

##### Domain:
La telerehabilitación y el monitoreo biomecánico remoto en el sector de medicina física y traumatología en el Perú.

##### Customer Segments:
- Administradores de Centros de Salud: Buscan optimizar la gestión de pacientes y la rentabilidad del servicio de terapia física.

- Fisioterapeutas: Requieren herramientas de seguimiento para validar y ajustar los protocolos de ejercicio basados en la evolución real.

- Pacientes en Rehabilitación: Personas con lesiones de codo o muñeca que necesitan guía y validación constante en sus hogares.

##### Pain Points:

- Incertidumbre Clínica: Desconocimiento de los rangos de movimiento reales alcanzados por el paciente en casa.

- Baja Adherencia: Desmotivación del paciente al no percibir un progreso medible o supervisado.

- Ineficiencia Operativa: Pérdida de tiempo en citas presenciales destinadas solo a verificar si el paciente realizó sus ejercicios básicos.

- Riesgo de Secuelas: Ejecución de movimientos compensatorios lesivos que no son detectados a tiempo.

##### Gap:

Existe una desconexión entre la prescripción médica en el consultorio y la ejecución física en el hogar, debido a la carencia de un sistema que capture e integre métricas articulares precisas en una plataforma de gestión centralizada.

##### Vision/Strategy:

Desarrollar una solución integral de monitoreo que combine tecnología de captura de movimiento con una plataforma de gestión multitenant. El enfoque estratégico es transformar la rehabilitación pasiva en un proceso basado en datos, donde la clínica mantenga el control operativo y el paciente reciba retroalimentación constante sobre su desempeño biomecánico.

##### Initial Segment:

Centros de rehabilitación física y clínicas traumatológicas privadas en Lima Metropolitana que ofrecen servicios de terapia ambulatoria para lesiones de miembro superior.


#### 1.2.2.2. Lean UX Assumptions

##### Business Assumptions

- Creo que mis clientes necesitan una forma de garantizar que la rehabilitación remota sea tan efectiva como la presencial, basándose en datos reales y no en suposiciones.


- Estas necesidades se pueden resolver con un ecosistema IoT reconfigurable de sensores sincronizado con una plataforma SaaS de gestión clínica.


- Mis clientes iniciales serán clínicas de fisioterapia y traumatología privadas en Lima que atienden a pacientes de los niveles socioeconómicos A y B.


- El valor #1 que un cliente quiere de mi servicio es la seguridad de una recuperación exitosa en menor tiempo gracias a la trazabilidad del movimiento.


- El cliente también puede obtener estos beneficios adicionales como reducción de costos de traslado, mayor disponibilidad de horarios para citas y una base de datos histórica de su evolución.


- Voy a adquirir la mayoría de mis clientes a través de venta directa B2B a directores de clínicas y marketing digital segmentado para centros de salud especializados.


- Haré dinero a través de un modelo híbrido de pago por kit de hardware (One-time fee) y una suscripción mensual por el uso del software SaaS (Fee por paciente activo).


- Mi competencia principal en el mercado serán centros de terapia física que usan métodos tradicionales (papel/video) y aplicaciones genéricas de fitness sin hardware especializado.


- Los venceremos debido a la precisión biomecánica de nuestros sensores vestibles y la capacidad de la clínica de autogestionar su propio ecosistema de datos.


- Mi mayor riesgo de producto es la resistencia al cambio por parte de fisioterapeutas tradicionales y la posible dificultad de algunos pacientes para configurar el hardware IoT.


- Resolveremos esto a través de un diseño Plug-and-Play simplificado, videos tutoriales integrados en la app y un soporte técnico especializado para la clínica.


##### User Assumptions

- ¿Quién es el usuario? Pacientes de 18 a 65 años con lesiones de miembro superior, fisioterapeutas (especialista clínico) y administradores de clínicas.


- ¿Dónde encaja nuestro producto en su trabajo o vida? En el caso del paciente, encaja en su rutina diaria de ejercicios en el hogar. Para el fisioterapeuta, en su flujo de supervisión y toma de decisiones clínicas asíncronas. Para el administrador, en el control de activos y rentabilidad del centro.


- ¿Qué problemas resuelve nuestro producto? Resuelve la falta de precisión en la medición de ángulos articulares fuera del consultorio, el miedo del paciente a realizar ejercicios incorrectos y la pérdida de ingresos de las clínicas por deserción de pacientes en tratamiento remoto.


- ¿Cuándo y cómo es usado nuestro producto? El hardware se usa durante las sesiones de ejercicio (20-40 min diarios). La aplicación móvil se usa para dar feedback en tiempo real y la aplicación web es consultada por el médico periódicamente para auditar el progreso.


- ¿Qué características son importantes? La precisión de los sensores (tolerancia de error < 5%), la facilidad de emparejamiento Bluetooth y la visualización de gráficos comparativos.


- ¿Cómo debe verse nuestro producto y cómo comportarse? La aplicación móvil debe ser intuitiva, con elementos visuales claros (gamificación) para guiar el movimiento. La aplicación debe ser profesional, de alta densidad de datos pero fácil de navegar.


#### 1.2.2.3. Lean UX Hypothesis Statements

##### Business Hypothesis Statement

- Hypothesis 01:
Creemos que el desarrollo de una plataforma SaaS multitenant con hardware IoT reconfigurable para clínicas de traumatología logrará que los centros de salud reduzcan su tasa de deserción de pacientes en un 25% y optimicen el tiempo de consulta de sus especialistas.
Sabremos que hemos tenido éxito cuando veamos que al menos 5 clínicas locales solicitan una demostración del sistema y recibamos reportes mensuales de un incremento en la retención de pacientes que iniciaron su terapia remota con uFlex.

##### Features Hypothesis Statement

- Hypothesis 02:
Creemos que proporcionar una aplicación web con dashboard y gráficos de ángulos articulares (ROM) capturados por sensores inerciales permitirá que los fisioterapeutas realicen ajustes precisos en los protocolos de ejercicio sin necesidad de una cita presencial semanal.
Sabremos que esto es cierto cuando veamos que el 80% de los especialistas encuestados afirman tener mayor confianza en la toma de decisiones clínicas y se registre una reducción del 30% en el tiempo promedio de evaluación manual con goniómetro en el consultorio.


- Hypothesis 03:
Creemos que la implementación de feedback visual en tiempo real y elementos de gamificación en la aplicación móvil logrará que los pacientes con fracturas de codo o muñeca realicen sus rutinas de ejercicio de manera autónoma y correcta.
Sabremos que esto es cierto cuando veamos que los logs del sistema muestran que el 90% de los pacientes completan sus repeticiones diarias dentro de los rangos de movimiento permitidos, reduciendo la percepción de dolor reportada en la aplicación en un 15% tras las primeras dos semanas.


- Hypothesis 04:
Creemos que el sistema de aprovisionamiento automático de dispositivos (ID de kit vinculado a la clínica) facilitará la escalabilidad del negocio de la startup y la gestión de inventario para el administrador de la clínica.
Sabremos que esto es cierto cuando veamos que el tiempo de configuración inicial (onboarding) de un nuevo kit IoT por parte del administrador es menor a 5 minutos y no se reportan incidencias de vinculación manual entre el sensor y la cuenta del paciente.


#### 1.2.2.4. Lean UX Canvas

A continuación, se presenta el Lean UX Canvas elaborado en la herramienta Miro:

<img src="/assets/images/screenshots/LeanUxCanvas.png" alt="LeanUxCanvas.png">

Enlace al Lean UX Canvas:
https://miro.com/app/board/uXjVGuekPgY=/?share_link_id=263966947817 

<hr class="page-break">

## 1.3. Segmentos objetivo

En el análisis de los segmentos objetivo de KinIoT, hemos identificado tres grupos clave que conforman el ecosistema de uFlex: pacientes en rehabilitación, especialistas en fisioterapia y administradores de centros de salud.

### Pacientes en rehabilitación de miembro superior

Este segmento integra a personas que han sufrido lesiones traumáticas como fracturas de codo o muñeca y requieren recuperar la funcionalidad del miembro superior, constituyendo el usuario final que interactúa con el hardware IoT y la aplicación móvil.

La mayoría se encuentra en el rango de adultos económicamente activos con acceso frecuente a Internet y smartphones, lo que valida la viabilidad de una solución basada en app móvil y conectividad Bluetooth para el hogar (INEI, 2025; OSIPTEL, 2024).

- **Edad:** Adultos de 18 a 65 años, con énfasis en población activa y adultos mayores con riesgo de caídas y fracturas (INEI, 2022).
- **Necesidad clave:** Guía técnica precisa y retroalimentación inmediata para realizar ejercicios correctamente en casa, reduciendo el miedo al movimiento (kinesiofobia) y evitando compensaciones biomecánicas.
- **Nivel educativo:** Grado de instrucción variado, capaz de seguir instrucciones visuales y auditivas sin requerir altos niveles de formación técnica.
- **Uso de tecnología:** Usuarios habituales de smartphones, con alto uso de dispositivos móviles en el hogar, que prefieren interfaces simplificadas y tecnologías de conexión plug‑and‑play (INEI, 2025; OSIPTEL, 2024).

### Fisioterapeutas y especialistas en rehabilitación

Los fisioterapeutas y especialistas en rehabilitación son los usuarios operativos que toman decisiones clínicas basadas en los datos capturados por el sistema, ajustando protocolos de tratamiento entre sesiones presenciales (Rosales et al., 2023). La creciente demanda de atención y la expansión de la telemedicina en el Perú refuerzan la necesidad de herramientas de telemonitorización que permitan supervisar el progreso del paciente de forma objetiva (MINSA, 2025).

- **Edad:** Profesionales de 24 a 55 años, con formación en Tecnología Médica, Terapia Física y Rehabilitación (Rosales et al., 2023).
- **Necesidad clave:** Obtener métricas objetivas (ángulos de ROM, simetría de movimientos, número de repeticiones correctas) para ajustar protocolos y reducir complicaciones.
- **Nivel educativo:** Formación universitaria en salud y rehabilitación, con alta familiaridad con el manejo de información clínica.
- **Uso de tecnología:** Manejo intermedio de plataformas digitales de gestión clínica, con preferencia por dashboards intuitivos y reportes exportables, ya que según estudios en Lima Metropolitana, alrededor de la mitad no adoptó la práctica digital durante la pandemia sin suficiente apoyo institucional (Rosales et al., 2023).

### Administradores de clínicas y centros de salud

Este segmento agrupa a los tomadores de decisiones B2B que gestionan la operación y la rentabilidad de clínicas y centros de salud privados, encargados de la adopción de soluciones tecnológicas como sistemas IoT y SaaS (MINSA, 2025a). La consolidación de la telemedicina y la alta penetración de dispositivos móviles en el hogar peruano respaldan la viabilidad económica de sistemas de monitoreo remoto para mejorar la retención de pacientes y la eficiencia operativa (INEI, 2025; OSIPTEL, 2024).

- **Edad:** Profesionales de 30 a 60 años, con formación en Administración de Salud, Gestión Empresarial o Medicina.
- **Necesidad clave:** Reducir la tasa de abandono de tratamientos, aumentar la productividad del personal clínico y gestionar eficientemente el inventario de equipos tecnológicos.
- **Nivel educativo:** Formación superior en administración, gestión o área clínica, con experiencia en toma de decisiones estratégicas.
- **Uso de tecnología:** Interés en soluciones SaaS multi‑tenant que permitan controlar múltiples sedes y cuentas de usuario desde una sola consola, alineándose con la tendencia de digitalización del sistema de salud peruano (MINSA, 2025a; INEI, 2025).

<hr class="page-break">

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores



### 2.1.1. Análisis competitivo

<table>
  <tr>
    <th colspan="6">Competitive Analysis landscape</th>
  </tr>
  <tr>
    <td colspan="2" align="center"><b>¿Por qué llevar a cabo este análisis?</b></td>
    <td colspan="4">¿De qué manera puede KinIoT diferenciarse de las soluciones de rehabilitación digital actuales mediante el uso de tecnología IoT para capturar datos cuantitativos precisos, superando las barreras de alto costo y falta de biofeedback en tiempo real que presentan los competidores en el mercado peruano?</td>
  </tr>
  <tr>
    <th colspan="2">Nombre</th>
    <th>KinIoT</th>
    <th>Sword Health</th>
    <th>Hinge Health</th>
    <th>Physitrack</th>
  </tr>
  <tr>
    <td colspan="2" align="center"><b>Logo</b></td>
    <td align="center"><img src="img/kiniot-logo.png" alt="KinIoT logo" width="100"></td>
    <td align="center"><img src="img/sword-logo.png" alt="Sword Health logo" width="100"></td>
    <td align="center"><img src="img/hinge-logo.png" alt="Hinge Health logo" width="100"></td>
    <td align="center"><img src="img/physitrack-logo.png" alt="Physitrack logo" width="100"></td>
  </tr>
  <tr>
    <td rowspan="2"><b>Perfil</b></td>
    <td><b>Overview</b></td>
    <td>Ecosistema IoT y SaaS para telerehabilitación con monitoreo biomecánico en tiempo real</td>
    <td>Líder global en terapia física digital con sensores de grado clínico y supervisión médica</td>
    <td>Clínica digital integral que usa sensores y visión computarizada para el cuidado articular</td>
    <td>Plataforma SaaS global para prescripción de ejercicios y seguimiento de resultados mediante video</td>
  </tr>
  <tr>
    <td><b>Ventaja competitiva ¿Qué valor ofrece a los clientes?</b></td>
    <td>Monitoreo cuantitativo preciso mediante sensores físicos a un costo accesible para el mercado local</td>
    <td>IA avanzada y sensores de alta fidelidad con validación clínica masiva en mercados premium</td>
    <td>Ecosistema híbrido que combina sensores físicos con visión artificial "TrueMotion"</td>
    <td>Marca establecida con una de las bibliotecas de ejercicios clínicos más grandes del mundo</td>
  </tr>
  <tr>
    <td rowspan="2"><b>Perfil de Marketing</b></td>
    <td><b>Mercado objetivo</b></td>
    <td>Centros de salud, Fisioterapeutas y pacientes con lesiones de miembro superior.</td>
    <td>Grandes corporaciones y planes de salud empresariales en EE. UU. y Europa</td>
    <td>Empleadores y planes de salud que buscan reducir costos por cirugías innecesarias</td>
    <td>Fisioterapeutas independientes y clínicas de tamaño medio a nivel global</td>
  </tr>
  <tr>
    <td><b>Estrategias de Marketing</b></td>
    <td>B2B enfocado en reducir la deserción y optimizar el tiempo de evaluación manual.</td>
    <td>Enfoque en el ahorro de costos para empleadores al evitar cirugías innecesarias</td>
    <td>Marketing basado en la reducción del dolor crónico y programas preventivos corporativos</td>
    <td>Marketing digital masivo y alianzas con asociaciones profesionales de fisioterapia</td>
  </tr>
  <tr>
    <td rowspan="3"><b>Perfil de Producto</b></td>
    <td><b>Productos &amp; Servicios</b></td>
    <td>Kinetic Track: Nodos vestibles (IoT) + App móvil con gamificación + Dashboard Web.</td>
    <td>Plataforma de "Terapeuta Digital", sensores propios y programas especializados como Bloom</td>
    <td>Sensores de movimiento, programas de coaching de salud y visión computarizada</td>
    <td>Aplicación para prescripción de ejercicios, telemedicina y seguimiento de adherencia</td>
  </tr>
  <tr>
    <td><b>Precios y Costos</b></td>
    <td>Pago por kit de hardware + Suscripción mensual por paciente activo (SaaS)</td>
    <td>Modelo de precios premium orientado a contratos corporativos de alto volumen</td>
    <td>Modelo de suscripción B2B de alto nivel para grandes beneficios corporativos</td>
    <td>Suscripción de bajo costo por profesional de la salud.</td>
  </tr>
  <tr>
    <td><b>Canales de distribución</b></td>
    <td>Web para especialistas y Administradores; App Móvil para pacientes.</td>
    <td>Ecosistema cerrado de Hardware, Tablet y Aplicaciones Móviles</td>
    <td>Aplicaciones móviles integradas con hardware y cámara</td>
    <td>Aplicaciones Web y Móviles multiplataforma</td>
  </tr>
  <tr>
    <td rowspan="4"><b>Análisis SWOT</b></td>
    <td><b>Fortalezas</b></td>
    <td>Captura de datos biomecánicos precisos que elimina la subjetividad clínica y enfoque específico en lesiones de miembro superior, permitiendo algoritmos más exactos</td>
    <td>Capital masivo, algoritmos de IA de vanguardia y validación clínica de nivel superior</td>
    <td>Utiliza una combinación avanzada de sensores vestibles y visión computarizada a través de la cámara del smartphone para corregir la postura en tiempo real</td>
    <td>Gran base de usuarios instalada y reconocimiento de marca global</td>
  </tr>
  <tr>
    <td><b>Oportunidades</b></td>
    <td>Alta penetración de smartphones y demanda de telemedicina en el hogar peruano</td>
    <td>Expansión a Latinoamérica mediante alianzas con aseguradoras globales.</td>
    <td>Aunque domina el mercado estadounidense, tiene una gran oportunidad de crecimiento en regiones como Latinoamérica</td>
    <td>Integrar visión computarizada para actualizar su propuesta tecnológica</td>
  </tr>
  <tr>
    <td><b>Debilidades</b></td>
    <td>Marca nueva en el mercado sin historial extenso de datos clínicos acumulados</td>
    <td>Precio prohibitivo para el mercado de clínicas pequeñas (MYPES) en regiones emergentes como Perú</td>
    <td>Su modelo de negocio está diseñado para grandes corporaciones (B2B), lo que resulta económicamente inviable para clínicas pequeñas o independientes</td>
    <td>Carece de herramientas de biofeedback en tiempo real o sensores de movimiento</td>
  </tr>
  <tr>
    <td><b>Amenazas</b></td>
    <td>Resistencia al cambio por parte de fisioterapeutas con métodos tradicionales analógicos</td>
    <td>Competencia agresiva de Hinge Health en el sector corporativo</td>
    <td>Usuarios que requieran mayor precisión clínica (IoT) para patologías complejas</td>
    <td>El surgimiento de sensores IoT de bajo costo y alta precisión que pueden democratizar el acceso a la tecnología que antes eran exclusivas</td>
  </tr>
</table>

### 2.1.2. Estrategias y tácticas frente a competidores

En esta sección se detallan las estrategias y tácticas que KinIoT aplicará para establecer una ventaja competitiva en el sector de la telerehabilitación biomecánica.

**Estrategias para afrontar las fortalezas de los competidores**

- **Diferenciación por Precisión Articular Específica:** Para enfrentar la fortaleza de Hinge Health y su tecnología de visión artificial, KinIoT aplicará la táctica de "Validación Biomecánica por Sensores Inerciales". Dado que la visión por cámara puede perder precisión ante oclusiones físicas, nuestros sensores físicos garantizan una captura de datos del Rango de Movimiento (ROM) con un margen de error menor al 5%, lo cual es fundamental para la rehabilitación de codo y muñeca.

- **Estrategia de Accesibilidad B2B Local:** Ante el dominio de Sword Health en mercados corporativos de alto nivel, implementaremos una táctica de "Aprovisionamiento de Bajo Costo para MYPES". Nos enfocaremos en clínicas privadas de Lima Metropolitana ofreciendo un modelo de pago por kit de hardware y una suscripción SaaS escalable, permitiendo que centros locales adopten tecnología de punta sin la inversión prohibitiva de los competidores globales.

**Estrategias para aprovechar las debilidades de los competidores**

- **Táctica de Biofeedback Activo en Tiempo Real:** Aprovecharemos la debilidad de Physitrack, que se limita al seguimiento pasivo basado en videos, mediante la implementación de corrección postural inmediata. La aplicación móvil de Kinetic Track proporcionará alertas visuales y gamificadas que guiarán al paciente durante la ejecución del ejercicio, asegurando que se cumplan los protocolos terapéuticos y reduciendo el riesgo de movimientos compensatorios lesivos.

- **Estrategia de Fidelización basada en Datos Objetivos:** Capitalizaremos la falta de métricas cuantitativas en las terapias tradicionales para ofrecer a los fisioterapeutas un dashboard de alta densidad de datos. Esto les permitirá ajustar los planes de tratamiento basados en evidencia clínica real, mejorando la adherencia del paciente y reduciendo la tasa de deserción que afecta la rentabilidad de las clínicas.

**Contexto de Oportunidades y Amenazas**

- **Oportunidades:** Aprovecharemos la alta penetración de smartphones en los hogares peruanos (94.8%) y el crecimiento de las atenciones por telemedicina (más de 3.4 millones recientemente) para posicionar la telerehabilitación como un estándar accesible.

- **Amenazas:** Para mitigar la resistencia al cambio de los especialistas tradicionales, se aplicará una táctica de "Onboarding y Soporte Especializado", demostrando mediante informes automáticos cómo nuestra herramienta reduce en un 30% el tiempo de evaluación manual en el consultorio.

<hr class="page-break">

## 2.2. Entrevistas



### 2.2.1. Diseño de entrevistas



### 2.2.2. Registro de entrevistas



### 2.2.3. Análisis de entrevistas



<hr class="page-break">

## 2.3. Needfinding



### 2.3.1. User Personas

Esta sección presenta nuestros usuarios ideales diseñados para el ecosistema de KinIoT. Estos artefactos se han construido a partir del análisis del mercado peruano de salud, el comportamiento de las clínicas privadas y las barreras de accesibilidad en la rehabilitación física.

**User persona del segmento de pacientes en rehabilitación del miembro superior**

<img src="img/user-persona-paciente.png" alt="User Persona Paciente" width="800">

**User persona del segmento de fisioterapeuta**

<img src="img/user-persona-fisioterapeuta.png" alt="User Persona Fisioterapeuta" width="800">

**User persona del segmento de administradores de clínica y centros de salud**

<img src="img/user-persona-administrador.png" alt="User Persona Administrador" width="800">

### 2.3.2. User Task Matrix



### 2.3.3. User Journey Mapping



### 2.3.4. Empathy Mapping



<hr class="page-break">

## 2.4. Big Picture EventStorming



<hr class="page-break">

## 2.5. Ubiquitous Language

<hr class="page-break">

# Capítulo III: Requirements Specification

## 3.1. User Stories



<hr class="page-break">

## 3.2. Impact Mapping



<hr class="page-break">

## 3.3. Product Backlog



<hr class="page-break">

# Capítulo IV: Solution Software Design



## 4.1. Strategic-Level Domain-Driven Design



### 4.1.1. Design-Level EventStorming



#### 4.1.1.1 Candidate Context Discovery



#### 4.1.1.2 Domain Message Flows Modeling



#### 4.1.1.3 Bounded Context Canvases



<hr class="page-break">

### 4.1.2. Context Mapping



<hr class="page-break">

### 4.1.3. Software Architecture



#### 4.1.3.1. Software Architecture System Landscape Diagram



#### 4.1.3.2. Software Architecture Context Level Diagrams



#### 4.1.3.3. Software Architecture Container Level Diagrams



#### 4.1.3.4. Software Architecture Deployment Diagrams



<hr class="page-break">

## 4.2. Tactical-Level Domain-Driven Design



### 4.2.X. Bounded Context: <Bounded Context Name>



#### 4.2.X.1. Domain Layer



#### 4.2.X.2. Interface Layer



#### 4.2.X.3. Application Layer



#### 4.2.X.4. Infrastructure Layer



#### 4.2.X.5. Bounded Context Software Architecture Component Level Diagrams



#### 4.2.X.6. Bounded Context Software Architecture Code Level Diagrams



##### 4.2.X.6.1. Bounded Context Domain Layer Class Diagrams



##### 4.2.X.6.2. Bounded Context Database Design Diagram

<hr class="page-break">

# Conclusiones



## Conclusiones y recomendaciones



<hr class="page-break">

# Bibliografía



<hr class="page-break">