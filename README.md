# config-data

Repositorio con la configuración externa (Spring Cloud Config) de todos los microservicios del sistema Syrion.

## Contiene
- `product.properties`, `cart.properties`, `invoice.properties`
- `gateway.yaml`, `registry.yaml`, `admin.yaml`
- `servicio_autenticacion.yml`

## Uso rápido
- El **config-server** apunta a este repo.
- Cada API usa: `spring.config.import=optional:configserver:` y `spring.cloud.config.uri=http://localhost:8888`.

Aquí se definen puertos, BD, JPA/Hibernate, Eureka, Swagger, etc.  
Lo consume `config-server` mediante `spring.cloud.config.server.git.uri`.
