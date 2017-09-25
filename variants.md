# 1) Experience level (Access Right)
**An access rights policy depending on coordinators experience level crisis management should be proposed to allocate crisis and alert to coordinators.**

---

* Se definirá el nivel de experiencia de cada coordinador. El administrador del sistema puede ser el encargado de esto o automáticamente se podrá asignar de acuerdo a las crisis que haya podido resolver, este último enfoque presentaría la desventaja del arranque en frío. Por lo que me parece más conveniente que el administrador determine el nivel inicial de cada coordinador que se cree en el sistema. 

* Cada crisis tendrá asignado un puntaje (q1- cómo es este puntaje asignado: i.e. politica de puntuaje de una crisis; quién se encarga de asignar dicho puntaje?). Luego cuando una crisis sea atendida por un coordinador, éste aumenta la valoración de su experiencia de acuerdo al puntaje de la crisis atendida, de esta forma podemos generar una relación entre la cantidad de puntos de experiencia y el nivel de experiencia alcanzado.

* Cada crisis será puntuada y sólo los coordinadores con cierto nivel de experiencia podrán atenderla.


# 2) Police (Info Diffusion)
**Some carefully selected information on the crisis and alerts should be made available to the Police headquarters for its diffusion**

---

* Añadir un campo de texto en la gestión de la crisis para realizar una difusión pública de los hechos.

* La información de ese campo podrá ser validada con un conjunto de palabras críticas (q2: cómo se determina ese conjunto de palabras críticas?) para evitar que se publique información privada o sensible que pueda afectar a los involucrados del hecho. Luego de esa verificiación, el contenido será remitido via email a la seccional de policía correspondiente (q3- cómo son las seccionales añadidas al sistema?) de acuerdo a la ubicación del evento.

* El conjunto de palabras críticas podrá ser extraído a partir de la información recibida en las alertas de la crisis.
