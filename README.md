![thumbnail-Formação Java](https://github.com/jacqueline-oliveira/3356-java-screenmatch-web/assets/66698429/d1e7755b-0a61-411f-bb99-9fcfda44f00c)

# Java: criando sua primeira API e conectando ao front

Projeto desenvolvido no terceiro curso da formação Avançando com Java da Alura


## 🔨 Objetivos do projeto

- Atualizar o projeto ScreenMatch, criado inicialmente com linha de comando, para se transformar em uma API REST;
- Entender a estrutura MVC no desenvolvimento de aplicações Web;
- Criar e mapear rotas utilizando as anotações do Spring;
- Utilizar boas práticas e entender o conceito de DTO (Data Transfer Object); 
- Conectar dados disponibilizados pelo back-end à uma aplicação front-end, disponibilizada nesse [link](https://github.com/jacqueline-oliveira/3356-java-web-front) 
- Tratar erros de CORS na disponibilização de dados;
- Fornecer uma experiência fullstack, demonstrando o fluxo ponta a ponta da aplicação.

## Aprendizados

### Aula 01

- Conectar o back-end ao front-end. Vimos que o front-end esperava buscar dados de uma url específica, que era localhost:8080, que é onde subimos nosso servidor.

- Configurar uma aplicação web com o Spring Boot. Conhecemos a dependência starter-web do Spring, que baixa várias outras dependências e configura automaticamente um servidor na porta localhost:8080, ou em alguma outra que configuremos na nossa aplicação.

- Organizar um projeto MVC. Aprendemos como estruturar o projeto em várias camadas e como conectá-las.

- Retornar uma informação no navegador. Criamos nosso primeiro controller e nossa primeira rota da API, utilizando anotações como `@RestController` e `@GetMapping`.
- 