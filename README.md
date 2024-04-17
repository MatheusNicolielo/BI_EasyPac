# Git Easypac - Novo Portal
-- -
- Curso: https://www.youtube.com/watch?v=ts-H3W1uLMM
- Recomendado Utilizar uma interface para controle, como:
    - Sourcetree
- Sempre criar uma <b>branch</b> nova para cada Task;
- Configurar nome e email para o commit;
- Tomar cuidado com indexação do código
- Nunca fazer alterações direto na <b>master</b> ou <b>develop</b>
## Fluxo Base
Diretório Local -> Stage -> Diretório Git
## Fluxo Uso
1. No Diretório Local criar uma nova branch
2. Realizar os Ajustes
3. Adicionar tudo na área de Stage
4. Realizar um commit na branch utilizada
## Nome Commit
*Task*-*Tipo*-*OndeFeito*-*Descrição*
ex: #25533-Funcionalidade-Geral-Alterando Painel Ociosidade
- *Task* -> Número da Task
- *Tipo* -> Foco Principal, sendo:
  - Refatoracao
  - Bug
  - Funcionalidade
- *OndeFeito* -> Onde foi feito os ajustes da task
    Caso queira especificar o local _
  - Geral
  - Visual
  - Medidas
  - Query
  - Outro : Usar _ para especificar (ex: Excel_ArquivoRegional)
- *Descrição* -> Pequena descrição do que realizou
## Branchs
- <b>master</b> -> branch em produção
- <b>develop</b> -> branch final em desenv
- <b>branch_tasks</b> -> branch criada para cada task
## Tag's
Utilizado para marcar um ponto específico, bom para quando for lançar versão, etc.
## Comando Básicos
### git add
    Adiciona os arquivos ao Stage
    - Modos de utilizar:
      - *git add .* -> adiciona todos os arquivos ao Stage
      - *git add index.html* -> adiciona somente o(s) arquivos listados na área de Stage
      - *git add .css* -> adiciona todos da extesão X para a área de Stage
### git status
    Mostra o Status dos arquivos atuais da branch, o que foi modificado, o que subiu ao stage, etc.
### git reset
    Tira mudanças do Stage sem alterar mudanças realizadas na área de trabalho
    - É possivel utilizar também para voltar commit's e HEAD
### git restore
    -> Reverte uma mudança que já subiu para o Stage, commit ou HEAD
### git diff
    Diferença do Stage para o arquivo modificado
### git commit
    Confirma as mudanças, cria uma 'foto' do código no momento do commit
    *-m* -> Título
    *-a* -> Faz o commit sem passar pelo Stage (Não é muito ideal)
    *-amend* -> Mudar o último commit (Último Caso)
### git log
    Status geral da Branch
    - *-x* -> x numero de logs que deseja ver, a partir do último
    - *graph*
    - *--author*
### git shortlog
    Versão otimizada do log
### git reflog
    Mudanças realizadas no repositório
### git checkout
    Troca para a Branch especificada
### git merge
    Move as alterações de Branch's
    Quando da conflito:
        *--abort*
        *--continue*
### git stash
    Cria uma 'branch' temporária com as mudanças feitas
    *pop* aplica as mudanças no stash na branch desejada






