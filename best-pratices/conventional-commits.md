<div align="center">
  <h1 id="conventional-commits">
    <strong>Conventional Commits</strong>
  </h1> 
</div>

## O que são Commits Convencionais?

Commits convencionais são uma convenção para escrever mensagens de commit de maneira padronizada. Essa prática ajuda a entender facilmente as mudanças feitas no código e automatiza a geração de changelogs, versão semântica, e outras tarefas relacionadas ao ciclo de vida do software.
<br><br>

## Seções

- [Estrutura de um Commit Convencional](#estrutura-de-um-commit-convencional)
- [Tipos de Commits Comuns](#tipos-de-commits-comuns)
  - [Exemplos de Commits](#exemplos-de-commits)
  - [Corpo e Rodapé de um Commit](#corpo-e-rodapé-de-um-commit)
- [Padrões de Emojis](#padrões-de-emojis)
- [Exemplos de Commits com Emoji](#exemplos-de-commits-com-emoji)
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

- `feat` - Uma nova funcionalidade para o usuário.
- `fix`- Correção de um bug.
- `docs` - Alterações na documentação.
- `style` - Alterações que não afetam o significado do código (espaços em branco, formatação, etc.).
- `refactor` - Alteração no código que não corrige um bug nem adiciona uma funcionalidade.
- `test` - Adição ou modificação de testes.
- `chore` - Atualização de tarefas de build, pacotes de terceiros, etc.
- `perf` - Melhoria de performance.
- `build` - Mudanças que afetam o sistema de build ou dependências externas (npm, pip, etc.).
- `ci` - Mudanças em arquivos de configuração de integração contínua.
- `raw` - Indicam mudanças relacionadas a arquivos de configurações, dados, features, parametros.
- `cleanup` - Utilizados para remover código comentado, trechos desnecessários ou qualquer outra forma de limpeza do código-fonte, visando aprimorar sua legibilidade e manutenção.

- `remove` - Commits do tipo remove indicam a exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas, reduzindo o tamanho e a complexidade do projeto e mantendo-o mais organizado.
<br>

### Exemplos de Commits
Aqui estão alguns exemplos de mensagens de commit seguindo a convenção:

- `feat(login): add login page`
- `fix(api): resolve issue with timeout on user endpoint`
- `docs(readme): update installation instructions`
- `style(css): format header component`
- `refactor(user-service): simplify user authentication logic`
- `test(cart): add tests for add to cart functionality`
- `chore(deps): update dependencies to latest versions`
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
<br>

## Padrões de Emojis

<table>
  <thead>
    <tr>
      <th>Tipo do commit</th>
      <th>Emoji</th>
      <th>Palavra-chave</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>Acessibilidade</td>
      <td>♿ <code>:wheelchair:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adicionando um teste</td>
      <td>✅ <code>:white_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Atualizando a versão de um submódulo</td>
      <td>⬆️ <code>:arrow_up:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Retrocedendo a versão de um submódulo</td>
      <td>⬇️ <code>:arrow_down:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adicionando uma dependência</td>
      <td>➕ <code>:heavy_plus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Alterações de revisão de código</td>
      <td>👌 <code>:ok_hand:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Animações e transições</td>
      <td>💫 <code>:dizzy:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Bugfix</td>
      <td>🐛 <code>:bug:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Comentários</td>
      <td>💡 <code>:bulb:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Commit inicial</td>
      <td>🎉 <code>:tada:</code></td>
      <td><code>init</code></td>
    </tr>
    <tr>
      <td>Configuração</td>
      <td>🔧 <code>:wrench:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Deploy</td>
      <td>🚀 <code>:rocket:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Documentação</td>
      <td>📚 <code>:books:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Em progresso</td>
      <td>🚧 <code>:construction:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Estilização de interface</td>
      <td>💄 <code>:lipstick:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Infraestrutura</td>
      <td>🧱 <code>:bricks:</code></td>
      <td><code>ci</code></td>
    </tr>
    <tr>
      <td>Lista de ideias (tasks)</td>
      <td>🔜 <code> :soon: </code></td>
      <td></td>
    </tr>
    <tr>
      <td>Mover/Renomear</td>
      <td>🚚 <code>:truck:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Novo recurso</td>
      <td>✨ <code>:sparkles:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Package.json em JS</td>
      <td>📦 <code>:package:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Performance</td>
      <td>⚡ <code>:zap:</code></td>
      <td><code>perf</code></td>
    </tr>
    <tr>
        <td>Refatoração</td>
        <td>♻️ <code>:recycle:</code></td>
        <td><code>refactor</code></td>
    </tr>
    <tr>
      <td>Limpeza de Código</td>
      <td>🧹 <code>:broom:</code></td>
      <td><code>cleanup</code></td>
    </tr>
    <tr>
      <td>Removendo um arquivo</td>
      <td>🗑️ <code>:wastebasket:</code></td>
      <td><code>remove</code></td>
    </tr>
    <tr>
      <td>Removendo uma dependência</td>
      <td>➖ <code>:heavy_minus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Responsividade</td>
      <td>📱 <code>:iphone:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Revertendo mudanças</td>
      <td>💥 <code>:boom:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Segurança</td>
      <td>🔒️ <code>:lock:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>SEO</td>
      <td>🔍️ <code>:mag:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tag de versão</td>
      <td>🔖 <code>:bookmark:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Teste de aprovação</td>
      <td>✔️ <code>:heavy_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Testes</td>
      <td>🧪 <code>:test_tube:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Texto</td>
      <td>📝 <code>:pencil:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tipagem</td>
      <td>🏷️ <code>:label:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tratamento de erros</td>
      <td>🥅 <code>:goal_net:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Dados</td>
      <td>🗃️ <code>:card_file_box:</code></td>
      <td><code>raw</code></td>
    </tr>
  </tbody>
</table>
<br>

## Exemplos de Commits com Emoji

<table>
  <thead>
    <tr>
      <th>Git Command</th>
      <th>Resultado no GitHub</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>git commit -m ":tada: Initial commit"</code>
      </td>
      <td>🎉 Initial commit</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":books: docs: Update README"</code>
      </td>
      <td>📚 docs: Update README</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bug: fix: Infinite loop at line 50"</code>
      </td>
      <td>🐛 fix: Infinite loop at line 50</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":sparkles: feat: Login page"</code>
      </td>
      <td>✨ feat: Login page</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bricks: ci: Modification to Dockerfile"</code>
      </td>
      <td>🧱 ci: Modification to Dockerfile</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":recycle: refactor: Switching to arrow functions"</code>
      </td>
      <td>♻️ refactor: Switching to arrow functions</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":zap: perf: Improvement in response time"</code>
      </td>
      <td>⚡ perf: Improvement in response time</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":boom: fix: Reverting inefficient changes"</code>
      </td>
      <td>💥 fix: Reverting inefficient changes</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":lipstick: feat: CSS styling of the form"</code>
      </td>
      <td>💄 feat: CSS styling of the form</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":test_tube: test: Creating new test"</code>
      </td>
      <td>🧪 test: Creating new test</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bulb: docs: Comments on LoremIpsum() function"</code>
      </td>
      <td>💡 docs: Comments on LoremIpsum() function</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":card_file_box: raw: RAW Data for year yyyy"</code>
      </td>
      <td>🗃️ raw: RAW Data for year yyyy</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":broom: cleanup: Removing commented-out code blocks and unused variables in the form validation function"</code>
      </td>
      <td>🧹 cleanup: Removing commented-out code blocks and unused variables in the form validation function</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":wastebasket: remove: Removing unused files from the project to maintain organization and continuous update"</code>
      </td>
      <td>🗑️ remove: Removing unused files from the project to maintain organization and continuous update</td>
    </tr>
  </tbody>
</table>
