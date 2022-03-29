# DRIVERS ARQUITECTONICOS

- **Atributos de calidad**
  - Mapa de empatía
        1. *Priorización de requisitos*
        ![MapaEmp](/assets/images/PriorizacióndeRequisistos.PNG)
        2. *Grafico radar*
        ![MapaEmp](/assets/images/GraficoRadar.PNG)
  - Por cada atributo priorizado
    - Confiabilidad = Reliabiliy
        1. Definición
        Capacidad del sistema para permanecer operativo a lo largo del tiempo, brindando información correcta y relevante
        2. Características
        ![MapaEmp](/assets/images/Caracteristicas.PNG)
            1. Escenarios de Calidad 1
            ![esc](/assets/images/Confiabilidad1.PNG)
            2. Escenarios de calidad 2
             ![esc](/assets/images/Confiabilidad2.PNG)
            3. Escenarios de Calidad 3
             ![esc](/assets/images/Confiabilidad3.PNG)
            4. Escenarios de calidad 4
             ![esc](/assets/images/Confiabilidad4.PNG)
            5. Escenarios de Calidad 5
             ![esc](/assets/images/Confiabilidad5.PNG)
            6. Escenarios de calidad 6
             ![esc](/assets/images/Confiabilidad6.PNG)
            7. Escenarios de Calidad 7
             ![esc](/assets/images/Confiabilidad7.PNG)
    - Mantenibilidad
        1. Definición
        Facilidad del sistema para incorporar los combios por nueva funcionalidad o para corrección de errores
        2. Características
        ![MapaEmp](/assets/images/CaracteristicasM.PNG)
            1. Escenarios de Calidad 1
            ![esc](/assets/images/Mantenibilidad1.PNG)
            2. Escenarios de calidad 2
             ![esc](/assets/images/Mantenibilidad2.PNG)
            3. Escenarios de Calidad 3
             ![esc](/assets/images/Mantenibilidad3.PNG)
    - Disponibilidad
        1. Definición
        condicion de estar disponible para su uso
        2. Características
        ![MapaEmp](/assets/images/CaracteristicasD.PNG)
            1. Escenarios de Calidad 1
            ![esc](/assets/images/Disponibilidad1.PNG)
            2. Escenarios de calidad 2
             ![esc](/assets/images/Disponibilidad2.PNG)
            3. Escenarios de Calidad 3
             ![esc](/assets/images/Disponibilidad3.PNG)
            4. Escenarios de Calidad 4
             ![esc](/assets/images/Disponibilidad4.PNG)
    - Rendimiento
        1. Definición
         es un indicador de la capacidad de respuesta del sistema para ejecutar una acción dentro de un intervalo de tiempo dado.
        2. Características
        ![MapaEmp](/assets/images/CaracteristicasR.PNG)
            1. Escenarios de Calidad 1
            ![esc](/assets/images/Rendimiento1.PNG)
            2. Escenarios de calidad 2
             ![esc](/assets/images/Rendimiento2.PNG)
    - Capacidad de ser administrado
        1. Definición
        la capacidad de ser modificado sin introducir errores
        2. Características
        ![MapaEmp](/assets/images/CaracteristicasA.PNG)
            1. Escenarios de Calidad 1
            ![esc](/assets/images/Cadmin1.PNG)
            2. Escenarios de Calidad 2
            ![esc](/assets/images/Cadmin2.PNG)
            3. Escenarios de Calidad 3
            ![esc](/assets/images/Cadmin3.PNG)
            4. Escenarios de Calidad 4
            ![esc](/assets/images/Cadmin4.PNG)
            5. Escenarios de Calidad 5
            ![esc](/assets/images/Cadmin5.PNG)
- **Funcionalidades criticas**
  - son aquellas imprescindibles para el proyecto, que tienen un reto de diseño o desconocemos técnicamente como llevarlas a cabo
    - REGISTRAR UN USUARIO: si bien no presenta un reto técnico es fundamental para hacer la reserva

            Esta funcionalidad es la encargada de registrar al usuario en la plataforma 

        ![FunCrit](/assets/images/RegistrarUsuario.png)

    - REGISTRAR UN VEHICULO: al igual que el registro de usuario este no presenta un reto técnico pero es imprescindible para la reserva del parqueadero el cual es una funcionalidad principal

            esta funcionalidad es la encargada de registrar un vehículo a nombre de un usuario anteriormente registrado y logueado

        ![FunCrit](/assets/images/RegistrarVehiculo.png)

    - REALIZAR UNA RESERVA: esta es una de las funcionalidades principales y presenta un reto de diseño

            esta funcionalidad es la encargada de hacer una reserva efectiva

        ![FunCrit](/assets/images/RealizarReserva.png)

    - INICIO Y FINALIZADO DE SESION: si bien el reto de diseño no es tan complicado el reto técnico lo es un poco mas ya que conlleva arraigado el cambio y recuperación de contraseñas que se realiza a través de  un proveedor de correos electrónicos

            esta funcionalidad es la encargada del inicio y cerrado de sesión así también como la recuperación o cambio de contraseñas

        ![FunCrit](/assets/images/InicioSesion.png)

    - MOSTRAR DISPONIBILIDAD DE CUPOS EN EL PARQUEADERO:

        esta no presenta un reto ni de diseño ni técnico pero es fundamental y en el cual se basan muchas otras funcionalidades

            esta funcionalidad muestra los cupos disponibles en el parqueadero

        ![FunCrit](/assets/images/Cupos.png)

    - DAR ENTRADA Y SALIDA A LOS VEHICULOS:

        este presenta un reto tanto técnico como de diseño y es fundamental para otras funcionalidades

            esta funcionalidad es la encargada de registrar el ingreso y salida de vehículos

        ![FunCrit](/assets/images/IngresoSalida.png)

- **Restricciones Técnicas**
  - Restricción Funcional
    - ciertas funciones solo están disponibles para usuarios registrados y que inicien sesión
    - ciertas funciones solo están disponibles para el administrador back office
  - Restricción Sobre Contenido
    - la pagina tendrá una parte de texto enriquecido donde el administrador podrá modificar el contenido visible
  - ¿Hay algunas tecnologías impuestas o prioritarias: lenguajes, frameworks, CMS…?
    - no existen normas que nos impongan usar alguna tecnología en especifico pero ya están definidos los drivers arquitectónicos según lo mas factible para la arquitectura que estamos manejando
  - ¿Con qué navegadores debe ser compatible tu sitio?
    - cualquier navegador capaz de usar el protocolo https
  - ¿Qué sistemas externos tienes pensado integrar: redes sociales, contabilidad, facturación, emailing, marketing automation, CRM, analítica web…?
    - email ya que se usa para la recuperación de contraseña
- **Restricciones de negocio**
  - Tiempo
    - se requiere entregar una de las funcionalidades principales al finalizar el semestre
  - Alcance
    - se necesita tener claro que es lo que vamos a entregar en el tiempo propuesto ya que si se aumenta el alcance necesita aumentar o bien el costo o el tiempo para mantener el equilibrio

        ![ResNeg](/assets/images/alcance.png)

  - ...
