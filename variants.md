# 1) Experience level (Access Right)
**An access rights policy depending on coordinators experience level crisis management should be proposed to allocate crisis and alert to coordinators.**

---

* Se define el nivel de experiencia de cada coordinador. El administrador del sistema determinará el nivel inicial de cada coordinador que se cree en el sistema.

* Cada crisis tendrá asignado un puntaje (q1- cómo es este puntaje asignado: i.e. politica de puntuaje de una crisis; quién se encarga de asignar dicho puntaje?). Luego cuando una crisis sea atendida por un coordinador, éste aumenta la valoración de su experiencia de acuerdo al puntaje de la crisis atendida, de esta forma podemos generar una relación entre la cantidad de puntos de experiencia y el nivel de experiencia alcanzado.

* Cada crisis será puntuada y sólo los coordinadores con cierto nivel de experiencia podrán atenderla. Si no existe coordinador con nivel de experiencia necesario para atender una crisis, se le asignará el coordinador con mayor puntos de experiencia del nivel inmediatamente anterior.

* r1: La crisis será categorizada como: compleja, intermedia o simple. El sistema determinará su puntaje de acuerdo a la cantidad de alertas que se reciban para esa crisis, sumando 10 puntos por cada alerta recibida de la crisis, la pertenecia de una alerta a una crisis se determinará de acuerdo a su ubicación.

Entonces la categorización de una crisis será la siguiente:

Categoría | Puntaje (p)
------------ | -------------
Compleja | p >= 200
Intermedia | 50 < p < 200
Simple | 0 < p <= 50

# 2) Police (Info Diffusion)
**Some carefully selected information on the crisis and alerts should be made available to the Police headquarters for its diffusion**

---

* Añadir un campo de texto en la gestión de la crisis para realizar una difusión pública de los hechos.

* La información de ese campo podrá ser validada con un conjunto de palabras críticas (q2: cómo se determina ese conjunto de palabras críticas?) para evitar que se publique información privada o sensible que pueda afectar a los involucrados del hecho. Luego de esa verificiación, el contenido será remitido via email a la seccional de policía correspondiente (q3- cómo son las seccionales añadidas al sistema?) de acuerdo a la ubicación del evento.

* El conjunto de palabras críticas podrá ser extraído a partir de la información recibida en las alertas de la crisis.

* r2: Los campos de datos personales en la entrada de usuario para crear una alerta determinarán el conjunto de palabras críticas que contiene la información que debe evitar ser difundida. Además, puede advertirse al usuario de no ingresar datos personales en los campos que se utilizarían para difundir la información a distintas instituciones.

* r3: Las seccionales de policía se ingresan al sistema desde el panel del administrador, quien por su parte será el encargado de esta tarea, y donde deberán proporcionarse entre otros datos el nombre de la seccional, la ubicación (coordenadas), email, etc.
