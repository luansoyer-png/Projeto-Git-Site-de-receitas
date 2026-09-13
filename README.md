# Manual de Delícias da Lanita

Sistema web para cadastro, busca e visualização de receitas culinárias.

O projeto foi desenvolvido utilizando **HTML, CSS e JavaScript**, com armazenamento das receitas no `localStorage` do navegador e implementação de operações CRUD.

## Funcionalidades

* Login com simulação de perfil de acesso
* Cadastro de novos usuários
* Cadastro de receitas
* Cadastro dinâmico de ingredientes
* Definição de receita pública ou privada
* Busca de receitas por nome
* Visualização completa da receita
* Exclusão de receitas
* Armazenamento utilizando `localStorage`
* CRUD de receitas

## CRUD

O sistema possui os seguintes métodos para gerenciamento das receitas:

```javascript
obterTodos()
obterPeloId(id)
salvar(receita)
atualizarPeloId(id, dadosAtualizados)
deletarPeloId(id)
```

### `obterTodos()`

Retorna todas as receitas armazenadas.

### `obterPeloId(id)`

Localiza uma receita específica através do seu ID.

### `salvar(receita)`

Cadastra uma nova receita e gera um ID único utilizando `crypto.randomUUID()`.

### `atualizarPeloId(id, dadosAtualizados)`

Atualiza os dados de uma receita existente.

### `deletarPeloId(id)`

Remove uma receita através do seu ID.

## Tecnologias utilizadas

* HTML5
* CSS3
* JavaScript
* LocalStorage
* DOM API
* Git
* GitHub

## Estrutura do projeto

```text
Manual-Lanita/
│
├── index.html
│
├── style.css
│
└── README.md
```




## Armazenamento

As receitas são armazenadas no `localStorage` do navegador utilizando a chave:

```javascript
receitas
```

Por isso, os dados ficam salvos localmente no navegador utilizado.

> Este projeto utiliza `localStorage` para fins de estudo e demonstração. Não é um banco de dados online.

## Perfis de acesso

O sistema possui dois perfis simulados:

### Usuário Padrão

Pode visualizar apenas receitas públicas.

### Usuário Privado

Pode visualizar receitas públicas e privadas.

## Exemplo de receita

Uma receita armazenada possui uma estrutura semelhante a:

```javascript
{
    id: "123456",

    nome: "Bolo de Chocolate",

    visibilidade: "publica",

    ingredientes: [
        {
            nome: "Farinha",
            quantidade: "500",
            unidade: "gramas",
            preparo: "ao natural"
        }
    ],

    preparo: "Misture todos os ingredientes...",

    tempo: "40",

    rendimento: "8 porções",

    categoria: "Doces"
}
```

## Objetivo do projeto

O projeto tem como objetivo praticar conceitos fundamentais de desenvolvimento web, principalmente:

* Manipulação do DOM
* Funções JavaScript
* Eventos
* Arrays e objetos
* `localStorage`
* CRUD
* Formulários
* Organização de código
* HTML semântico
* CSS responsivo
* Integração entre HTML, CSS e JavaScript

## Status

🚧 Projeto em desenvolvimento.

Novas funcionalidades poderão ser adicionadas futuramente, como:

* Edição de receitas
* Sistema de usuários real
* Banco de dados online
* Autenticação
* Favoritos
* Avaliação de receitas
* Upload de imagens
* Categorias
* Melhorias na responsividade

---

## Autor

**Luan Matos**

Projeto desenvolvido para fins de estudo e prática em desenvolvimento web.
