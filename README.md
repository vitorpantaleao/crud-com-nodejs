# CRUD com NodeJS e Express

## Projeto criado para estudos com NodeJs.

* Após clonar o projeto, instale as dependências com o comando abaixo:

`npm install`

* Inicialize o servidor através do arquivo index.js usando o node:

`node index.js`

O servidor será inicializado em [http://localhost:3000](http://localhost:3000)

* Após inicializar o servidor, utilize o Insomnia (ou o plugin Thunder Client do VSCode) para realizar as consultas e testes.

## Para criar um novo curso

Envie um **POST** para [http://localhost:3000/cursos/](http://localhost:3000/cursos/) no formato `JSON` seguindo o exemplo abaixo, informando o nome do curso que deseja adicionar:

`{
    "name": "React Js"
 }`

## Listar todos os cursos

Envie uma requisição do tipo **GET** para http://localhost:3000/cursos

## Listar um único curso

Envie uma requisição do tipo **GET** para http://localhost:3000/cursos/1

*o número após **`/cursos`** é o index do item que deseja listar* 

## Atualizar um curso existente

Envie uma requisição do tipo `PUT` para [http://localhost:3000/cursos/2](http://localhost:3000/cursos/2) passando na URL depois de `/cursos` o número do curso que deseja atualizar, contendo um `JSON` no formato abaixo:

`{
    "name": "React Js"
 }`

 ## Deletar um curso existente

Envie uma requisição do tipo `DELETE` para [http://localhost:3000/cursos/2](http://localhost:3000/cursos/2) passando na URL depois de `/cursos` o número do curso que deseja deletar, contendo um `JSON` no formato abaixo:

`{
    "name": "React Js"
 }`