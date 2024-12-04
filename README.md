

# TrackFit - Documentação do Projeto

## Visão Geral do Projeto
O **TrackFit** é um aplicativo de rastreamento de fitness projetado para monitorar a ingestão de calorias e atividades físicas. Este projeto inclui um frontend desenvolvido em React e um backend construído com Flask.

---

## Instruções de Instalação

### 1. Pré-requisitos
- **Node.js**: Instale a versão mais recente a partir do [Site Oficial do Node.js](https://nodejs.org/).
- **Python**: Certifique-se de que o Python 3.8 ou superior está instalado. Baixe em [Site Oficial do Python](https://www.python.org/).
- **Git**: Opcional, mas recomendado para controle de versão.
- **Banco de Dados**: SQLite (incluído no Python) ou MySQL.

---

### 2. Configurando o Backend
1. Navegue até o diretório `TrackFit/backend`:
   ```bash
   cd TrackFit/backend
   ```
2. Crie e ative um ambiente virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   ```
3. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```
4. Configure o banco de dados:
   - Crie o banco de dados usando o arquivo `schemas.sql` localizado em `TrackFit/database`:
     ```bash
     sqlite3 database.db < ../database/schemas.sql
     ```
   - Ou importe o esquema no seu banco MySQL, caso esteja utilizando MySQL.

5. Inicie o servidor backend:
   ```bash
   flask run
   ```
   - Acesse o backend em [http://127.0.0.1:5000](http://127.0.0.1:5000).

---

### 3. Configurando o Frontend
1. Navegue até o diretório `TrackFit/frontend`:
   ```bash
   cd TrackFit/frontend
   ```
2. Instale as dependências necessárias para o Node.js:
   ```bash
   npm install
   ```
3. Inicie o servidor de desenvolvimento do frontend:
   ```bash
   npm start
   ```
   - O aplicativo estará acessível em [http://localhost:3000](http://localhost:3000).

---

## Testando o Aplicativo
1. Abra o frontend no navegador ([http://localhost:3000](http://localhost:3000)).
2. Cadastre-se e faça login como um novo usuário.
3. Use o painel para rastrear calorias, definir metas e monitorar atividades.

---

## Solução de Problemas
- **Problemas no Backend**: Certifique-se de que o ambiente virtual está ativado e todas as dependências estão instaladas corretamente.
- **Problemas no Frontend**: Apague a pasta `node_modules` e execute `npm install` novamente.
- **Problemas no Banco de Dados**: Verifique a conexão com o banco de dados e certifique-se de que o esquema foi carregado corretamente.

---

## Notas Adicionais
- Este projeto utiliza Flask para APIs no backend e React para a interface do usuário no frontend.
- Melhorias futuras incluem suporte para aplicativos móveis e integração com dispositivos vestíveis (wearables).
