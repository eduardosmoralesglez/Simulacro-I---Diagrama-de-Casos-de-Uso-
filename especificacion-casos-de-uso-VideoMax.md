
# Especificación de los casos de uso de VideoMax

## Especificación de Actores

### Actor: Cliente
| Actor | Cliente |
|---|---|
| **Descripción** | Usuario que alquila y reserva películas a través de la plataforma. |
| **Características** | Capacidad de proporcionar datos personales y tiene interés en el entretenimiento y películas. |
| **Relaciones** |  |
| **Referencias** | Proporcionar datos personales, Alquilar película, Reservar película. |
| **Notas** | Este actor puede tener preferencias tipos de películas que deben considerarse para maximizar las ganancias. |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

### Actor: Administrador
| Actor | Administrador |
|---|---|
| **Descripción** | Persona encargada de gestionar la plataforma y su contenido. |
| **Características** | Habilidad para interactuar con clientes y proveedores. |
| **Relaciones** |  |
| **Referencias** | Registrar a los clientes, Registrar alquiler, Registrar reserva, Registrar película, Actualizar proveedor. |
| **Notas** | Debe tener acceso a información confidencial de los clientes y potestad para cambiar de proveedor. |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

### Actor: Proveedor
| Actor | Proveedor |
|---|---|
| **Descripción** | Entidad encargada de abastecer las películas en la plataforma. |
| **Características** | Debe tener información sobre la disponibilidad de películas. |
| **Relaciones** | |
| **Referencias** | Abastecer películas según existencia. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

---

## Especificación de Casos de Uso

| Caso de Uso CU | Proporcionar datos personales |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Cliente |
| **Descripción** | El Cliente proporciona su información personal para el registro en la plataforma. |
| **Flujo básico** | 1. Cliente ingresa sus datos personales. ---> 2. Cliente envía la información. ---> 3. Administrador almacena la información. |
| **Pre-condiciones** | El Cliente debe tener acceso a la plataforma. |
| **Post-condiciones** | Los datos personales del Cliente se registran en el sistema. |
| **Requerimientos** | Dispositivo con acceso a Internet. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

| Caso de Uso CU | Alquilar película |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Cliente |
| **Descripción** | El Cliente alquila una película de la plataforma. |
| **Flujo básico** | 1. Cliente selecciona una película. ---> 2. Cliente confirma el alquiler. ---> 3. Administrador registra el alquiler. |
| **Pre-condiciones** | El Cliente debe estar registrado y tener datos personales válidos. |
| **Post-condiciones** | La película se marca como alquilada en el sistema. |
| **Requerimientos** | Método de pago válido. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

| Caso de Uso CU | Reservar película |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Cliente |
| **Descripción** | El Cliente reserva una película para un alquiler futuro. |
| **Flujo básico** | 1. Cliente selecciona una película. ---> 2. Cliente confirma la reserva. ---> 3. Administrador registra la reserva. |
| **Pre-condiciones** | El Cliente debe estar registrado. |
| **Post-condiciones** | La película se reserva y está marcada en el sistema. |
| **Requerimientos** | Validación de disponibilidad. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

| Caso de Uso CU | Registrar a los clientes |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Administrador |
| **Descripción** | El Administrador registra a nuevos Clientes en el sistema. |
| **Flujo básico** | 1. Administrador ingresa datos del Cliente. ---> 2. Administrador confirma registro. ---> 3. Sistema almacena los datos. |
| **Pre-condiciones** | El Administrador debe estar autenticado en el sistema. |
| **Post-condiciones** | Los datos del nuevo Cliente se registran en el sistema. |
| **Requerimientos** | Acceso administrativo a la plataforma. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

| Caso de Uso CU | Registrar Alquiler |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Administrador |
| **Descripción** | El Administrador registra a un Alquiler de pelicula en el sistema. |
| **Flujo básico** | 1. Cliente confirma el alquiler. ---> 2. Administrador registra el alquiler. ---> 3. Sistema almacena los datos.|
| **Pre-condiciones** | El Administrador debe estar autenticado en el sistema. |
| **Post-condiciones** | Los datos del nuevo Alquiler se registran en el sistema. |
| **Requerimientos** | Cliente solicita nuevo Alquiler. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

| Caso de Uso CU | Registrar Reserva |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Administrador |
| **Descripción** | El Administrador registra a una reserva de pelicula en el sistema. |
| **Flujo básico** | 1. Cliente confirma el reserva. ---> 2. Administrador registra la reserva. ---> 3. Sistema almacena los datos.|
| **Pre-condiciones** | El Administrador debe estar autenticado en el sistema. |
| **Post-condiciones** | Los datos de la nueva reserva se registran en el sistema. |
| **Requerimientos** | Cliente solicita nuevo reserva. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

| Caso de Uso CU | Registrar Pelicula |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Administrador |
| **Descripción** | El Administrador registra a una pelicula en el sistema. |
| **Flujo básico** | 1. Proveedor abastece la pelicula ---> 2. Administrador registra la pelicula. ---> 3. Sistema almacena los datos.|
| **Pre-condiciones** | El Administrador debe estar autenticado en el sistema. |
| **Post-condiciones** | Los datos de la nueva pelicula se registran en el sistema. |
| **Requerimientos** | Proveedor abastece la pelicula. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

| Caso de Uso CU | Abastecer películas según existencia |
|---|---|
| **Fuentes** | Documento de requisitos de sistema |
| **Actor** | Proveedor |
| **Descripción** | El Proveedor abastece las películas en función de la disponibilidad. |
| **Flujo básico** | 1. Proveedor revisa el inventario. ---> 2. Proveedor añade películas que faltan. ---> 3. Sistema actualiza el inventario. |
| **Pre-condiciones** | El Proveedor debe estar autenticado en el sistema. |
| **Post-condiciones** | El inventario de películas se actualiza. |
| **Requerimientos** | Acceso administrativo a las existencias de la plataforma. |
| **Notas** |  |
| **Autor** | Eduardo Serafín Morales González |
| **Fecha** | 20/11/2024 |

