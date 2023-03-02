# Indice
- [Sobre](#-sobre)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Instalação do projeto](#-instalacao-do-projeto)

## Sobre

O projeto **VxTel** é um workspace de uma aplicação web (front end e back end) com intuito de calcular o custo total da ligação, seguindo uma tabela de preço enviada por email.
É o workspace do teste para a vaga de Full Stack da empresa **Vortx**.

---

### 🚀 Tecnologias utilizadas

O projeto utilizou as seguintes principais tecnologias:

#### Front End
- [ReactJS](https://reactjs.org)
- [Axios](https://github.com/axios/axios)
- [Typescript](https://www.typescriptlang.org)
- [Vite](https://vitejs.dev)


#### Back End
- [NestJs](https://nestjs.com/)
- [SwaggerUI](https://swagger.io/tools/swagger-ui/)
- [Typescript](https://www.typescriptlang.org)

---

###### O projeto consome uma API própria

- [api-vxTel](https://github.com/isabellasantiago/api-VxTel.git)

A port padrão da API é 3333, caso deseje mudar, no projeto contém um `.env.example`.
É só trocar o nome do arquivo para `.env` e o valor VITE_NODE_API para o qual desejar.

ps: é necessário que a API esteja rodando na mesma porta que informada no `.env`

## 🗂 Instalação do projeto


```bash
    # Clonar o repositório
    $ git clone --recurse-submodules https://github.com/isabellasantiago/vxTel.git
    # Entrar no diretório
    $ cd vxTel
    # Instalar as dependências da api
    $ cd api-vxTel
    $ yarn
    #Iniciando a API
    $ yarn start:dev
    # Rodar os testes
    $ yarn test

    #Instalar as dependências do front end
    $ cd web-vxTel
    $ yarn
    # Iniciar o front end
    $ yarn dev
```

O front end roda na porta 5173, porta padrão do Vite.
A api roda na porta 3333, porta padrão setada, mas podendo ser alterada através do `.env`.

Caso haja alteração na porta da API, é necessário atualizar a `.env` do front end.

--- 
###### Observações

Cada submódulo contém orientações em seus `README.md`.
A api contém a rota documentada através do **Swagger UI**, acessada pela rota `http://localhost:3333/docs`.

---

Desenvolvido 💜 por Isabella Santiago