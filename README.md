# Total Electro - E-commerce Project

## Descripción
Total Electro es una plataforma de comercio electrónico desarrollada como proyecto colaborativo. El sistema permite la gestión de productos, usuarios y transacciones en línea.

## Equipo de Desarrollo
- Ignacio Piñeyro
- Walter Ramos
- Alan Canto
- Ani Celeste
- Ana Julia

## Tecnologías Utilizadas

### Backend
- Java 17
- Spring Boot 3.4.5
- Spring Data JPA
- Hibernate Validator 8.0.0
- Lombok

### Frontend
- Thymeleaf (Motor de plantillas)

### Base de Datos
- H2 Database (Base de datos en memoria para desarrollo)

### Herramientas de Desarrollo
- Maven (Gestión de dependencias)
- Spring Boot DevTools (Herramientas de desarrollo)
- Spring Boot Test (Framework de testing)

## Estructura del Proyecto
```
total-electro/
├── src/
│   ├── main/
│   │   ├── java/        # Código fuente Java
│   │   └── resources/   # Recursos estáticos y configuración
│   └── test/           # Pruebas unitarias
├── .mvn/               # Configuración de Maven
├── target/            # Archivos compilados
└── pom.xml           # Configuración de Maven y dependencias
```

## Requisitos del Sistema
- Java 17 o superior
- Maven 3.6.x o superior

## Configuración del Proyecto

1. Clonar el repositorio
2. Asegurarse de tener Java 17 instalado
3. Ejecutar `mvn clean install` para instalar las dependencias
4. Ejecutar `mvn spring-boot:run` para iniciar la aplicación

## Características Principales
- Gestión de productos
- Sistema de usuarios
- Carrito de compras
- Proceso de checkout
- Panel de administración

## Guía de Contribución
### Flujo de Trabajo
1. Crear una rama para cada nueva característica (`git checkout -b feature/nueva-caracteristica`)
2. Realizar los cambios necesarios
3. Hacer commit de los cambios (`git commit -m 'Agregar nueva característica'`)
4. Subir los cambios a la rama (`git push origin feature/nueva-caracteristica`)
5. Crear un Pull Request

### Convenciones de Código
- Seguir las convenciones de Java
- Documentar todas las clases y métodos públicos
- Escribir pruebas unitarias para nueva funcionalidad
- Mantener el código limpio y legible

## Ambiente de Desarrollo
### Configuración del IDE
- Recomendado: IntelliJ IDEA o Eclipse
- Configurar el JDK 17
- Importar el proyecto como proyecto Maven
- Habilitar el soporte de Lombok

### Variables de Entorno
```properties
# Configuración de la base de datos
spring.datasource.url=jdbc:h2:mem:totalelectro
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=

# Configuración del servidor
server.port=8080
```

## Troubleshooting
### Problemas Comunes
1. **Error de compilación con Lombok**
   - Asegurarse de tener instalado el plugin de Lombok en el IDE
   - Ejecutar `mvn clean install` para regenerar las clases

2. **Problemas con la base de datos H2**
   - Verificar que no haya otra instancia de la aplicación corriendo
   - Limpiar la caché de Maven: `mvn clean`

## Roadmap
- [ ] Implementación de sistema de pagos
- [ ] Integración con pasarelas de pago
- [ ] Sistema de notificaciones por email
- [ ] Panel de análisis y reportes
- [ ] API REST para integración con aplicaciones móviles

## Seguridad
- Implementación de autenticación JWT
- Encriptación de datos sensibles
- Protección contra ataques comunes (XSS, CSRF, SQL Injection)
- Validación de datos en el backend

## Monitoreo y Logging
- Implementación de logs estructurados
- Monitoreo de rendimiento
- Alertas automáticas
- Métricas de negocio

## Licencia
Este proyecto es privado y confidencial.

## Contacto
Para más información sobre el proyecto, contactar a los desarrolladores mencionados en la sección de Equipo de Desarrollo.
