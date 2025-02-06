# demo-dotnetcore-graphql
Demonstração de implementação de graphql server com .net 

Para acessar: https://localhost:56307/graphql/


## Exemplo de mutação para add.

```
mutation {
  criarUsuario(usuario: {
    id: 4,
    nome: "Nome do Usuário",
    idade: 30
  }) {
    id
    nome
    idade
  }
}
```

get all usuarios
```
{ usuario {id, nome, dataCriacao, dataAlteracao, idade}}
```

com filtro
```
{ usuario (id:2) {
  id, nome
} }

```