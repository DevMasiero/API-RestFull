# API CRUD - Simulador de Backend do YouTube

Esta é uma API RESTful que simula o backend do YouTube, implementando um padrão CRUD (Create, Read, Update, Delete) para gerenciar vídeos. A aplicação é construída com Fastify e utiliza PostgreSQL hospedado no Neon.tech. A API está configurada para rodar na porta 3333.

## Funcionalidades

- **Cadastrar Vídeos (Create)**: Adicione novos vídeos com título, descrição, URL e outras informações relevantes.
- **Listar Vídeos (Read)**: Recupere todos os vídeos cadastrados.
- **Buscar Vídeo (Read)**: Obtenha detalhes de um vídeo específico.
- **Atualizar Vídeo (Update)**: Modifique as informações de vídeos existentes.
- **Remover Vídeo (Delete)**: Exclua vídeos que não são mais necessários.

## Tecnologias Utilizadas

- **Linguagem**: JavaScript
- **Framework**: Fastify
- **Banco de Dados**: PostgreSQL (Neon.tech)
- **Porta**: 3333

## Instalação

### Pré-requisitos

- Node.js (versão 14 ou superior)
- Conta no Neon.tech com um banco de dados configurado

### Passos para Instalação

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/api-youtube-simulator.git
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd api-youtube-simulator
   ```

3. Instale as dependências:
   ```bash
   npm install
   ```

4. Configure suas credenciais do banco de dados no arquivo `.env`:
   ```env
   DB_HOST=your_neon_db_host
   DB_USER=your_db_user
   DB_PASSWORD=your_db_password
   DB_NAME=your_db_name
   ```

5. Inicie o servidor:
   ```bash
   npm run dev
   ```

6. Acesse a API em `http://localhost:3333`.

## Uso

A API disponibiliza os seguintes endpoints seguindo o padrão CRUD:

- **POST /videos**: Cadastrar um novo vídeo.
- **GET /videos**: Listar todos os vídeos.
- **GET /videos/:id**: Obter detalhes de um vídeo específico.
- **PUT /videos/:id**: Atualizar informações de um vídeo.
- **DELETE /videos/:id**: Remover um vídeo.

### Exemplo de Requisições

- **Cadastrar um Vídeo**:
   ```bash
   curl -X POST http://localhost:3333/videos -H "Content-Type: application/json" -d '{"title": "Meu Vídeo", "description": "Descrição do vídeo", "url": "http://exemplo.com/video"}'
   ```

- **Listar Vídeos**:
   ```bash
   curl -X GET http://localhost:3333/videos
   ```

## Contribuição

Contribuições são bem-vindas! Se você deseja contribuir com melhorias ou correções, siga os passos abaixo:

1. Fork o repositório.
2. Crie uma nova branch (`git checkout -b minha-feature`).
3. Faça suas alterações e commit (`git commit -m 'Adicionando uma nova feature'`).
4. Envie para o repositório remoto (`git push origin minha-feature`).
5. Abra um pull request.

## Contato

Para dúvidas ou sugestões, entre em contato pelo e-mail: andremasierodev@gmail.com
```
