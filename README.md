# pass.in

O pass.in é uma aplicação de **gestão de participantes em eventos presenciais**. 

A ferramenta permite que o organizador cadastre um evento e abra uma página pública de inscrição.

Os participantes inscritos podem emitir uma credencial para check-in no dia do evento.

O sistema fará um scan da credencial do participante para permitir a entrada no evento.

## Requisitos

### Requisitos funcionais

- [x] O organizador deve poder cadastrar um novo evento;
- [x] O organizador deve poder visualizar dados de um evento;
- [x] O organizador deve poder visualizar a lista de participantes; 
- [x] O participante deve poder se inscrever em um evento;
- [x] O participante deve poder visualizar seu crachá de inscrição;
- [x] O participante deve poder realizar check-in no evento;

### Regras de negócio

- [x] O participante só pode se inscrever em um evento uma única vez;
- [x] O participante só pode se inscrever em eventos com vagas disponíveis;
- [x] O participante só pode realizar check-in em um evento uma única vez;

### Requisitos não-funcionais

- [x] O check-in no evento será realizado através de um QRCode;

# Anotações

Métodos HTTP: Get, POST, PUT, DELETE, PATCH, HEAD, OPTIONS, ...

Corpo da requisição (Request Body)
Parâmetros de busca (Search Params / Query Params) 'http://localhost:3333/users?name=Emerson'
Parâmetros de rota (Route Params) -> Identificação de recursos 'DELETE http://localhost:3333/users/5'
Cabeçalhos (Headers) -> Contexto

Semânticas = Significado

Driver nativo / Query Builders / ORMs

Object Relational Mapping (Hibernate / Doctrine / ActiveRecord)

JSON - JavaScript Object Notation

20x => Sucesso
30x => Redirecionamento
40x => Erro do cliente (Erro em alguma informação enviada por QUEM está fazendo a chamada p/ API)
50x => Error do servidor (Um erro que está acontecendo INDEPENDENTE do que está sendo enviado p/ o servidor)
