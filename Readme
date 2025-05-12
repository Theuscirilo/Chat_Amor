# Chat de Amor - README

Este é um projeto de um aplicativo de chat com foco em conexões amorosas. Ele oferece funcionalidades de login, cadastro com foto de perfil, e um sistema básico para exibir o status da conexão e notificações. O projeto utiliza Firebase para autenticação, armazenamento de dados (Firestore) e armazenamento de arquivos (Storage).

## Funcionalidades

* **Login:** Permite que usuários existentes façam login com seu email e senha.
* **Cadastro:** Novos usuários podem se cadastrar fornecendo nome, email, senha e opcionalmente uma foto de perfil.
* **Upload de Foto de Perfil:** Durante o cadastro, os usuários podem adicionar uma foto de perfil que é armazenada no Firebase Storage.
* **Status de Conexão:** Exibe visualmente se o usuário está online ou offline, e também indica a conexão com o Firebase.
* **Notificações Toast:** Um sistema de notificações visuais para informar os usuários sobre o sucesso ou falha de operações como login e cadastro, além de problemas de conexão.
* **Persistência Offline:** O Firestore está configurado para habilitar a persistência offline, permitindo que o aplicativo funcione de forma mais resiliente em conexões instáveis.
* **Tratamento de Erros e Reconexão:** Implementa tentativas de reconexão automáticas para operações do Firebase em caso de falha na rede.

## Tecnologias Utilizadas

* **HTML:** Estrutura da página web.
* **CSS:** Estilos visuais, incluindo um tema claro e um tema escuro (o tema escuro não está totalmente implementado neste trecho de código, mas as variáveis CSS estão definidas).
* **JavaScript:** Lógica da aplicação, manipulação do DOM e integração com o Firebase.
* **Firebase:**
    * **Firebase Authentication:** Para autenticação de usuários (login e cadastro).
    * **Firebase Firestore:** Banco de dados NoSQL para armazenar informações dos usuários e futuras mensagens do chat.
    * **Firebase Storage:** Para armazenar as fotos de perfil dos usuários.
    * **Firebase SDK (Compatibilidade):** As bibliotecas JavaScript do Firebase para integrar os serviços ao aplicativo web.
* **Font Awesome:** Para ícones.
* **Google Fonts (Poppins):** Para a tipografia da página.

## Configuração do Firebase

Para executar este projeto, você precisará de uma conta no Firebase e um projeto configurado. Siga estes passos:

1.  **Crie um Projeto no Firebase:**
    * Acesse o [Firebase Console](https://console.firebase.google.com/).
    * Clique em "Adicionar projeto".
    * Siga as instruções para dar um nome ao seu projeto e configurá-lo.

2.  **Configure a Autenticação:**
    * No menu lateral do Firebase Console, vá em "Authentication".
    * Na aba "Sign-in methods", habilite o método de autenticação por "Email/password".

3.  **Configure o Firestore:**
    * No menu lateral, vá em "Firestore Database".
    * Clique em "Criar banco de dados".
    * Escolha o modo de início (recomenda-se o modo de teste para desenvolvimento, mas lembre-se de configurar as regras de segurança para produção).
    * Selecione a localização do seu banco de dados.

4.  **Configure o Storage:**
    * No menu lateral, vá em "Storage".
    * Clique em "Começar".
    * Leia e entenda as regras de segurança (você precisará ajustá-las para seu aplicativo em produção).
    * Clique em "Próximo" e selecione a localização do seu bucket.

5.  **Obtenha as Chaves de Configuração:**
    * No seu projeto do Firebase Console, clique no ícone de engrenagem (Configurações do projeto) ao lado de "Visão geral do projeto".
    * Na aba "Geral", role para baixo até encontrar a seção "Seus aplicativos".
    * Clique no ícone "</>" (Web) para adicionar um aplicativo web ao seu projeto, se ainda não tiver feito isso.
    * Siga as instruções e copie o objeto `firebaseConfig` que será fornecido.

6.  **Atualize o Código:**
    * No arquivo HTML (`index.html` ou o nome do seu arquivo principal), localize a seção de configuração do Firebase (dentro da tag `<script>`).
    * Substitua os valores de `apiKey`, `authDomain`, `projectId`, `storageBucket`, `messagingSenderId`, `appId` e `measurementId` pelos seus valores obtidos no Firebase Console.

    ```javascript
    const firebaseConfig = {
      apiKey: "SUA_API_KEY",
      authDomain: "SEU_AUTH_DOMAIN.firebaseapp.com",
      projectId: "SEU_PROJECT_ID",
      storageBucket: "SEU_STORAGE_BUCKET.appspot.com",
      messagingSenderId: "SEU_MESSAGING_SENDER_ID",
      appId: "SEU_APP_ID",
      measurementId: "SEU_MEASUREMENT_ID"
    };
    ```

## Como Executar

1.  **Salve o arquivo HTML:** Salve o código HTML em um arquivo com a extensão `.html` (por exemplo, `index.html`).
2.  **Abra no Navegador:** Abra o arquivo `index.html` no seu navegador web.

O aplicativo deverá exibir a interface de login e cadastro. Certifique-se de que sua conexão com a internet esteja ativa para que o Firebase possa ser inicializado corretamente.

## Próximos Passos (Para Continuar o Desenvolvimento)

* **Implementar a Interface do Chat:** Adicionar a estrutura HTML e CSS para exibir a lista de contatos/conversas e a área de mensagens.
* **Lógica do Chat:** Implementar as funcionalidades para enviar e receber mensagens em tempo real usando o Firebase Firestore.
* **Listagem de Usuários Online:** Exibir uma lista de usuários online.
* **Mensagens Privadas:** Permitir que os usuários iniciem conversas privadas.
* **Estilos do Chat:** Adicionar estilos para as mensagens enviadas e recebidas, timestamps, etc.
* **Melhorias na Interface:** Tornar a interface responsiva e melhorar a experiência do usuário.
* **Testes:** Escrever testes para garantir a funcionalidade e a robustez do aplicativo.
* **Regras de Segurança do Firebase:** Configurar regras de segurança adequadas no Firestore e Storage para proteger os dados dos usuários.
* **Tema Escuro:** Completar a implementação do tema escuro.

Este README fornece uma visão geral do código fornecido e os passos iniciais para configurar e executar o projeto. O desenvolvimento de um aplicativo de chat completo requer um conhecimento mais aprofundado das funcionalidades do Firebase e das tecnologias web.