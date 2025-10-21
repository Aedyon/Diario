Projeto Diário Pessoal com React Native e Supabase

Este é um aplicativo de diário pessoal desenvolvido com React Native e Expo, utilizando Supabase como backend para autenticação, banco de dados e armazenamento de arquivos.

🚀 Tecnologias Utilizadas

Este projeto foi construído utilizando as seguintes tecnologias:

React Native: Framework para desenvolvimento de aplicativos móveis multiplataforma (Android e iOS).

Expo: Plataforma e conjunto de ferramentas para facilitar o desenvolvimento e a publicação de apps React Native.

Supabase:

Supabase Auth: Para gerenciamento completo de autenticação de usuários (cadastro, login e logout).

Supabase Database: Banco de dados PostgreSQL para armazenar as entradas do diário (título, conteúdo, etc.).

Supabase Storage: Para fazer o upload e armazenamento seguro de mídias (imagens, vídeos ou áudios) associadas a cada entrada.

Expo Image Picker: Para permitir que o usuário selecione imagens e vídeos da galeria do dispositivo.

Expo AV: Para manipulação e exibição de áudio e vídeo no aplicativo.

✨ Funcionalidades Implementadas

O aplicativo conta com as seguintes funcionalidades:

Autenticação de Usuário:

Tela de Login para usuários existentes.

Tela de Registro para novos usuários.

Funcionalidade de Logout seguro para encerrar a sessão.

Gerenciamento de Entradas do Diário:

Criação: Adição de novas entradas com título, conteúdo em texto e anexo de mídias.

Listagem: Visualização de todas as entradas do diário em uma lista cronológica.

Visualização Detalhada: Acesso ao conteúdo completo de uma entrada específica.

Exclusão: Remoção de entradas do diário.

Upload de Mídia:

O usuário pode fazer o upload de imagens, vídeos ou áudios ao criar uma nova entrada.

Os arquivos são enviados para o Supabase Storage e associados à respectiva entrada no banco de dados.

⚙️ Como Rodar o Projeto

Siga os passos abaixo para configurar e executar o projeto em seu ambiente de desenvolvimento.

Pré-requisitos

Node.js (versão LTS recomendada)

Git

Conta no Supabase para criar seu projeto backend.

Expo Go instalado em seu dispositivo móvel (Android ou iOS) ou um emulador configurado.

Passos para Instalação

Clone o repositório:

git clone [https://github.com/seu-usuario/nome-do-repositorio.git](https://github.com/seu-usuario/nome-do-repositorio.git)
cd nome-do-repositorio


Instale as dependências:

npm install


Configure as variáveis de ambiente:

Crie um arquivo chamado .env na raiz do projeto.

Adicione as chaves da sua API do Supabase, que podem ser encontradas no painel do seu projeto em Project Settings > API.

Arquivo .env:

EXPO_PUBLIC_SUPABASE_URL="URL_DO_SEU_PROJETO_SUPABASE"
EXPO_PUBLIC_SUPABASE_ANON_KEY="SUA_CHAVE_ANON_PUBLICA"


Configure o Supabase:

No seu painel do Supabase, navegue até Storage e crie um novo "Bucket" (por exemplo, com o nome media).

Certifique-se de que as políticas de acesso do bucket permitem o upload e a visualização de arquivos para usuários autenticados.

Execute o projeto:

npm start


ou

npx expo start


Abra no seu dispositivo:

Após executar o comando acima, um QR code será exibido no terminal.

Abra o aplicativo Expo Go em seu celular e escaneie o QR code para carregar o aplicativo.

Feito com ❤️ para a atividade de desenvolvimento mobile.
