#Web-based-Online-Food-Ordering-and-Delivery-Management-Software
## Giải thích chi tiết các thư mục và file quan trọng

### 1. **Thư mục java/com/fooddelivery/**

#### **FoodDeliveryApplication.java**
- File chính để chạy ứng dụng Spring Boot
- Chứa annotation `@SpringBootApplication`

#### **config/**
- **SecurityConfig.java**: Cấu hình Spring Security, JWT, phân quyền
- **WebMvcConfig.java**: Cấu hình MVC, CORS, interceptor
- **DatabaseConfig.java**: Cấu hình kết nối database
- **JpaConfig.java**: Cấu hình JPA, Hibernate
- **SwaggerConfig.java**: Cấu hình API documentation
- **AsyncConfig.java**: Cấu hình xử lý bất đồng bộ

#### **controller/web/**
- Controllers cho giao diện web (Thymeleaf)
- Trả về view name (HTML templates)
- Xử lý form submission, hiển thị trang

#### **controller/api/v1/**
- REST API controllers
- Trả về JSON response
- Xử lý các API endpoint cho mobile/frontend

#### **service/ và service/impl/**
- Interface và implementation của business logic
- Xử lý các quy trình nghiệp vụ phức tạp
- Transaction management

#### **repository/**
- JPA repositories
- Thao tác với database
- Custom queries với JPQL/Native SQL

#### **entity/**
- JPA entities
- Ánh xạ với bảng database
- Định nghĩa relationships

#### **dto/**
- **request/**: DTO cho dữ liệu gửi lên server
- **response/**: DTO cho dữ liệu trả về client
- **common/**: DTO dùng chung

#### **security/**
- JWT token generation và validation
- Custom user details service
- Authentication filters

#### **exception/**
- Custom exceptions
- Global exception handler
- Error response formatting

#### **util/**
- Các utility classes
- Helper methods
- Common functions

#### **mapper/**
- Convert Entity ↔ DTO
- Object mapping logic

#### **validator/**
- Custom validators
- Validation annotations
- Business rule validations

#### **constant/**
- Enums
- Constants
- Status codes

#### **event/ và event/listener/**
- Event-driven architecture
- Async event handling
- Notification triggers

#### **payment/**
- Payment gateway integrations
- VNPay, MoMo, COD implementations

### 2. **Thư mục resources/**

#### **application.properties**
- Cấu hình chính của ứng dụng
- Database connection
- Server port, context path

#### **application-{profile}.properties**
- Cấu hình theo môi trường (dev, prod, test)

#### **db/migration/**
- Flyway/Liquibase migration scripts
- Versioned database changes
- Schema evolution

#### **static/**
- **css/**: Stylesheets
- **js/**: JavaScript files
- **images/**: Static images, icons
- **fonts/**: Custom fonts

#### **templates/**
- Thymeleaf HTML templates
- Organized by role (admin, restaurant, shipper, customer)
- Reusable fragments

#### **messages/**
- Internationalization (i18n)
- Error messages
- Validation messages

#### **email-templates/**
- HTML templates cho email
- Transactional emails

#### **certificates/**
- SSL certificates
- Aiven CA certificate

### 3. **Thư mục test/**

- **controller/**: Controller unit tests
- **service/**: Service layer tests
- **repository/**: Repository tests
- **integration/**: Integration tests
- Test data và utilities

### 4. **Thư mục docs/**

- **api/**: API documentation, Postman collections
- **database/**: Database design documents, diagrams
- **deployment/**: Deployment guides
- **user-guide/**: User manuals cho từng role
- **technical/**: Technical specifications

### 5. **Thư mục scripts/**

- **setup/**: Initialization scripts
- **build/**: Build và deployment scripts
- **maintenance/**: Database backup, logs cleanup

### 6. **Thư mục docker/**

- **Dockerfile**: Docker image definition
- **docker-compose.yml**: Multi-container setup
- Development và production configs

### 7. **Root level files**

- **pom.xml**: Maven dependencies và plugins
- **.gitignore**: Git ignore rules
- **.env.example**: Environment variables template
- **README.md**: Project documentation
- **LICENSE**: License information
- **CHANGELOG.md**: Version history
- **TODO.md**: Task tracking

---