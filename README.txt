Вытащи все файлы из рарника куда-нибудь, главное чтобы start.bat и board.jar лежали в одной папке

Запуск сервера:
Дважды кликаешь start.bat и наблюдаешь загрузку аля

C:\Users\Иван\Desktop>java -jar board.jar

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::                (v3.1.4)

2023-10-01T18:13:42.909+03:00  INFO 52184 --- [           main] c.a.fordarina.ForDarinaApplication       : Starting ForDarinaApplication v0.0.1-SNAPSHOT using Java 18.0.2 with PID 52184 (C:\Users\╨Ш╨▓╨░╨╜\Desktop\board.jar started by ╨Ш╨▓╨░╨╜ in C:\Users\╨Ш╨▓╨░╨╜\Desktop)
2023-10-01T18:13:42.911+03:00  INFO 52184 --- [           main] c.a.fordarina.ForDarinaApplication       : No active profile set, falling back to 1 default profile: "default"
2023-10-01T18:13:43.588+03:00  INFO 52184 --- [           main] .s.d.r.c.RepositoryConfigurationDelegate : Bootstrapping Spring Data JPA repositories in DEFAULT mode.
2023-10-01T18:13:43.668+03:00  INFO 52184 --- [           main] .s.d.r.c.RepositoryConfigurationDelegate : Finished Spring Data repository scanning in 65 ms. Found 4 JPA repository interfaces.
2023-10-01T18:13:44.309+03:00  INFO 52184 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
2023-10-01T18:13:44.317+03:00  INFO 52184 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
2023-10-01T18:13:44.317+03:00  INFO 52184 --- [           main] o.apache.catalina.core.StandardEngine    : Starting Servlet engine: [Apache Tomcat/10.1.13]
2023-10-01T18:13:44.388+03:00  INFO 52184 --- [           main] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2023-10-01T18:13:44.389+03:00  INFO 52184 --- [           main] w.s.c.ServletWebServerApplicationContext : Root WebApplicationContext: initialization completed in 1424 ms
2023-10-01T18:13:44.555+03:00  INFO 52184 --- [           main] o.hibernate.jpa.internal.util.LogHelper  : HHH000204: Processing PersistenceUnitInfo [name: default]
2023-10-01T18:13:44.611+03:00  INFO 52184 --- [           main] org.hibernate.Version                    : HHH000412: Hibernate ORM core version 6.2.9.Final
2023-10-01T18:13:44.613+03:00  INFO 52184 --- [           main] org.hibernate.cfg.Environment            : HHH000406: Using bytecode reflection optimizer
2023-10-01T18:13:44.758+03:00  INFO 52184 --- [           main] o.h.b.i.BytecodeProviderInitiator        : HHH000021: Bytecode provider name : bytebuddy
2023-10-01T18:13:44.912+03:00  INFO 52184 --- [           main] o.s.o.j.p.SpringPersistenceUnitInfo      : No LoadTimeWeaver setup: ignoring JPA class transformer
2023-10-01T18:13:44.930+03:00  INFO 52184 --- [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Starting...
2023-10-01T18:13:45.318+03:00  INFO 52184 --- [           main] com.zaxxer.hikari.pool.HikariPool        : HikariPool-1 - Added connection org.postgresql.jdbc.PgConnection@a7f0ab6
2023-10-01T18:13:45.320+03:00  INFO 52184 --- [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Start completed.
2023-10-01T18:13:45.688+03:00  INFO 52184 --- [           main] o.h.b.i.BytecodeProviderInitiator        : HHH000021: Bytecode provider name : bytebuddy
2023-10-01T18:13:46.444+03:00  INFO 52184 --- [           main] o.h.e.t.j.p.i.JtaPlatformInitiator       : HHH000490: Using JtaPlatform implementation: [org.hibernate.engine.transaction.jta.platform.internal.NoJtaPlatform]
2023-10-01T18:13:46.745+03:00  INFO 52184 --- [           main] j.LocalContainerEntityManagerFactoryBean : Initialized JPA EntityManagerFactory for persistence unit 'default'
2023-10-01T18:13:47.167+03:00  INFO 52184 --- [           main] c.a.fordarina.services.ImageService      : Image directory set to C:\images
2023-10-01T18:13:47.203+03:00  WARN 52184 --- [           main] JpaBaseConfiguration$JpaWebConfiguration : spring.jpa.open-in-view is enabled by default. Therefore, database queries may be performed during view rendering. Explicitly configure spring.jpa.open-in-view to disable this warning
2023-10-01T18:13:47.543+03:00  INFO 52184 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat started on port(s): 8080 (http) with context path ''
2023-10-01T18:13:47.552+03:00  INFO 52184 --- [           main] c.a.fordarina.ForDarinaApplication       : Started ForDarinaApplication in 5.106 seconds (process running for 5.597)  

Последняя строчка означает что все запустилось. Если вывод сильно отличается, значит что-то не так.

Сервер стартует на порту 8080,
остальное читай в openApi - вот сюда https://editor.swagger.io/ копируешь и вставляешь все что ниже, после чего разбираешься.
Чтобы остановить сервер в открывшейся консоли зажимаешь сочетание клавиш ctrl + c. Должно написать 

^CЗавершить выполнение пакетного файла [Y(да)/N(нет)]? 2023-10-01T18:13:49.025+03:00  INFO 52184 --- [ionShutdownHook] j.LocalContainerEntityManagerFactoryBean : Closing JPA EntityManagerFactory for persistence unit 'default'
2023-10-01T18:13:49.027+03:00  INFO 52184 --- [ionShutdownHook] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Shutdown initiated...
2023-10-01T18:13:49.084+03:00  INFO 52184 --- [ionShutdownHook] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Shutdown completed.




Open api которое надо скопировать:



openapi: "3.0.3"
info:
  title: "Board API"
  description: "Тут все шо нада"
  version: "1.0.0"
servers:
  - url: "http://localhost:8080"
paths:
  /themes:
    post:
      tags:
        - Themes
      summary: "Создать новую тему"
      operationId: "createTheme"
      requestBody:
        content:
          application/json:
            schema:
              $ref: "#/components/schemas/CreateThemeRequest"
        required: true
      responses:
        "201":
          description: "CREATED"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/ThemeResponseEntity"
    get:
      tags:
        - Themes
      summary: "Получить все темы"
      operationId: "getAllThemes"
      responses:
        "200":
          description: "OK"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/ThemeResponseArray"
  /themes/{id}:
    get:
      tags:
        - Themes
      summary: "Получить одну тему по id"
      operationId: "getThemeById"
      parameters:
        - name: id
          in: path
          required: true
          schema:
            type: integer
          description: "ID темы, информацию о которой хотим получить"
      responses:
        '200':
          description: "OK"
          content:
            application/json:
              schema:
                $ref: "#/components/schemas/ThemeResponseEntity"

  /threads:
    post:
      tags:
        - Threads
      summary: "Создать новый тред в теме"
      operationId: "createThread"
      requestBody:
        content:
          application/json:
            schema:
              $ref: "#/components/schemas/CreateThreadRequest"
        required: true
      responses:
        "201":
          description: "CREATED"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/ThreadResponseEntity"
    get:
      tags:
        - Threads
      summary: "Получить все треды по теме"
      operationId: "getAllThreadsByTheme"
      parameters:
        - name: themeId
          in: query
          required: true
          schema:
            type: integer
          description: "ID темы, все треды которой хотим получить"
      responses:
        "200":
          description: "OK"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/ThreadResponseArray"
  /threads/{id}:
    get:
      tags:
        - Threads
      summary: "Получить одну тему по id"
      operationId: "getThreadById"
      parameters:
        - name: id
          in: path
          required: true
          schema:
            type: integer
          description: "ID треда, информацию о котором хотим получить"
      responses:
        '200':
          description: "OK"
          content:
            application/json:
              schema:
                $ref: "#/components/schemas/ThreadResponseEntity"


  /messages:
    post:
      tags:
        - Messages
      summary: "Создать новое сообщение в треде"
      operationId: "createMessage"
      requestBody:
        content:
          application/json:
            schema:
              $ref: "#/components/schemas/CreateMessageRequest"
        required: true
      responses:
        "201":
          description: "CREATED"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/MessageResponseEntity"
    get:
      tags:
        - Messages
      summary: "Получить все треды по теме"
      operationId: "getAllMessagesByThread"
      parameters:
        - name: threadId
          in: query
          required: true
          schema:
            type: integer
          description: "ID треда, все сообщения которого хотим получить"
      responses:
        "200":
          description: "OK"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/MessageResponseArray"
  /messages/{id}:
    get:
      tags:
        - Messages
      summary: "Получить одно сообщение по ID"
      operationId: "getMessageById"
      parameters:
        - name: id
          in: path
          required: true
          schema:
            type: integer
          description: "ID сообщения, информацию о котором хотим получить"
      responses:
        '200':
          description: "OK"
          content:
            application/json:
              schema:
                $ref: "#/components/schemas/MessageResponseEntity"

  /images:
    post:
      tags:
        - Images
      summary: "Загрузить пикчу"
      operationId: "uploadImage"
      parameters:
        - name: "file"
          in: query
          required: true
          schema:
            type: "string"
            format: "binary"
        - name: "messageId"
          in: "query"
          required: true
          schema:
            type: "integer"
            format: "int64"
      responses:
        "201":
          description: "OK"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/ImageResponseEntity"

    get:
      tags:
        - Images
      summary: "Получить пикчи по messageId"
      operationId: "getImagesByMessageId"
      parameters:
        - name: "messageId"
          in: "query"
          required: true
          schema:
            type: "integer"
            format: "int64"
      responses:
        "200":
          description: "OK"
          content:
            'application/json':
              schema:
                $ref: "#/components/schemas/ImageResponseArray"
  /images/{id}:
    get:
      tags:
        - Images
      summary: "Получить ресурс на одну пикчу по ID"
      operationId: "getImageById"
      parameters:
        - name: id
          in: path
          required: true
          schema:
            type: integer
          description: "ID пикчи, информацию о котором хотим получить"
      responses:
        '200':
          description: OK
          content:
              application/png:
                schema: 
                  type: string
                  format: binary
  /clear:
    post:
      tags:
        - CLEAR DATABASE
      summary: "Полностью очищает всю базу данных. Достаточно 1 раз послать сюда POST"
      operationId: "clearAll"
      responses:
        '200':
          description: "OK"
          content:
            "*/*":
              schema:
                type: string





components:
  schemas:
    CreateThemeRequest:
      type: "object"
      properties:
        name:
          type: "string"
        prefix:
          type: "string"
    ThemeResponseEntity:
      description: "Вот такой вот ответ"
      type: "object"
      properties:
        id:
          type: "integer"
        name:
          type: "string"
        prefix:
          type: "string"
    ThemeResponseArray:
      description: "Вот такой вот массив ответов"
      type: "array"
      items:
        type: "object"
        properties:
          id:
            type: "number"
          name:
            type: "string"
          prefix:
            type: "string"
      minItems: 3


    CreateThreadRequest:
      type: "object"
      properties:
        name:
          type: "string"
        themeId:
          type: number
    ThreadResponseEntity:
      description: "Информация об одном треде"
      type: "object"
      properties:
        id:
          type: "integer"
        name:
          type: "string"
        themeId:
          type: number
    ThreadResponseArray:
      description: "Информация о нескольких тредах"
      type: "array"
      items:
        type: "object"
        properties:
          id:
            type: "number"
          name:
            type: "string"
          themeId:
            type: number
      minItems: 3

    CreateMessageRequest:
      type: "object"
      properties:
        text:
          type: "string"
        threadId:
          type: number
    MessageResponseEntity:
      description: "Информация об одном сообщении"
      type: "object"
      properties:
        id:
          type: "integer"
        text:
          type: "string"
        threadId:
          type: number
    MessageResponseArray:
      description: "Информация о нескольких сообщениях"
      type: "array"
      items:
        type: "object"
        properties:
          id:
            type: "number"
          text:
            type: "string"
          threadId:
            type: number
      minItems: 3

    ImageResponseEntity:
      type: "object"
      properties:
        id:
          type: "integer"
        messageId:
          type: "integer"
        fileName:
          type: "string"
    ImageResponseArray:
      description: "Информация о нескольких пикчах"
      type: "array"
      items:
        type: "object"
        properties:
          id:
            type: "integer"
          messageId:
            type: "integer"
          fileName:
            type: "string"
      minItems: 3
