# 1) Experience level (Access Right)
**An access rights policy depending on coordinators experience level crisis management should be proposed to allocate crisis and alert to coordinators.**

---

* Se define el nivel de experiencia de cada coordinador. El administrador del sistema determinará el nivel inicial de cada coordinador que se cree en el sistema.

* Cada crisis tendrá asignado un puntaje. Cuando una crisis sea atendida por un coordinador, éste aumenta la valoración de su experiencia de acuerdo al puntaje de la crisis atendida, de esta forma podemos generar una relación entre la cantidad de puntos de experiencia y el nivel de experiencia alcanzado.

* Cada crisis será puntuada y sólo los coordinadores con cierto nivel de experiencia podrán atenderla. Si no existe coordinador con nivel de experiencia necesario para atender una crisis, se le asignará el coordinador con mayor puntos de experiencia del nivel inmediatamente anterior.

* La crisis será categorizada como: compleja, intermedia o simple. El sistema determinará su puntaje de acuerdo a la cantidad de alertas que se reciban para esa crisis, sumando 10 puntos por cada alerta recibida de la crisis, la pertenecia de una alerta a una crisis se determinará de acuerdo a su ubicación.

Entonces la categorización de una crisis será la siguiente:

Categoría | Puntaje (p)
------------ | -------------
Compleja | p >= 250
Intermedia | 50 < p < 250
Simple | 0 < p <= 50

El nivel de experiencia se determina de acuerdo a la cantidad de puntos alcanzados por el coordinador, que es un número entero asociado a cada coordinador y, por lo tanto, define una relacion de orden entre ellos: A > B > C

Nivel de experiencia | Puntos de EXP
--|--
A | 2000 <= EXP
B | 500 < EXP < 2000
C | 500 <= EXP

El sistema emitirá la notificación de atención a los coordinadores de acuerdo el nivel de experiencia alcanzado. La relación es la siguiente:

Clase de crisis | Nivel de experiencia necesario
-- | --
Compleja | A
Intermedia | B
Simple | C


# 2) Police (Info Diffusion)
**Some carefully selected information on the crisis and alerts should be made available to the Police headquarters for its diffusion**

---

* Añadir un reporte asociado a cada crisis para realizar la difusión pública de los hechos.

* Los coordinadores serán encargados de crear el reporte para evitar que se publique información privada o sensible que pueda afectar a los involucrados del hecho. El reporte generado podrá ser remitido via email a la seccional de policía más cercana a la ubicación del evento.

* Cada crisis tendrá asociado a lo sumo un reporte y el estado de envío. Un coordinador podrá crear un nuevo reporte para la crisis si y sólo si el reporte anterior fue enviado. Caso contrario deberá modificar el reporte ya existente.

* La información del reporte será extraída a partir de los datos recibidos en las alertas de esa crisis.

* Los administradores de iCrash serán los encargados de registar las seccionales en el sistema. Para realizar esta tarea deberán contar con datos como el nombre de la seccional, email y la ubicación (coordenadas).
