# Chat de Amor 💕

Um aplicativo de chat em tempo real com conexão via código de convite, desenvolvido com Firebase e JavaScript moderno.

## 🌐 Demo Online

Acesse a versão online do chat: [Chat de Amor](https://theuscirilo.github.io/Chat_Amor/)

## ✨ Funcionalidades

- 🔐 Autenticação segura com email/senha
- 🔑 Sistema de código de convite único para cada usuário
- 💬 Chat em tempo real
- 📱 Interface responsiva e moderna
- 👁️ Status de visualização das mensagens
- ⏰ Horário das mensagens
- 🟢 Indicador de status online
- 📋 Cópia fácil do código de convite

## 🚀 Tecnologias Utilizadas

- Firebase Authentication
- Firebase Firestore
- JavaScript (ES6+)
- HTML5
- CSS3
- Font Awesome Icons
- Google Fonts

## 🛠️ Configuração

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/chat-de-amor.git
cd chat-de-amor
```

2. Instale as dependências:
```bash
npm install
```

3. Configure o Firebase:
   - Crie um projeto no [Firebase Console](https://console.firebase.google.com)
   - Ative a autenticação com email/senha
   - Configure o Firestore Database
   - Substitua as configurações do Firebase no arquivo `index.html` e `chat.html`

4. Inicie o servidor local:
```bash
npm start
```

5. Acesse o chat em `http://localhost:8080`

## 📱 Como Usar

1. Acesse a página inicial
2. Digite seu nome para criar uma conta
3. Copie seu código de convite único
4. Compartilhe o código com quem você quer conversar
5. A outra pessoa deve:
   - Acessar o chat
   - Criar sua conta
   - Colar seu código de convite
   - Clicar em "Conectar"

## 🔒 Regras do Firestore

```javascript
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{userId} {
      allow read: if request.auth != null;
      allow write: if request.auth != null && request.auth.uid == userId;
    }
    match /messages/{messageId} {
      allow read: if request.auth != null;
      allow create: if request.auth != null;
      allow update: if request.auth != null;
    }
  }
}
```

## 🎨 Personalização

O chat usa variáveis CSS para fácil personalização:

```css
:root {
  --primary: #4834d4;
  --primary-light: #6f5ff6;
  --secondary: #ffaac3;
  --accent: #fd6f96;
  --bg-color: #f8f9fb;
  --text-color: #1a1a2e;
}
```

## 🤝 Contribuindo

1. Faça um Fork do projeto
2. Crie uma Branch para sua Feature (`git checkout -b feature/AmazingFeature`)
3. Faça o Commit das suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Faça o Push para a Branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👥 Autores

- Matheus Cirilo - [@Theuscirilo](https://github.com/Theuscirilo)

## 🙏 Agradecimentos

- Firebase por fornecer uma plataforma incrível
- Comunidade open source
- Todos os contribuidores

## 📞 Suporte

Se você encontrar algum problema ou tiver alguma sugestão, por favor abra uma issue no GitHub.

---

Feito com ❤️ por [Matheus](https://github.com/Theuscirilo)