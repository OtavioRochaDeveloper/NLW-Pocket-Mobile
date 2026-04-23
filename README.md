# 📍 Nearby — NLW Pocket Mobile

<p align="center">
  <img src="https://img.shields.io/badge/Expo-1B1F23?style=for-the-badge&logo=expo&logoColor=white" />
  <img src="https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" />
</p>

<p align="center">
  Aplicativo mobile de clube de benefícios desenvolvido durante o evento <strong>NLW Pocket Mobile</strong> da <a href="https://rocketseat.com.br">Rocketseat</a>.
</p>

---

## 📋 Sobre o Projeto

O **Nearby** é um aplicativo mobile que permite aos usuários encontrarem estabelecimentos parceiros próximos à sua localização e resgatar cupons de desconto e benefícios exclusivos. O projeto é composto por dois módulos:

- **Mobile (Frontend):** Aplicativo React Native com Expo
- **API (Backend):** Servidor Node.js com Express e Prisma ORM

---

## 🚀 Funcionalidades

- 📍 Listagem de estabelecimentos parceiros próximos ao usuário
- 🗺️ Integração com mapas para visualização geográfica dos locais
- 🎟️ Leitura de QR Code para resgate de cupons
- 🏷️ Filtragem de estabelecimentos por categoria
- 📄 Visualização dos detalhes de cada estabelecimento
- 🔗 Consumo de API REST com dados em tempo real

---

## 🛠️ Tecnologias Utilizadas

### 📱 Mobile (Frontend)

| Tecnologia | Versão | Descrição |
|---|---|---|
| React Native | — | Framework para apps mobile |
| Expo | SDK gerenciado | Plataforma de desenvolvimento |
| Expo Router | — | Navegação baseada em arquivos |
| TypeScript | ^5.6.3 | Tipagem estática |
| Expo Font | — | Carregamento de fontes customizadas |

### ⚙️ API (Backend)

| Tecnologia | Versão | Descrição |
|---|---|---|
| Node.js | — | Runtime JavaScript |
| Express | ^4.19.2 | Framework HTTP |
| Prisma ORM | ^5.21.0 | ORM para banco de dados |
| TypeScript | ^5.6.3 | Tipagem estática |
| Zod | ^3.23.8 | Validação de schemas |
| TSX | ^4.19.1 | Execução TypeScript em desenvolvimento |

---

## 📁 Estrutura do Projeto

```
NLW-Pocket-Mobile/
├── assets/
│   └── images/          # Ícones e imagens do app
├── prisma/
│   └── seed.ts          # Script de seed do banco de dados
├── src/                 # Código-fonte (mobile e/ou API)
├── app.json             # Configuração do Expo
├── package.json         # Dependências e scripts
└── tsconfig.json        # Configuração do TypeScript
```

---

## ⚙️ Como Rodar o Projeto

### Pré-requisitos

Antes de começar, você vai precisar ter instalado:

- [Node.js](https://nodejs.org/) (v18+)
- [npm](https://www.npmjs.com/) ou [yarn](https://yarnpkg.com/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/)
- [Expo Go](https://expo.dev/go) no celular (ou emulador Android/iOS)

---

### 🔧 Instalação

**1. Clone o repositório:**

```bash
git clone https://github.com/OtavioRochaDeveloper/NLW-Pocket-Mobile.git
cd NLW-Pocket-Mobile
```

**2. Instale as dependências:**

```bash
npm install
```

---

### 🗄️ Configurando o Banco de Dados (API)

**3. Execute as migrations e o seed:**

```bash
npx prisma migrate dev
npm run prisma -- db seed
```

**4. Inicie a API:**

```bash
npm run start
```

> A API estará disponível em: `http://localhost:3333`

---

### 📱 Rodando o App Mobile

**5. Inicie o servidor Expo:**

```bash
npx expo start
```

**6. Acesse o app:**
- Escaneie o QR Code com o **Expo Go** (Android/iOS)
- Ou pressione `a` para abrir no emulador Android
- Ou pressione `i` para abrir no simulador iOS

---

## 📜 Scripts Disponíveis

### API

| Comando | Descrição |
|---|---|
| `npm run start` | Inicia a API em modo watch (tsx) |
| `npm run knex` | Executa comandos do Knex |

### Mobile

| Comando | Descrição |
|---|---|
| `npx expo start` | Inicia o servidor de desenvolvimento |
| `npx expo build` | Gera build de produção |

---

## 🌐 Endpoints da API

> Base URL: `http://localhost:3333`

| Método | Rota | Descrição |
|---|---|---|
| GET | `/categories` | Lista todas as categorias |
| GET | `/markets/category/:id` | Lista mercados por categoria |
| GET | `/markets/:id` | Detalhes de um mercado |
| PATCH | `/coupons/:qrcode` | Resgata um cupom via QR Code |

---

## 🎨 Layout

O layout do projeto foi desenvolvido no Figma e está disponível no evento NLW Pocket Mobile da Rocketseat.

- Paleta de cor principal: `#257F49` (verde)
- Suporte a temas claro e escuro (`userInterfaceStyle: "automatic"`)
- Orientação: Portrait

---

## 👨‍💻 Autor

Desenvolvido por **Otávio Rocha** durante o evento **NLW Pocket Mobile** da [Rocketseat](https://rocketseat.com.br).

- GitHub: [@OtavioRochaDeveloper](https://github.com/OtavioRochaDeveloper)

---

## 📝 Licença

Este projeto está sob a licença **ISC**. Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

---

<p align="center">
  Feito com 💚 durante o NLW Pocket Mobile · Rocketseat
</p>
