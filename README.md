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

Este proyecto cuenta con tres microservicios que teóricamente comparten una lógica de negocio porque para un e-commerce sería el modelo `cliente`, `producto`, `orden`. Pero, como están implementados únicamente con fines de demostración del Gateway, son completamente independientes entre sí. Adjunto los repositorios de cada microservicio. También se encuentran en la estructura de este repositorio.

[Microservicio de clientes](https://github.com/AlejandroTorres05/users-service-repo)

[Microservicio de productos](https://github.com/AlejandroTorres05/product-service-repo)

[Microservicio de órdenes](https://github.com/AlejandroTorres05/orders-service-repo)

La arquitectura se completa con el Gateway completamente desplegado y montado en AZURE, no necesita código en este repositorio para poder cumplir su función de redireccionamiento.

## Endpoints disponibles

Los micro servicios de manera individual, pueden ser accedidos en la nube a través de estos enlaces:

[Microservicio de clientes](https://users-service-ct-h4e0gabdc6ede8fu.eastus2-01.azurewebsites.net)

[Microservicio de productos](https://products-service-ct-fghrecgkesdmddeb.eastus2-01.azurewebsites.net)

[Microservicio de órdenes](https://orders-service-ct-a7fadza8aqasb2fb.eastus2-01.azurewebsites.net)

A través del API Gateway, mediante estos enlaces:

[Microservicio de clientes](https://api-gateway-demo-ct.azure-api.net/user)

[Microservicio de productos](https://api-gateway-demo-ct.azure-api.net/product/products)

[Microservicio de órdenes](https://api-gateway-demo-ct.azure-api.net/srvc/orders)

## Demostración y proceso de desarrollo

Todo el proceso de desarrollo y las respectivas evidencias de trabajo, están disponibles en en la bitácora del proyecto que se encuentra dentro de la carpeta docs como [dev-log.md](./docs/dev-log.md).

## Recursos adicionales

Para ver la documentación de AZURE, más detallada sobre API Gateway y su descomposición en patrones más específicos visitar:

- [Gateway Routing pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/gateway-routing)
- [Gateway Offloading pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/gateway-offloading)
- [Gateway Aggregation pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/gateway-aggregation)

## Autores

[Juan David Calderon Salamanca](https://github.com/juanC773) y [Alejandro Torres Soto](https://github.com/AlejandroTorres05)
