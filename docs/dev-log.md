# Bitácora de Desarrollo (`dev-log.md`)

Este documento describe paso a paso el proceso de construcción del proyecto de arquitectura basada en API Gateway. La implementación se realizó con Node.js y busca ejemplificar el funcionamiento básico de este patrón arquitectónico en la nube.

---

### Creación de microservicios

Para poder usar un API Gateway y ejemplificarlo correctamente, es necesario definir microservicios para que el Gateway pueda hacer la redirección.

Para desarrollar este punto, decidimos generar el código de los microservicios con una inteligencia artificial. Puesto que, solo servirán de ejemplo y lo importante es el Gateway.

Hemos decidido generar microservicios de productos, órdenes y usuarios. Para cada uno dentro de su respectivo directorio corrimos los comandos:

```bash
npm init -y
npm install express
```

Y para correr cada microservicio

```bash
npm start
```

Todos los servicios corren en puertos diferentes (3001, 3002, 3003).

![](./images/orderService.png)

![](./images/productService.png)

![](./images/userService.png)
