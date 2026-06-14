# THESRAPTO
## Ecosistema Modular Híbrido Multidimensional

**Creador:** Luis Ángel Astengo Sanchez  
**País:** Perú  
**Fecha de concepción:** Abril 2026  
**Fecha de documentación:** Junio 2026  
**Repositorio inicial:** MP3_unomas (github.com/LuisAngel4254/MP3_unomas)

---

## ¿Qué es Thesrapto?

Thesrapto es una arquitectura de software modular híbrida multidimensional, concebida y desarrollada empíricamente por Luis Ángel Astengo Sanchez durante el desarrollo de un reproductor de música en Flutter para Android.

No parte de teoría matemática ni académica. Parte de la observación directa de cómo los sistemas deberían funcionar: un cerebro liviano que evoca módulos según la necesidad del usuario, liberándolos cuando no se usan, sin saturar recursos.

---

## La Analogía del Cubo

La estructura se entiende mejor con una imagen:

Toma un **Cubo de Rubik**. Cada cara exterior es una función visible para el usuario. Al seleccionar una cara, esta se abre y revela 6 caras internas — sus módulos propios. Cada módulo interno puede a su vez contener sus propias caras.

Un cubo → 6 caras externas  
Cada cara → 6 caras internas  
Total primer nivel → 36 nodos funcionales  
Escalable infinitamente sin romper la estructura base

Esto no es navegación lineal (A→B→C). Es navegación multidimensional — desde cualquier punto puedes acceder a cualquier módulo directamente, como girar el cubo a la cara que necesitas.

---

## Principios Fundamentales

**1. Cerebro Liviano**  
El núcleo (main/cerebro) contiene únicamente las funciones esenciales de sistema. No ejecuta funciones que no están siendo usadas. Su único trabajo es coordinar.

**2. Módulos Evocables**  
Cada función vive en su propio módulo independiente. El cerebro los llama cuando el usuario los necesita y los libera cuando no.

**3. Capas Core y Modules**  
- `core/` → módulos permanentes de sistema (permisos, archivos, playlist, volumen)  
- `modules/` → módulos evocables según interacción del usuario (reproductor, ecualizador, tipos de reproducción, velocidad, voz)

**4. Botones como Detectores de Módulos**  
Un botón visible en pantalla indica que su módulo existe y está disponible. Si el módulo no existe, el botón no aparece o está inactivo. La interfaz refleja la realidad del sistema en tiempo real.

**5. Hibridez**  
La arquitectura no depende del hardware subyacente. Puede ejecutarse sobre Android, sobre una API externa, sobre un LLM local, o sobre cualquier combinación de estos. Es portable por diseño.

**6. Escalabilidad sin ruptura**  
Agregar un módulo nuevo no modifica el cerebro ni los módulos existentes. El ecosistema crece sin romper lo que ya funciona.

---

## Aplicaciones del Ecosistema

La misma arquitectura base sirve para construir:

- Reproductores multimedia (audio, video, fotos)
- Asistentes personales con IA y voz
- Gestores de productividad y tareas
- Sistemas operativos móviles alternativos
- Herramientas de desarrollo móvil
- Clientes de comunicación modulares
- Automatizadores de tareas
- Cualquier sistema que requiera funciones independientes coordinadas por un núcleo central

---

## Implementación Actual

El primer prototipo funcional es **MP3_unomas**, un reproductor de música para Android construido 100% desde un teléfono Redmi Note 13 4G, editando código en GitHub desde el navegador y compilando con GitHub Actions — sin PC, sin IDE de escritorio.

**Stack tecnológico inicial:**
- Flutter / Dart
- Android (compilación vía GitHub Actions)
- just_audio, permission_handler, volume_controller

**Estado actual (Junio 2026):**
- Reproducción de música funcional
- Carga automática de playlist desde almacenamiento
- Control de volumen del sistema
- Navegación por playlist
- Reproducción continua automática
- Barra de progreso funcional

---

## Nota de Autoría

Esta arquitectura fue concebida, nombrada y documentada por **Luis Ángel Astengo Sanchez**, Perú, en el período Abril-Junio 2026.

El desarrollo es autodidacta. No existe formación universitaria en sistemas ni programación formal. La arquitectura emergió de la necesidad práctica y la observación directa, no de la teoría académica.

La evidencia de autoría y fechas se encuentra en los commits del repositorio GitHub bajo el usuario LuisAngel4254, con registros desde Abril 2026.

---

*"La diferencia es que el matemático describe la estructura. Yo la uso."*  
— Luis Ángel Astengo Sanchez, Junio 2026
