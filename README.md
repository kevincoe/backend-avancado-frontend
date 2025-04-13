# 💼 Frontend Gerente Banco MVP 🚀

Este projeto implementa um sistema completo de gerenciamento bancário, permitindo a administração de clientes e investimentos. O sistema oferece uma interface amigável para gerentes bancários gerenciarem seus clientes e um concierge de investimentos para auxiliar na compra de ações e dólares. 🏦

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** 📄  
- **CSS3** 🎨  
- **JavaScript** 🛠️  
- **Docker** 🐳
---

## 🗂️ Estrutura do Projeto

```plaintext
backend-avancado-frontend/
├── concierge.html         # Interface do concierge de investimentos
├── Dockerfile             # Configuração para containerização
├── index.html             # Interface principal de gerenciamento
├── README.md              # Documentação do projeto
├── css/
│   ├── concierge.css      # Estilos para a interface do concierge
│   └── styles.css         # Estilos gerais da aplicação
├── img/
│   └── smart-bank.png     # Logo e imagens do sistema
└── js/
    ├── api.js             # Comunicação com a API backend
    ├── cliente.js         # Modelo de dados do cliente
    ├── clienteService.js  # Serviço de gerenciamento de clientes
    ├── investimentos.js   # Lógica para gestão de investimentos
    └── main.js            # Lógica principal da aplicação
```

### 🖊 Descrição dos Arquivos

- **css/styles.css**  
  Contém os estilos CSS utilizados na interface da aplicação.

- **css/concierge.css**  
  Estilos específicos para a interface do concierge

- **index.html**  
  Arquivo principal que estrutura a interface do usuário.

- **concierge.html**  
  Interface especializada para gestão de investimentos.

- **js/api.js**  
  Define a classe `Api` para interação com o backend RESTful.

- **js/cliente.js**  
  Define o modelo `Cliente` com suas propriedades.

- **js/clienteService.js**  
  Serviço que abstrai operações com clientes.

- **js/main.js**  
  Lógica principal de interação e eventos da interface de clientes.

- **js/investimentos.js**  
  Lógica para a interface de concierge de investimentos

---

## ⚙️ Como Configurar e Executar

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/kevincoe/backend-avancado-frontend.git
   cd backend-avancado-frontend
   ```

2. **Construa a imagem Docker**
   ```bash
   docker build -t backend-avancado-frontend .
   ```

3. **Execute o Contêiner:**
   ```bash
   docker run -p 80:80 backend-avancado-frontend
   ```

4. **Acesse a aplicação**
   - Abra seu navegador e acesse http://localhost

---

## 📋 Funcionalidades

### 🧑‍💼 Clientes

- **Listar Clientes:**  
  Exibe todos os clientes cadastrados no sistema.

- **Adicionar Cliente:**  
  Permite cadastrar novos clientes no banco.

- **Editar Cliente:**  
  Atualiza as informações de clientes existentes.

- **Remover Cliente:**  
  Exclui clientes do sistema de forma prática.

- **Pesquisar Cliente:**  
  Encontre clientes por nome ou número de conta.

---

### 💰 Concierge de Investimentos

- **Seleção de Cliente:**
  Escolha um cliente para gerenciar investimentos.

- **Visualização de Portfoli:**
  Veja todos os investimentos do cliente.

- **Compra de Ações:**
  Adquira ações para o portfolio do cliente.

- **Compra de Dólares:**
  Adicione dólares ao portfolio do cliente.

- **Valor da Carteira:**
  Acompanhe o valor total dos investimentos.

---

### 🔗 Integração com Backend
A aplicação integra-se com um backend RESTful através da classe Api. O backend deve estar executando em http://127.0.0.1:5000 e oferecer os seguintes endpoints:

- /api/clientes - Gerenciamento de clientes
- /api/clientes/{id}/investimentos - Gerenciamento de investimentos
- /api/clientes/{id}/investimentos/acoes - Compra de ações
- /api/clientes/{id}/investimentos/dolar - Compra de dólares
- /api/clientes/{id}/investimentos/carteira - Valor da carteira
- /api/clientes/{id}/investimentos/agregados - Investimentos agregados

---

### 🎨 Interface Visual
O sistema apresenta duas interfaces principais:

- **Gerente Bancário:** Interface completa para gerenciamento de clientes
- **Concierge de Investimentos:** Interface especializada para gerenciamento de investimentos

- Ambas interfaces seguem um design moderno e responsivo, oferecendo uma experiência de usuário intuitiva e agradável.
