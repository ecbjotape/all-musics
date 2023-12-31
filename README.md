# ALL MUSICS

## Descrição
Este projeto é uma aplicação Vue.js que integra as APIs do YouTube e Spotify para acessar e reproduzir listas de reprodução do usuário.

## Funcionalidades
- Autenticação OAuth 2.0 para YouTube e Spotify.
- Recuperação de listas de reprodução do usuário a partir das APIs do YouTube e Spotify.
- Reprodução de músicas do YouTube e Spotify.

## Instalação
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-projeto.git
   cd seu-projeto

## Instale as dependências:
npm install

## Configure as variáveis de ambiente:

Crie um arquivo .env.local na raiz do projeto e adicione suas credenciais:
VUE_APP_YOUTUBE_CLIENT_ID=SEU_CLIENT_ID_DO_YOUTUBE
VUE_APP_YOUTUBE_AUTH_URL=URL_DE_AUTORIZACAO_DO_YOUTUBE
VUE_APP_YOUTUBE_REDIRECT_URI=URL_DE_RETORNO_DO_SEU_APLICATIVO

VUE_APP_SPOTIFY_CLIENT_ID=SEU_CLIENT_ID_DO_SPOTIFY
VUE_APP_SPOTIFY_AUTH_URL=URL_DE_AUTORIZACAO_DO_SPOTIFY
VUE_APP_SPOTIFY_REDIRECT_URI=URL_DE_RETORNO_DO_SEU_APLICATIVO

## Inicie o servidor de desenvolvimento:
npm run serve
Acesse a aplicação em http://localhost:8080.

## Configuração da Autenticação OAuth
Google Developers Console: Crie um projeto, ative a API do YouTube e configure as credenciais OAuth.
Spotify for Developers: Crie um aplicativo, configure as permissões e obtenha as credenciais OAuth.

## Uso
Implemente funcionalidades adicionais e melhore a interface do usuário conforme necessário.
Adicione a lógica de reprodução de músicas usando bibliotecas de áudio como Howler.js ou React Player.
Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas ou enviar pull requests.


Certifique-se de substituir os marcadores de posição, como `SEU_CLIENT_ID_DO_YOUTUBE`, `URL_DE_AUTORIZACAO_DO_YOUTUBE`, etc., pelos valores reais do seu projeto. Se você tiver uma licença específica, substitua `URL_DA_LICENCA` pela URL ou nome da sua licença.
