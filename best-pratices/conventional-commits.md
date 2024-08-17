<div align="center">
  <h1 id="conventional-commits">
    <strong>Conventional Commits</strong>
  </h1> 
</div>

## O que são Commits Convencionais?

Commits convencionais são uma convenção para escrever mensagens de commit de maneira padronizada. Essa prática ajuda a entender facilmente as mudanças feitas no código e automatiza a geração de changelogs, versão semântica, e outras tarefas relacionadas ao ciclo de vida do software.
<br>

## Estrutura de um Commit Convencional

A mensagem de commit convencional segue este formato:

```plaintext
<tipo>(<escopo opcional>): <descrição curta>

[corpo opcional]
[rodapé opcional]
```

- **Tipo**: Descreve a categoria das mudanças feitas no código.
- **Escopo**: Um escopo opcional que especifica a parte do projeto que foi afetada.
- **Descrição**: Uma breve descrição das mudanças (no máximo 50 caracteres).
- **Corpo (opcional)**: Explicação detalhada das mudanças, razões e impactos.
- **Rodapé (opcional)**: Usado para referências de issues, breaking changes, ou outras informações adicionais.
<br>

## Tipos de Commits Comuns

Aqui estão alguns tipos de commit frequentemente usados:

- **feat:** Uma nova funcionalidade para o usuário.
- **fix:** Correção de um bug.
- **docs:** Alterações na documentação.
- **style:** Alterações que não afetam o significado do código (espaços em branco, formatação, etc.).
- **refactor:** Alteração no código que não corrige um bug nem adiciona uma funcionalidade.
- **test:** Adição ou modificação de testes.
- **chore:** Atualização de tarefas de build, pacotes de terceiros, etc.
- **perf:** Melhoria de performance.
- **build:** Mudanças que afetam o sistema de build ou dependências externas (npm, pip, etc.).
- **ci:** Mudanças em arquivos de configuração de integração contínua.
<br>

### Exemplos de Commits
Aqui estão alguns exemplos de mensagens de commit seguindo a convenção:

- **feat(login)**: add login page
- **fix(api)**: resolve issue with timeout on user endpoint
- **docs(readme)**: update installation instructions
- **style(css)**: format header component
- **refactor(user-service)**: simplify user authentication logic
- **test(cart)**: add tests for add to cart functionality
- **chore(deps)**: update dependencies to latest versions
<br>

### Corpo e Rodapé de um Commit
O corpo e o rodapé de um commit são opcionais, mas úteis em alguns casos:

- **Corpo:** se necessário, pode ser incluido um corpo com detalhes adicionais:

```plaintext
fix(auth): resolve incorrect password validation

The password validation was not properly handling edge cases where the
user input contained special characters. Updated the regex to match
the correct criteria.
```

- **Rodapé:** para referências de issues ou breaking changes:

```plaintext
feat(api): add support for new payment method

BREAKING CHANGE: The payment API has been updated to handle new payment
method tokens. The old method of payment has been deprecated and will be
removed in the next major release.

Closes #123
```