# Como contribuir

Este repositório é mantido em grupo. Para manter o histórico organizado e evitar
retrabalho, siga o fluxo abaixo em toda contribuição (documentação ou código).

## 1. Nunca commitar direto na `main`

A branch `main` só recebe alterações por meio de Pull Request revisado por
outra pessoa do grupo. Nenhum push direto é permitido.

## 2. Fluxo de branch

1. Atualize sua `main` local:
   ```shell
   git checkout main
   git pull origin main
   ```
2. Crie uma branch a partir da `main`, com um nome curto e descritivo do que
   será feito, por exemplo:
   - `docs/participacoes-base`
   - `docs/modelagem-bpmn`
   - `fix/link-sidebar`
3. Trabalhe e commite na sua branch.
4. Antes de abrir o Pull Request (ou se ele demorar para ser revisado),
   atualize sua branch com a `main` para evitar conflitos:
   ```shell
   git fetch origin
   git merge origin/main
   ```
5. Envie a branch para o repositório remoto:
   ```shell
   git push -u origin nome-da-sua-branch
   ```
6. Abra um Pull Request para a `main` explicando o que foi feito.
7. Aguarde a aprovação de pelo menos uma outra pessoa do grupo antes do merge.

## 3. Mensagens de commit

- Todas as mensagens de commit devem ser escritas em português.
- Prefira mensagens curtas e diretas, no imperativo, descrevendo o que a
  alteração faz, por exemplo:
  - `Adiciona tabela de integrantes`
  - `Corrige link quebrado no sidebar`
  - `Atualiza seção de participações da base`

## 4. Identidade nos commits

Cada commit deve ficar atrelado à conta GitHub de quem efetivamente realizou
a contribuição. Confira se `git config user.name` e `git config user.email`
correspondem à sua conta antes de commitar.

## 5. Estrutura de documentação

A documentação segue o template oficial da disciplina, organizada em
`docs/Base` e `docs/Projeto`. Não omita seções exigidas pelo template; se uma
seção ainda não tiver conteúdo, deixe um placeholder claro indicando que está
pendente, em vez de removê-la.

## 6. Legenda das imagens

Toda imagem de engenharia reversa (print de tela, diagrama, print de
ferramenta) deve ter uma legenda logo abaixo, no seguinte formato:

```html
<p align="center">
  <img src="Base/Assets/SubEquipe_0X/nome-do-arquivo.png" alt="Descrição da imagem" width="600">
</p>
<p align="center"><b>Figura N</b> — Descrição breve do que a imagem mostra.<br>
<b>Fonte:</b> origem da imagem (site, ferramenta, "Elaborado pela SubEquipe 0X", etc.).</p>
```

- O caminho da imagem em `src` deve ser relativo à raiz de `docs/` (ex.:
  `Base/Assets/SubEquipe_03/arquivo.png`), sem `./` nem `../` no início.
  Isso é necessário por causa do roteamento por hash do docsify: um `<img>`
  em HTML puro é resolvido a partir da raiz, não da pasta do arquivo
  `.md`. Sintaxe `![]()` de markdown segue outra regra (relativa ao
  arquivo) e não deve ser usada para imagens de engenharia reversa, para
  evitar essa inconsistência.
- A numeração das Figuras é **sequencial pelo documento inteiro**,
  seguindo a ordem em que as imagens aparecem no arquivo (não reinicia por
  seção nem por autor). Antes de adicionar uma imagem nova, confira qual é
  a última Figura já numerada no arquivo e continue a partir dela. Se você
  inserir uma imagem antes de figuras já numeradas, renumere as
  seguintes.
