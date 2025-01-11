# Painel de Controle de Estoque - Sistema Open Source

**Controle de Estoque** é uma plataforma moderna e eficiente para gestão de inventário, desenvolvido como um sistema open-source e acessível para empresas de todos os tamanhos. Este projeto oferece uma interface intuitiva, com funcionalidades de cadastro de produtos, usuários e visualização de dados de estoque, construído com as tecnologias mais modernas da web.

## Características Principais
- **Interface de Usuário Moderna**: Baseada em um design limpo e funcional, com gráficos interativos para visualização de dados.
- **Gerenciamento de Produtos**: Cadastro de produtos com quantidades e gerenciamento direto via navegador.
- **Cadastro de Usuários**: Funcionalidade para adicionar e gerenciar novos usuários diretamente no painel.
- **Armazenamento no Navegador**: Utiliza a tecnologia **Dexie.js** para persistência de dados localmente no navegador, garantindo um uso eficiente e sem necessidade de servidores backend.
- **Integração com Gráficos**: Visualização dos dados de estoque através de gráficos interativos utilizando **Chart.js**.
- **Criptografia JWT**: Segurança adicional com a biblioteca **JWT-simple** para criptografar senhas de usuários.

## Tecnologias Utilizadas
- **HTML5, CSS3 e JavaScript**: Para a estruturação e interação do frontend.
- **ReactJS (via CDN)**: Para manipulação eficiente do DOM e criação de interações dinâmicas.
- **Chart.js**: Para a criação de gráficos interativos, visualizando a quantidade de produtos no estoque.
- **Dexie.js**: Uma biblioteca que facilita o gerenciamento de banco de dados no navegador, utilizando IndexedDB.
- **JWT Simple**: Para segurança no armazenamento e criptografia de senhas de usuários.
- **CDNs do Bootstrap, Materialize e FontAwesome**: Para estilização rápida e responsiva, além da adição de ícones modernos.

## Funcionalidades
### 1. **Gerenciamento de Estoque**
   - O painel de controle permite adicionar produtos ao estoque com nome e quantidade.
   - Os produtos são armazenados localmente no navegador, utilizando IndexedDB através do Dexie.js.
   - Exibição de gráficos interativos (Chart.js) mostrando a quantidade de produtos no estoque em tempo real.

### 2. **Cadastro de Usuários**
   - Cadastro de usuários com autenticação básica.
   - Utilização de **JWT** para criptografar senhas antes de armazená-las no banco de dados local.

### 3. **Autenticação Local**
   - O sistema autentica o usuário com a base de dados local e valida se está logado ao acessar o painel.
   - Logout simples com remoção de dados da sessão.

## Estrutura do Projeto
```plaintext
.
├── index.html             # Página inicial com o formulário de login
├── page.html              # Painel de controle de estoque
├── README.md              # Documentação do projeto
└── style.css              # Arquivo de estilos CSS
└── scripts.js             # Funcionalidades JavaScript
└── package.json           # Dependências e configuração de pacotes
