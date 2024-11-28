# STUDY-APP-React-Native
Aplicativo mobile

# Study App 2024-2

Este é um aplicativo mobile desenvolvido em **React Native** utilizando **Expo**. O objetivo é gerenciar tarefas e cartões de estudo, permitindo que os usuários criem, editem e organizem informações importantes para seus estudos. O aplicativo utiliza **Firebase** para autenticação e armazenamento de dados.
---
## 📝 **Descrição do Projeto**

O aplicativo oferece as seguintes funcionalidades principais:
- **Autenticação de Usuários**: Login e registro utilizando Firebase Authentication.
- **Gerenciamento de Cartões de Estudo**: Criação, edição, exclusão e listagem de cartões.
- **Controle de Prazos**: Exibição de tarefas e cartões com vencimentos próximos.
- **Persistência de Dados**: Utilização do Firestore para armazenamento remoto.
---
## 📂 **Estrutura do Projeto**

O projeto segue uma organização modular para facilitar a manutenção e escalabilidade. 
study-app-revisao-2024-2/ ├── .expo/ # Diretório gerenciado pelo Expo CLI ├── assets/ # Arquivos estáticos (imagens, ícones, etc.) ├── node_modules/ # Dependências instaladas via npm ├── src/ # Código-fonte principal do aplicativo │ ├── config/ # Configurações globais │ │ └── firebaseConfig.js # Configuração e inicialização do Firebase │ ├── contexts/ # Contextos globais para gerenciamento de estado │ │ ├── AuthContext.js # Contexto de autenticação │ │ └── CartoesEstudoContext.js # Contexto de gerenciamento de cartões │ ├── screens/ # Telas do aplicativo │ ├── EdicaoCartaoScreen.js # Tela de edição de cartões │ ├── ListaCartaoScreen.js # Tela de listagem de cartões │ ├── LoginScreen.js # Tela de login │ ├── RegistroScreen.js # Tela de registro de usuários │ └── TarefasVencimentoProximoScreen.js # Tela de controle de prazos ├── .env # Arquivo com variáveis de ambiente ├── .gitignore # Arquivos ignorados pelo Git ├── App.js # Arquivo principal que inicializa o app ├── app.json # Configuração específica do Expo ├── babel.config.js # Configuração do Babel ├── index.js # Ponto de entrada da aplicação ├── package.json # Gerenciamento de dependências e scripts └── package-lock.json # Controle de versões exatas das dependências
---

## 📋 **Descrição dos Arquivos**

### **1. Configurações**
- **firebaseConfig.js**: Configura e inicializa o Firebase Authentication e Firestore. Inclui persistência de autenticação com `AsyncStorage`.

### **2. Contextos**
- **AuthContext.js**: Gerencia o estado de autenticação (login, logout, usuário autenticado).
- **CartoesEstudoContext.js**: Gerencia operações relacionadas aos cartões de estudo, como adicionar, editar, excluir e listar.

### **3. Telas**
- **LoginScreen.js**: Tela de login, permite que os usuários façam autenticação.
- **RegistroScreen.js**: Tela para registro de novos usuários.
- **ListaCartaoScreen.js**: Exibe os cartões cadastrados pelo usuário.
- **EdicaoCartaoScreen.js**: Tela para editar informações de um cartão.
- **TarefasVencimentoProximoScreen.js**: Tela que mostra cartões ou tarefas com prazos próximos.

---

## 📦 **Bibliotecas Utilizadas**

| Biblioteca                                   | Finalidade                                                                 |
|---------------------------------------------|---------------------------------------------------------------------------|
| `expo`                                      | Plataforma para desenvolvimento com React Native.                        |
| `firebase`                                  | Integração com Firebase Authentication e Firestore.                      |
| `@react-native-async-storage/async-storage` | Persistência de dados local.                                              |
| `@react-navigation/native`                  | Gerenciamento de navegação entre telas.                                  |
| `@react-navigation/stack`                   | Navegação baseada em pilhas.                                              |
| `react-native-modal-datetime-picker`        | Seletor de data para cartões e tarefas.                                   |
| `react-native-vector-icons`                 | Ícones para melhorar a interface do usuário.                             |
| `dotenv`                                    | Gerenciamento de variáveis de ambiente para maior segurança.             |

---

## 🚀 **Como Configurar e Executar**

### **1. Clone o repositório**
```bash
git clone https://github.com/seu-usuario/study-app-revisao-2024-2.git
cd study-app-revisao-2024-2

2. Instale as dependências
Certifique-se de ter o Node.js e npm instalados:
npm install

3. Configure o Firebase
Crie um arquivo .env na raiz do projeto e adicione suas chaves do Firebase:
FIREBASE_API_KEY=your-api-key
FIREBASE_AUTH_DOMAIN=your-auth-domain
FIREBASE_PROJECT_ID=your-project-id
FIREBASE_STORAGE_BUCKET=your-storage-bucket
FIREBASE_MESSAGING_SENDER_ID=your-messaging-sender-id
FIREBASE_APP_ID=your-app-id


4. Inicie o projeto
Execute o seguinte comando para iniciar o Expo:
npm start
Escaneie o QR Code com o Expo Go (Android ou iOS).
🖥️ Descrição das Funcionalidades
Autenticação
•	Tela de Login: Permite que os usuários façam login com email e senha.
•	Tela de Registro: Registra novos usuários no sistema.
Gerenciamento de Cartões
•	Listagem: Exibe todos os cartões cadastrados.
•	Edição: Permite editar informações dos cartões.
•	Exclusão: Remove cartões específicos.
Controle de Prazos
•	Tela dedicada para exibir cartões ou tarefas com vencimentos próximos.

🛠️ Melhorias Futuras
•	Notificações Push: Lembretes para cartões com prazos próximos.
•	Modo Offline: Sincronização local com Firestore.
•	Filtro de Cartões: Opções para filtrar cartões por categoria ou prazo.
________________________________________
🤝 Contribuições
Contribuições são bem-vindas! Siga os passos abaixo para colaborar:
1.	Faça um fork do repositório.
2.	Crie uma branch para sua feature:
bash
Copiar código
git checkout -b minha-feature
3.	Faça as alterações e commit:
git commit -m "Descrição das alterações"
4.	Envie um pull request.

📜 Licença
Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.
