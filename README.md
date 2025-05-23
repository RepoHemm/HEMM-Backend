# 🏥 HEMM - Backend

Este repositório contém o backend do projeto HEMM (Hospital Equipment Maintenance Management), desenvolvido em **NestJS**, **TypeScript** e **Prisma**.

## Sumário

- [Pré-requisitos](#pré-requisitos)
- [Clonando o repositório](#clonando-o-repositório)
- [Configurando o ambiente](#configurando-o-ambiente)
- [Fluxo de trabalho](#fluxo-de-trabalho)
  - [Como atualizar seu fork](#como-atualizar-seu-fork)
  - [Como criar uma branch](#como-criar-uma-branch)
  - [Como fazer commits](#como-fazer-commits)
  - [Como enviar suas alterações (push)](#como-enviar-suas-alterações-push)
  - [Como abrir um Pull Request](#como-abrir-um-pull-request)

---

## Pré-requisitos

- Node.js (versão >= 18.x)
- npm ou yarn
- MySQL
- Git
- NestJS CLI

---

## Clonando o repositório

1. Faça um fork deste repositório para a sua conta no GitHub.
2. Clone o seu fork localmente:

```bash
git clone https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
```

3. Entre na pasta do projeto:

```bash
cd NOME_DO_REPOSITORIO
```

4. Instale as dependências:

```bash
npm install
```

---

## Configurando o ambiente

1. Configure o arquivo `.env` com as variáveis de ambiente necessárias, como a URL do banco de dados.
2. Gere o cliente Prisma:

```bash
npx prisma generate
```

3. Execute as migrações (se necessário):

```bash
npx prisma migrate dev
```

4. Rode a aplicação:

```bash
npm run start:dev
```

---

## Fluxo de trabalho

### ✅ Como atualizar seu fork

1. **Adicione o repositório original como `upstream`:**

```bash
git remote add upstream https://github.com/ORIGINAL_OWNER/NOME_DO_REPOSITORIO.git
```

2. **Busque as alterações do repositório original:**

```bash
git fetch upstream
```

3. **Atualize sua branch local `develop`:**

```bash
git checkout develop
git merge upstream/develop
```

4. **Envie para o seu fork:**

```bash
git push origin develop
```

---

### Como criar uma branch

Sempre trabalhe em uma branch nova baseada na `develop`:

```bash
git checkout develop
git pull origin develop
git checkout -b nome-da-feature
```

---

### Como fazer commits

1. Adicione os arquivos modificados:

```bash
git add .
```

2. Faça um commit claro e descritivo:

```bash
git commit -m "feat: descrição da funcionalidade"
```

**Padrão de commit:**

- `feat:` Nova funcionalidade
- `fix:` Correção de bug
- `docs:` Alteração na documentação
- `refactor:` Refatoração de código
- `test:` Adição ou alteração de testes

---

### Como enviar suas alterações (push)

```bash
git push origin nome-da-feature
```

---

### Como abrir um Pull Request

1. Acesse o seu fork no GitHub.
2. Clique em **"Compare & pull request"**.
3. Preencha o título e descrição explicando o que foi feito.
4. Selecione `develop` como branch base.
5. Aguarde revisão e aprovação.

---

### Contato equipe Hemm
Email: hemmmanager@gmail.com
