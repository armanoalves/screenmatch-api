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

- Retornar uma informação no navegador. Criação do primeiro controller e a primeira rota da API, utilizando anotações como `@RestController` e `@GetMapping`.

### Aula 02

- Devolver os dados do nosso banco para o navegador. Trabalhamos devolvendo os dados do nosso banco no Controller, devidamente serializados.

- Tratar serialização circular. Vimos os problemas que ocorrem ao tentar serializar entidades mapeadas de forma bidirecional e como resolvê-los.

- Utilizar o padrão DTO. Para evitar a serialização circular e principalmente para seguir boas práticas, criação dos DTOs. Assim, nossos dados ficaram mais seguros e foram devolvidos de forma personalizada.

- Lidar com o erro de CORS. Conhecemos o erro entre a comunicação entre rotas de origens diferentes e pudemos tratá-lo, criando a classe `CorsConfiguration`.

- Configurar o Live Reload. Para que a aplicação não precise ser parada e reinicializada sempre que houver mudanças, usamos o Devtools e mudamos as configurações necessárias no Intellij.

### Aula 03

- Deixar o código mais limpo e organizado. Vimos que a única responsabilidade de um controlador é tratar da comunicação e das rotas da API. Assim, ele não deve conter regras de negócio. E para fazer essa divisão, criamos uma classe de serviços, a SerieService. 

- Utilizar boas práticas de extração de métodos Aplicamos princípios da orientação a objetos, extraindo métodos que eram comuns no código, facilitando a manutenção.

- Criar uma url fixa para o Controller. Usamos o `@RequestMapping` para que todas as urls mapeadas pelo controlador de séries tenham como prefixo o “/series”.

- Retornar os dados de uma única série. Para buscar uma série, precisamos que o seu id seja passado como parâmetro. Conhecemos o `@PathVariable`, que nos auxilia nesse objetivo.

### Aula 04 

- Trabalhar de forma colaborativa. Vimos que é importante sempre testar exaustivamente o código, principalmente com registros diferentes. Somente assim temos a confirmação de que nossas buscas estão corretas.

- Passar parâmetros na url. Usamos novamente a anotação @PathVariable e vimos que ela pode ser utilizada tanto com números quanto com strings. Para que ela funcione, basta que passemos o nome do parâmetro entre chaves na url do @GetMapping, exatamente como ele está declarado na função.

- Comparar streams e buscas no banco de dados. Aprendemos que podemos utilizar tanto streams quanto consultas do banco de dados, não precisamos nos restringir ao uso exclusivo de um deles. Basta que analisemos a complexidade das buscas, filtros e operações que faremos.

- Desenvolver uma aplicação de forma incremental. Ao trabalhar na integração do front com o back-end, identificamos, ao longo do tempo, os requisitos necessários para tudo funcionar em conjunto. O trabalho incremental é muito comum no ambiente de desenvolvimento.
