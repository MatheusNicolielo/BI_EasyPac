# Git Easypac - Novo Portal
-- -
- Curso: https://www.youtube.com/watch?v=ts-H3W1uLMM
- Recomendado Utilizar uma interface para controle, como:
    - Sourcetree
>
## Fluxo Base
Diretório Local -> Stage -> Diretório Git
## Fluxo Uso
1. No Diretório Local criar uma nova Branch (git checkout)
1. Realizar os devidos ajustes
1. Adicionar na área de Staging (git add)
1. Realizar um commit no repositório local (git commit)
1. Enviar este commit para o repositório remoto (git push)
1. Criar um Merge Request para juntar suas alterações com a branch develop
1. Após o processo do MR, atualizar sua branch develop do repositório local (git pull)
## Nome\MSG Commit
1. <b>Task</b> -> Código completo da Task (#30580)
1. <b>Local do Ajuste</b> -> Onde realizou os ajustes no BI ou demais arquivos:
   1. Geral;
   2. Visual;
   3. Medidas;
    1. Query;
    1. Outro, especificar (Ex. Outro_ExcelRegional)
1. <b>Descrição</b> -> Pequena descrição para detalhar o que foi realizado e facilitar a busca por onde validar, testar, etc.

<b>Ex :  #30888-Geral-Adicionado Data Inicio e Recebimento e Alterado Último Acesso</b>
## Branchs
- <b>main</b> -> branch em produção
- <b>develop</b> -> branch final em desenv
- <b>branch_tasks</b> -> branch criada para cada task
## Tag's
Utilizado para marcar um ponto específico, bom para quando for lançar versão, etc.
## Boas Práticas
1. Nunca fazer alterações direto na main ou develop;
1. Caso ocorrer, migrá-las para uma nova branch.
1. Sempre criar uma nova branch para realizar as alterações, idealmente com o nome do número da task;
1. Tomar cuidado com indexação ou formatação de código.
1. Não guardar arquivos binários no projeto (PDF, Imagens, etc.)
   1. Uma alternativa que não pesa o projeto é colocar a imagem em algum link externo e por meio de um Markdown File mostra-la.
   2. <b>.gitignore</b>
1. Commits devem possuir poucas mudanças, em geral. Ou seja: commite constantemente
1. Manter readme ou outro arquivo .md com a versão, regras, etc.
1. Preferencialmente não aprove seu Merge Request

