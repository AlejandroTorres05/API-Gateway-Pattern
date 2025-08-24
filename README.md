# API Gateway Pattern - Implementación en la Nube

## ¿Qué es el patrón API Gateway?

Un API Gateway actúa como un único punto de entrada para múltiples servicios, manejando routing, autenticación, rate limiting, entre otros.

**Es útil cuando:**

- Se requiere exponer múltiples servicios en un solo endpoint y enrutar hacia el servicio apropiado a partir de la solicitud.

![](/images/multile-disparate-service.png)

- Se requiere exponer múltiples instancias del mismo servicio en un solo endpoint para balanceo de carga y/o disponibilidad.

![](/images/multiple-instance-service.png)

- Para exponer diferentes versiones del mismo servicio en un solo endpoint y enrutar el tráfico entre dichas versiones.

![](/images/multiple-versions.png)

## Arquitectura del proyecto

## Cómo ejecutar el proyecto

## Endpoints disponibles

## Capturas o Demostración

## Recursos adicionales

Para ver la documentación de AZURE, más detallada sobre API Gateway y su descomposición en patrones más específicos visitar:

- [Gateway Routing pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/gateway-routing)
- [Gateway Offloading pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/gateway-offloading)
- [Gateway Aggregation pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/gateway-aggregation)

## Autores

[Juan David Calderon Salamanca](https://github.com/juanC773) y [Alejandro Torres Soto](https://github.com/AlejandroTorres05)
