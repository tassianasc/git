# **Configurando o Git no VSCode para GitHub**

Bem-vindo ao guia de **configuração do Git no VSCode** para integração com o **GitHub**. Siga estas etapas para criar e gerenciar repositórios no GitHub diretamente do VSCode.

---

## **Sumário**

1. [Visão Geral](#visão-geral)
2. [Requisitos](#requisitos)
3. [Configuração do Ambiente](#configuração-do-ambiente)
   - [Criar um Repositório no GitHub](#1-criar-um-repositório-no-github)
   - [Instalar e Configurar o Git no VSCode](#2-instalar-e-configurar-o-git-no-vscode)
   - [Escolher Git Bash no Terminal do VSCode](#3-escolher-git-bash-no-terminal-do-vscode)
4. [Inicialização do Repositório](#inicialização-do-repositório)
   - [Configurar Usuário e E-mail](#4-configurar-usuário-e-email)
   - [Inicializar o Repositório Git](#5-inicializar-o-repositório-git)
5. [Enviando o Código para o GitHub](#enviando-o-código-para-o-github)
   - [Conectar ao Repositório Remoto](#6-conectar-ao-repositório-remoto)
   - [Adicionar Arquivos ao Repositório](#7-adicionar-arquivos-ao-repositório)
   - [Realizar um Commit](#8-realizar-um-commit)
   - [Renomear a Branch Principal](#9-renomear-a-branch-principal)
   - [Enviar para o Repositório Remoto](#10-enviar-para-o-repositório-remoto)
6. [Adicionando Mudanças Posteriormente](#adicionando-mudanças-posteriormente)
   - [Verificar o status dos arquivos](#verificar-o-status-dos-arquivos)
   - [Adicionar apenas os arquivos modificados](#adicionar-apenas-os-arquivos-modificados)
   - [Realizar um Commit das Mudanças](#realizar-um-commit-das-mudanças)
   - [Enviar as Mudanças para o GitHub](#enviar-as-mudanças-para-o-github)
7. [Notas Finais](#notas-finais)

---

## **Visão Geral**

Este guia abrange os passos necessários para:

- Criar um repositório no **GitHub**.
- Configurar o **Git** no **VSCode**.
- Usar o **Git Bash** no terminal do VSCode.
- Executar comandos **Git** para inicializar, adicionar, commitar e enviar código para o **GitHub**.

---

## **Requisitos**

- **VSCode**
- **Git**
- **Conta no GitHub**

---

## **Configuração do Ambiente**

### **1. Criar um Repositório no GitHub**

1. Acesse o **GitHub** e faça login.
2. Clique no botão **"New"** para criar um novo repositório.
3. Dê um nome ao repositório, adicione uma descrição (opcional) e defina se será **público** ou **privado**.
4. Clique em **"Create repository"**.

---

### **2. Instalar e Configurar o Git no VSCode**

1. Verifique se o **Git** está instalado:

   ```bash
   git --version
Se não estiver instalado, siga as instruções no site do Git.

3. Escolher Git Bash no Terminal do VSCode
Abra o VSCode.
No menu superior, selecione "Terminal" > "New Terminal".
No terminal aberto, clique no ícone de seleção de terminal e escolha "Git Bash".
Inicialização do Repositório
4. Configurar Usuário e E-mail
Configure seu usuário e e-mail no Git:

bash
Copiar código
git config --global user.email "seuemail@exemplo.com"
git config --global user.name "seuNomeNoGitHub"
Verifique se as configurações estão corretas:

bash
Copiar código
git config user.name
git config user.email
5. Inicializar o Repositório Git
Dentro da pasta do seu projeto, inicialize o repositório:

bash
Copiar código
git init
Enviando o Código para o GitHub
6. Conectar ao Repositório Remoto
Adicione o repositório remoto do GitHub:

bash
Copiar código
git remote add origin https://github.com/seuUsuario/seuRepositorio.git
7. Adicionar Arquivos ao Repositório
Adicione os arquivos ao estágio de commit:

bash
Copiar código
git add .
Dica: O comando git add . adiciona todos os arquivos e alterações no diretório atual ao estágio para commit.

8. Realizar um Commit
Realize o commit das alterações:

bash
Copiar código
git commit -m "Primeira versão"
Nota: git commit -m "mensagem" cria um ponto de salvamento no histórico do Git, com a mensagem explicando as mudanças.

9. Renomear a Branch Principal
Renomeie a branch principal para "main":

bash
Copiar código
git branch -M main
10. Enviar para o Repositório Remoto
Envie suas mudanças para o GitHub:

bash
Copiar código
git push -u origin main
Autorização: Se solicitado, faça login no GitHub e autorize o Git a usar sua conta.

Adicionando Mudanças Posteriormente
Verificar o status dos arquivos
Para ver quais arquivos foram modificados:

bash
Copiar código
git status
Adicionar apenas os arquivos modificados
Adicione os arquivos modificados:

bash
Copiar código
git add nome_do_arquivo
Realizar um Commit das Mudanças
Comite as mudanças:

bash
Copiar código
git commit -m "Descrição das mudanças"
Enviar as Mudanças para o GitHub
Envie as mudanças:

bash
Copiar código
git push
Notas Finais
Este guia cobre as etapas essenciais para configurar e usar o Git no VSCode com o GitHub. Certifique-se de manter suas credenciais seguras e de revisar suas configurações de usuário antes de iniciar o uso do Git.

Se precisar de mais ajuda, consulte a documentação do Git e do VSCode:

Documentação do Git
Documentação do VSCode
csharp
Copiar código
