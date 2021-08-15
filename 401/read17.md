# Spring Boot and OAuth2
##  create a minimal application that uses GitHub for authentication steps.

1. Creating a New Project:

```
$ mkdir ui && cd ui
$ curl https://start.spring.io/starter.tgz -d style=web -d name=simple | tar -xzvf -
```

2. Add a Home Page : create index.html in the src/main/resources/static folder.
3. Securing the Application with GitHub and Spring Security by adding this dependencies:

```
<dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-oauth2-client</artifactId>
</dependency>
```

4. Add a New GitHub App: Select "New OAuth App" and then the "Register a new OAuth application" page is presented. Enter an app name and description. Then, enter your app’s home page, which should be http://localhost:8080, Finally, indicate the Authorization callback URL as http://localhost:8080/login/oauth2/code/github and click Register Application.

5. Configure application.yml : to make the link to GitHub, add the following to your application.yml

```
spring:
  security:
    oauth2:
      client:
        registration:
          github:
            clientId: github-client-id
            clientSecret: github-client-secret
```

6. Boot Up the Application : you can run your app again and visit the home page at http://localhost:8080. Now, instead of the home page, you should be redirected to login with GitHub.


![img](https://marco.dev/assets/img/uploads/2017/01/oauth2-1_full.png)

## [BACK](../README.md)