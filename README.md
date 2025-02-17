
# 🚀 Inicializando o Projeto

## 📂 Configuração do Banco de Dados

```bash
create database sistema_tramitacao
```

O arquivo .env está presente no projeto para facilitar a configuração do banco de dados. Certifique-se de ajustar as variáveis conforme necessário antes de rodar o sistema.


## 📥 Clonando o Repositório

Para começar, clone o projeto executando o seguinte comando:

```bash
git clone https://github.com/LucGadelha/frontend-solasstec.git
```


## 📌 Instalando Dependências

1. Acesse o diretório do projeto:

```bash
cd backend-solasstec
```


2. Instale as dependências do projeto:

```bash
npm install
```


## ⚙️ Configurando o Banco de Dados

Após instalar as dependências, execute os seguintes comandos para configurar o banco de dados com Prisma:

```bash
npx prisma db push
npx prisma generate
npx prisma migrate deploy
```

Caso seja necessário carregar dados iniciais de setores e tipos de documentos, execute:

```bash
npm run seed
```

## 🛑 Problema com SSL no Prisma?

Caso ocorra algum erro relacionado a SSL ao rodar os comandos do Prisma, utilize o seguinte comando:

```bash
NODE_TLS_REJECT_UNAUTHORIZED=0 npx prisma generate
```

Isso desativa a verificação de SSL para conexões TLS, permitindo que o Prisma funcione corretamente em ambientes com certificados não confiáveis.


## 🚀 Executando o Projeto

Para iniciar o servidor, utilize um dos seguintes comandos:

```bash
npm run dev
# ou
yarn dev
# ou
pnpm dev
# ou
bun dev
```
