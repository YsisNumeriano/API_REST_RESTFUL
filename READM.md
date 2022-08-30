## API  - Comunicação entre front e backend
Cliente (Client)
Garçom (pedidos, levar seus pedidos para a cozinha) (API)
Cozinha (Server)
API - Conjunto de rotinas e padrôes  que uma aplicação disponibiliza pra gente para que outras aplicações peguem essa informação. 
                        client > api > Server
                        r                                             
> Responsável por estabelecer comunicação entre diferentes serviços.
> Meio de campo entre tecnologias
> Intermediador para troca de informações

## REST - Algumas regras

 > Será feita a transferência de dados de uma maneira simbolica, figurativa, representativa, de maneira didática.
 > A transferência de dados, geralmente, usando o protocolo HTTP.
 > O Rest, delimita algumas obrigações nessas transferências de dados. (Resources)
 > Resources seria entãio, uma entidade, um objeto.
 > 5 necessidades (constraints) para ser RESTful

- Cliente-Server: Separação do cliente e do armazenamento de dados (servidor), dessa forma, poderemos ter uma portabilidade do nosso sistema, usando o React para web e reactnative para o smartphone, por exemplo.
- Stateless: Cada requisição que o cliente faz para o servidor, deverá conter todas as informações necessárias para o servidor entender e responder (RESPONSE) a requisição (RESQUEST). Exemplo: A sessão do usuário deverá ser enviada em todas as requisições, para saber se aquele usuário está autenticado e apto a usar os serviços, e o servidor não pode lembra que o cliente foi autenticado na requisição anterior. tipo Tokens.
- Cavheable: As respostas para uma requisição, deverão ser explicitas ou dizer se aquela requisição, pode ou não ser cacheada pelo cliente.
- Leyered System: O cliente aceesa o endpoint, sem precisar saber da complexibilidade, de quais passos estão sendo necessários para o servidor responder a requisição, ou quais outras camadas o servidor estará lidando, para que a requisiçãom seja respondida.
- Code on demand (optional): Dá a possibilidade da nossa aplicação pegar códigos, como o JS, por exemplo, e executar no cliente.

## BOAS PRÁTICAS

- Utilizar verbos HTTP para requisições
- Utilizar plural ou singular na criação dos endpoints? _NÃO IMPORTA!_ use um padrão!!
- Não deixar barra no final do endpoint
- Nunca deixe o cliente sem respostas!

## Verbos HTTP

- GET: Receber dados de um Resource
- POST: Enviar dados ou informações para serem proessados por um Resource.
- PUT: Atualizar dados de um Resource.
- DELET: Deletar um Resource.

## STATUS DAS RESPOSTAS

- 1xx: Informação
- 2xx: Sucesso
    - 200: OK
    - 201: CREATED
    - 204: não tem conteúdo PUT POST DELETE
- 3xx: Redirection
- 4xx: Client Error
    - 400: Bad Request
    - 404: Not Found!
- 5xx: Server Error
  500: Internal Server Error


  ## RESTFUL - Aplicação das regras
  - server.js




























