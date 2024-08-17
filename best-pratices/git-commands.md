<div align="center">
  <h1>
    <strong>Git Comands Cheat Sheet</strong>
  </h1> 
</div>

Este documento contém uma lista de comandos Git mais comuns e úteis para facilitar o fluxo de trabalho com Git. Ele é projetado para fornecer uma referência rápida para as operações básicas e avançadas que você pode precisar ao trabalhar com repositórios Git.

## Seções

- [Configuração Inicial](#configuração-inicial): Comandos para configurar o Git no seu ambiente.
- [Repositório](#repositório): Comandos para criar e clonar repositórios.
- [Status e Histórico](#status-e-histórico): Comandos para verificar o status do repositório e visualizar o histórico de commits.
- [Adicionar e Confirmar Mudanças](#adicionar-e-confirmar-mudanças): Comandos para adicionar arquivos ao próximo commit e confirmar mudanças.
- [Trabalhando com Branches](#trabalhando-com-branches): Comandos para criar, trocar e excluir branches.
- [Mesclagem e Rebase](#mesclagem-e-rebase): Comandos para mesclar e rebase branches.
- [Sincronização com o Repositório Remoto](#sincronização-com-o-repositório-remoto): Comandos para adicionar, enviar e baixar mudanças do repositório remoto.
- [Reversão e Undo](#reversão-e-undo): Comandos para desfazer mudanças e reverter commits.
- [Outros Comandos Úteis](#outros-comandos-úteis): Comandos adicionais para operações diversas com Git.

## Configuração Inicial

- **Configurar nome de usuário e email**
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"
```
<br><br>
- **Verificar configuração**
```bash
git config --list
```
<br><br>

## Repositório

- **Criar um novo repositório**
```bash
git init
```
<br><br>

- **Clonar um repositório existente**
```bash
git clone <url-do-repositorio>
```
<br><br>

## Status e  Histórico

- **Verificar o status do repositório**
```bash
git status
```
<br><br>

- **Ver o histórico de commits**
```bash
git log
```
<br><br>

- **Ver o histórico de commits com uma linha por commit**
```bash
git log --oneline
```
<br><br>

## Adicionar e Confirmar Mudanças

- **Adicionar arquivos para o próximo commit**
```bash
git add <arquivo> # Adiciona um arquivo expecífico
git add .  # Adiciona todos os arquivos modificados
```
<br><br>

- **Confirmar mudanças (commit)**
```bash
git commit -m "Mensagem do commit"
```
<br><br>

## Trabalhando com Branches

- **Criar uma nova branch e mudar para ela**
```bash
git checkout -b <nome-da-branch>
```
<br><br>

- **Trocar de branch**
```bash
git checkout <nome-da-branch-desejada>
```
<br><br>

- **Listar branches**
```bash
git branch
```
<br><br>

## Mesclagem e Rebase

- **Mesclar uma branch na branch atual**
```bash
git m
erge <nome-da-branch>
```
<br><br>

- **Rebase a branch atual com outra branch**
```bash
git rebase <nome-da-branch>
```
<br><br>

## Sincronização com o Repositório Remoto (GitHub)

- **Adicionar um repositório remoto**
```bash
git remote add origin <url-do-repositorio>
```
<br><br>

- **Enviar commits para o repositório remoto**
```bash
git push origin <nome-da-branch>
```
<br><br>

- **Baixar mudanças do repositório remoto**
```bash
git pull origin <nome-da-branch>
```
<br><br>

- **Verificar os repositórios remotos configurados**
```bash
git remote -v
```
<br><br>

## Reversão e Undo

- **Desfazer mudanças não confirmadas (restaurar para o último commit)**
```bash
git checkout -- <arquivo>
```
<br><br>

- **Desfazer o último commit (mantendo as mudanças)**
```bash
git reset --soft HEAD~1
```
<br><br>

- **Desfazer o último commit e remover mudanças**
```bash
git reset --hard HEAD~1
```
<br><br>

- **Reverter um commit específico**
```bash
git revert <hash-do-commit>
```
<br><br>

## Outros Comandos Úteis

- **Verificar o que foi alterado em arquivos**
```bash
git diff
```
<br><br>

- **Verificar o que foi alterado em arquivos entre commits**
```bash
git diff <commit1> <commit2>
```
<br><br>

- **Criar uma tag para marcar um ponto específico no histórico**
```bash
git tag <nome-da-tag>
```
<br><br>

- **Listar tags existentes**
```bash
git tag
```
<br><br>