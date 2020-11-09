# Angular 10 + Nodejs JWT Token Based Authentication with MySQL Example

Tutorial Link: [Angular 10 + Nodejs JWT Token Based Authentication with MySQL Example](https://loizenai.com/angular-10-nodejs-jwt-authentication-mysql-examples-tutorials/#sourcecode)

![Angular 10 + Nodejs JWT Token Based Authentication with MySQL Example](https://loizenai.com/wp-content/uploads/2020/06/Angular-10-Nodejs-Security-JWT-Authentication-MySQL-Example.png)

“How to implement Angular 10 + Nodejs JWT Token Based Authentication with MySQL Example?” is always a big common question in development world? So in the tutorial, I guide you very clearly how to build a full stack example to demonstrate an JWT Authentication flow from Angular (signup & signin with by JWT Token) to backend: Nodejs and database MySQL.

## ANGULAR FRONT-END WITH INTERCEPTOR

![ANGULAR FRONT-END WITH INTERCEPTOR](https://loizenai.com/wp-content/uploads/2020/06/Angular-Nodejs-Jwt-Authentication-Architecture-Diagram-Front-End-Client.png)

– app.component is the parent component that contains routerLink and router-outlet for routing. It also has an authority variable as the condition for displaying items on navigation bar.
– user.component, pm.component, admin.component correspond to Angular Components for User Board, PM Board, Admin Board. Each Board uses user.service to access authority data.
– register.component contains User Registration form, submission of the form will call auth.service.
– login.component contains User Login form, submission of the form will call auth.service and token-storage.service.

– user.service gets access to authority data from Server using Angular HttpClient ($http service).
– auth.service handles authentication and signup actions with Server using Angular HttpClient ($http service).
– every HTTP request by $http service will be inspected and transformed before being sent to the Server by auth-interceptor (implements HttpInterceptor).
– auth-interceptor check and get Token from token-storage.service to add the Token to HTTP Request Header.

– token-storage.service manages Token inside Browser’s sessionStorage.

[![Video Guide – Angular 10 + Nodejs JWT Token based Authentication with MySQL Example](https://img.youtube.com/vi/rYmf_MthobU/0.jpg)](https://www.youtube.com/watch?v=rYmf_MthobU)

## JWT Authentication with Nodejs/Express RestAPIs

![JWT Authentication with Nodejs/Express RestAPIs](https://loizenai.com/wp-content/uploads/2020/06/Angular-Nodejs-Jwt-Authentication-Architecture-Diagram-Back-End-Server.png)

## Overview Nodejs server for JWT Authentication

![Overview Nodejs server for JWT Authentication](https://loizenai.com/wp-content/uploads/2020/06/Angular-Nodejs-Security-Jwt-Authentication-Work-Process-Diagram.png)

– SignUp /api/auth/signup:

![Nodejs JWT Authentication SignUp – Jack user with PM role](https://loizenai.com/wp-content/uploads/2020/06/Nodejs-JWT-Authentication-SignUp-Jack-user-with-PM-role.png)

– Sign In /api/auth/signin:

![SignIn Jack User](https://loizenai.com/wp-content/uploads/2020/06/SignIn-Jack-User.png)

– Access User Page /api/test/user:

![Access to protected page](https://loizenai.com/wp-content/uploads/2020/06/Access-to-protected-page.png)

– Access PM Page /api/test/pm:

![Access to PM page](https://loizenai.com/wp-content/uploads/2020/06/Access-to-PM-page.png)

– Access to Admin page /api/test/admin:

![Jack can NOT access Admin Page](https://loizenai.com/wp-content/uploads/2020/06/Jack-can-NOT-access-Admin-Page-1.png)

## Nodejs Project structure:

![Nodejs Project structure](https://loizenai.com/wp-content/uploads/2020/06/Nodejs-JWT-authentication-project-structure.png)

## Angular project structure

![Angular Project Structure](https://loizenai.com/wp-content/uploads/2020/05/Angular-Project-Structure.png)

### Related posts

- [Nodejs Token Based Authentication Example](https://loizenai.com/nodejs-jwt-authentication-example-with-mysql-postgresql-database/)
- [SpringBoot JWT Token Based Authentication Example](https://loizenai.com/spring-boot-security-jwt-authentication-example-mysql-postgresql-spring-jpa-restapis/)
- [Angular 10 SpringBoot Token Based Authentication Example](https://loizenai.com/angular-10-spring-boot-jwt-token-based-authentication-example-spring-security-mysql-database/)
