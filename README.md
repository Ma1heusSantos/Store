# Store App

Este é um aplicativo de e-commerce desenvolvido com **React Native** e **Expo Router**. Ele permite que os usuários naveguem por categorias de produtos, visualizem detalhes de produtos e explorem informações do perfil.

## Estrutura do Projeto

A estrutura do projeto está organizada da seguinte forma:

```
├── app/                # Contém as telas e layouts do aplicativo
│   ├── _layout.tsx     # Layout principal do aplicativo
│   ├── index.tsx       # Tela inicial
│   ├── (tabs)/         # Navegação por abas
│       ├── _layout.tsx # Layout das abas
│       ├── home.tsx    # Tela inicial das abas
│       ├── profile.tsx # Tela de perfil
│       └── categories/ # Tela de categorias
│           ├── _layout.tsx
│           ├── category.tsx
│           └── [id].tsx
├── assets/             # Recursos estáticos (imagens, fontes, etc.)
├── components/         # Componentes reutilizáveis
├── constants/          # Constantes globais
├── data/               # Dados mockados para categorias e produtos
├── services/           # Serviços para manipulação de dados
├── types/              # Tipos TypeScript para categorias e produtos
├── .expo/              # Configurações do Expo
├── .vscode/            # Configurações do Visual Studio Code
├── package.json        # Dependências e scripts do projeto
├── tsconfig.json       # Configurações do TypeScript
└── app.json            # Configurações do Expo
```

## Funcionalidades

- **Navegação por abas**: Home, Categorias e Perfil.
- **Listagem de produtos**: Exibição de produtos por categoria.
- **Detalhes do produto**: Visualização de informações detalhadas de um produto.
- **Perfil do usuário**: Exibição de informações de contato e links sociais.

## Tecnologias Utilizadas

- **React Native**: Framework para desenvolvimento mobile.
- **Expo**: Ferramenta para simplificar o desenvolvimento React Native.
- **Expo Router**: Gerenciamento de rotas baseado em arquivos.
- **TypeScript**: Tipagem estática para JavaScript.
- **React Navigation**: Navegação no aplicativo.

## Como Executar o Projeto

1. Certifique-se de ter o **Node.js** e o **Expo CLI** instalados.
2. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/store-app.git
   ```
3. Instale as dependências:
   ```bash
   npm install
   ```
4. Inicie o aplicativo:
   ```bash
   npm start
   ```
5. Escaneie o QR Code no terminal com o aplicativo **Expo Go** ou execute no emulador.

## Scripts Disponíveis

- `npm start`: Inicia o servidor de desenvolvimento.
- `npm run android`: Executa o aplicativo no emulador Android.
- `npm run ios`: Executa o aplicativo no emulador iOS.
- `npm run web`: Executa o aplicativo no navegador.
- `npm test`: Executa os testes com Jest.

## Estrutura de Dados

### Categoria

```ts
type Category = {
  id: number;
  title: string;
  cover: string;
};
```

### Produto

```ts
type Product = {
  id: number;
  idCategory: number;
  image: string;
  title: string;
  description: string;
  price: number;
};
```

## Contribuição

1. Faça um fork do repositório.
2. Crie uma branch para sua feature:
   ```bash
   git checkout -b minha-feature
   ```
3. Faça commit das suas alterações:
   ```bash
   git commit -m "Minha nova feature"
   ```
4. Envie para o repositório remoto:
   ```bash
   git push origin minha-feature
   ```
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais informações.
