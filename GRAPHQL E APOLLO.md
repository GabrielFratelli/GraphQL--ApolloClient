# GraphQL Apollo

GRAPHQL E APOLLO

Problemas que o GraphQL resolve:

 

Overfetching = buscar informações demais. 

Exemplo: se quiser pegar um energético o REST teria retornado uma geladeira com energético, já o GRAPHQL faz a busca expecífica do item em si.

Underfetching === buscar dados de menos. 

Exemplo: uma rota de usuarios só retorna usuários, mas é necessário te retornar usuários e endereço, então teria q ser feita uma nova rota que iria retornar apensas os endereço.

Dificuldades do GraphQL: 

- Cache: (Lidar com o cache de requisições) 

GraphQL É uma ferramenta criada pelo time do facebook, é uma query language ou seja é uma forma de eu escrever operações de escrita e leitura.

Para que serve o GraphQL? 

Ele serve para realizar operações de escrita e leitura, através da comunicação de front com back.

O Backend vai ter um endereço por exemplo , sempre essa rota: [http://localhost:3000/graphql](http://localhost:3000/graphql), e nele vai ter todos os dados disponível da API, somente pro Frotend trabalhando com graphql escolhe oque ele vai utilizar, qual dado ele vai querer!

Dificuldades:

Cache: por exemplo o browser já faz automaticamente o cache da tela, se fosse pra fazer isso com GraphQL seria mais difcil.

No GraphQL os códigos de erros são 200, é o codigo de sucesso para o browser.

`query {
  users {
    id
    name
    github

    addresses {
      city
      state
      country
    }
  }
}`

Ele traz mais complexidade, ou seja, o GraphQL ele especifica quais dados ele quer, ao enves de deixar explicito na mão como era antes, ele especifica no código pedindo qual dado ele quer, para não ter um monte sem ser utilizado.

Apollo é onde funciona a API do backend na qual o front pode puxar, ele e altamente typado ou seja, vai corrigir e mostrar oque está disponivel.

Schema-first: Escrevemos o schema e depois escrevemos o código.

Code-first: Escrevemos o código e ele sozinho cria o schema pra gente.

Na hora de trabalhar com GRAPHQL, importar ele como gql e criar uma variavel GET_USER, e cria a query com os dados necessitários como por exemplo:

`Query {
  users {
  id
  name
  }
}`
