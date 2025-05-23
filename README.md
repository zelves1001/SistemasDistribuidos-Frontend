# Chat App - Frontend

Frontend para aplicação de chat do projeto de Sistemas Distribuídos, construído com React, TypeScript e Material UI.

## Funcionalidades

- Login com nickname
- Chat em tempo real usando SignalR
- Histórico de mensagens
- Design responsivo com Material UI
- Redefinição do histórico de chat

## Tecnologias Utilizadas

- React 18
- TypeScript
- Material UI
- SignalR para comunicação em tempo real
- Axios para requisições HTTP
- React Router para navegação

## Pré-requisitos

- Node.js (v14 ou superior)
- NPM (v6 ou superior)

## Como executar

1. Clone o repositório
2. Navegue até a pasta do projeto:
   ```
   cd C:\Users\jpontes\Desktop\Tudo\SistemaDistribuidos\frontend\chat-app-new
   ```
3. Instale as dependências:
   ```
   npm install
   ```
4. Execute o aplicativo:
   ```
   npm start
   ```
5. Abra o navegador em [http://localhost:3000](http://localhost:3000)

## Estrutura do Projeto

- `src/`
  - `components/` - Componentes reutilizáveis
  - `contexts/` - Contextos do React
  - `pages/` - Páginas principais
  - `services/` - Serviços para comunicação com o backend
  - `App.tsx` - Componente principal
  - `index.tsx` - Ponto de entrada

## Detalhes da Comunicação com o Backend

- A aplicação se comunica com o backend através de SignalR e REST API
- SignalR é utilizado para comunicação em tempo real
- REST API é utilizada como fallback e para operações específicas

## Backend

O backend deve estar rodando em https://localhost:7099 com os seguintes endpoints:

- SignalR Hub: `/chatHub`
- REST API: `/api/Chat/*`

## Resolução de Problemas

### CORS

Se encontrar problemas de CORS, verifique se o backend está configurado para permitir requisições de `http://localhost:3000`.

### SSL/HTTPS

Se estiver utilizando certificados autoassinados, pode ser necessário aceitar o certificado manualmente acessando o endpoint do backend diretamente no navegador.

### Redis

Esta aplicação depende do Redis para armazenamento de mensagens no backend. Certifique-se que o Redis está rodando e acessível pelo backend.
#   S i s t e m a s D i s t r i b u i d o s - F r o n t e n d  
 