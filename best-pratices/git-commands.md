<div align="center">
  <h1>
    <strong>Git Comands Cheat Sheet</strong>
  </h1> 
</div>

Este documento contém uma lista de comandos Git mais comuns e úteis para facilitar o fluxo de trabalho com Git. Ele é projetado para fornecer uma referência rápida para as operações básicas e avançadas que você pode precisar ao trabalhar com repositórios Git.

## Seções

- **Configuração Inicial**: Comandos para configurar o Git no seu ambiente.
- **Repositório**: Comandos para criar e clonar repositórios.
- **Status e Histórico**: Comandos para verificar o status do repositório e visualizar o histórico de commits.
- **Adicionar e Confirmar Mudanças**: Comandos para adicionar arquivos ao próximo commit e confirmar mudanças.
- **Trabalhando com Branches**: Comandos para criar, trocar e excluir branches.
- **Mesclagem e Rebase**: Comandos para mesclar e rebase branches.
- **Sincronização com o Repositório Remoto**: Comandos para adicionar, enviar e baixar mudanças do repositório remoto.
- **Reversão e Undo**: Comandos para desfazer mudanças e reverter commits.
- **Outros Comandos Úteis**: Comandos adicionais para operações diversas com Git.

## Configuração Inicial

- **Configurar nome de usuário e email**
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"
```
- **Verificar configuração**
```bash
git config --list
```

## Repositório

- **Criar um novo repositório**
```bash
git init
```

- **Clonar um repositório existente**
```bash
git clone <url-do-repositorio>
```

## Status e  Histórico

- **Verificar o status do repositório**
```bash
git status
```

- **Ver o histórico de commits**
```bash
git log
```

- **Ver o histórico de commits com uma linha por commit**
```bash
git log --oneline
```

## Adicionar e Confirmar Mudanças

- **Adicionar arquivos para o próximo commit**
```bash
git add <arquivo> # Adiciona um arquivo expecífico
git add .  # Adiciona todos os arquivos modificados
```

- **Confirmar mudanças (commit)**
```bash
git commit -m "Mensagem do commit"
```

## Trabalhando com Branches

- **Criar uma nova branch e mudar para ela**
```bash
git checkout -b <nome-da-branch>
```

- **Trocar de branch**
```bash
git checkout <nome-da-branch-desejada>
```

- **Listar branches**
```bash
git branch
```

## Mesclagem e Rebase

- **Mesclar uma branch na branch atual**
```bash
git merge <nome-da-branch>
```

- **Rebase a branch atual com outra branch**
```bash
git rebase <nome-da-branch>
```

## Sincronização com o Repositório Remoto (GitHub)

- **Adicionar um repositório remoto**
```bash
git remote add origin <url-do-repositorio>
```

- **Enviar commits para o repositório remoto**
```bash
git push origin <nome-da-branch>
```

- **Baixar mudanças do repositório remoto**
```bash
git pull origin <nome-da-branch>
```

- **Verificar os repositórios remotos configurados**
```bash
git remote -v
```

## Reversão e Undo

- **Desfazer mudanças não confirmadas (restaurar para o último commit)**
```bash
git checkout -- <arquivo>
```

- **Desfazer o último commit (mantendo as mudanças)**
```bash
git reset --soft HEAD~1
```

- **Desfazer o último commit e remover mudanças**
```bash
git reset --hard HEAD~1
```

- **Reverter um commit específico**
```bash
git revert <hash-do-commit>
```

## Outros Comandos Úteis

- **Verificar o que foi alterado em arquivos**
```bash
git diff
```

- **Verificar o que foi alterado em arquivos entre commits**
```bash
git diff <commit1> <commit2>
```

- **Criar uma tag para marcar um ponto específico no histórico**
```bash
git tag <nome-da-tag>
```

- **Listar tags existentes**
```bash
git tag
```