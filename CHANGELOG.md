# Changelog

Todas as alterações relevantes deste produto são registadas neste ficheiro.

O formato segue o Keep a Changelog e as versões seguem SemVer.

## Não publicado

## 0.2.0 - 2026-08-29

### Adicionado

- Foi adicionado um assistente de configuração que descobre projetos Taskmark na pasta escolhida, valida o quadro e guarda o projeto ativo.
- Foi adicionada uma barra de aplicação com a marca Taskmark e troca rápida entre projetos.
- Foram adicionadas listas de épicos, histórias, tarefas e bugs lidas diretamente do markdown local.
- Foi adicionado um painel de detalhe para qualquer item, com markdown formatado, datas legíveis, navegação para trás e ligação direta por URL.
- Passou a ser possível ver diagramas Mermaid desenhados no detalhe do item, em vez do bloco de código.
- Foi adicionada a vista Work items, com tabela única de todo o trabalho, etiquetas de épico e história, barras de progresso e pontos visíveis ao passar sobre o tamanho.
- Foram adicionadas paginação, pesquisa, ordenação por coluna, filtro de período, filtro por épico ou história, filtro por etiquetas e a opção de esconder trabalho concluído.
- Passou a ser possível ter tarefas e bugs diretamente num épico, sem história intermédia.
- Foi adicionada a identidade de quem cria e resolve trabalho, com iniciais em avatar nas listas e autor nos registos de atividade.
- Foi adicionado um painel de métricas com a contagem total e concluída de itens e a lista de contribuidores do projeto.
- O quadro passou a abrir com um único comando: `npx taskmark serve` dentro da pasta do quadro, ou `npx @taskmark/ui` para escolher o projeto.
- Foram adicionados os comandos `/tkmd-init`, `/tkmd-plan`, `/tkmd-save`, `/tkmd-plan-do`, `/tkmd-do`, `/tkmd-shelf` e `/tkmd-commit` no Cursor, sendo o último o único que faz commit.
- Foi adicionado o estado arquivado, para fechar trabalho que nunca será implementado sem o dar como feito, com aspeto próprio e escondido junto com o concluído.
- Foram adicionados os comandos `/tkmd-changelog` e `/tkmd-version`, que escrevem as notas de alterações em `CHANGELOG.md` e a versão no `package.json` do quadro, sem fazer commit nem publicar.
- Foi criado o site do Taskmark, com página inicial, demonstração em consola, secções de funcionalidades, motivação e contribuição, formulário de contacto e seletor de tema claro ou escuro.
- Foi publicada a documentação do produto, com instalação, referência de comandos, estrutura de pastas, especificação dos ficheiros, tamanhos e fluxos de trabalho.
- Foram adicionados favicons, imagens de partilha e metadados de SEO no site e no quadro local.

### Alterado

- A vista Overall passou a ser uma árvore hierárquica expansível, em vez de tabelas empilhadas, com ordenação por incompletos e mais recentes, pesquisa que mantém o contexto dos pais, atalhos de teclado, suporte para leitores de ecrã e expansão preservada durante a sessão.
- O quadro passou a viver em `<projeto>/taskmark/` quando há um só repositório, ou num repositório dedicado `<comum>-taskmark` quando há vários, deixando de ser copiado para dentro de cada projeto.
- Os tamanhos passaram a ser fixos, de XS a XXL, com pontos previsíveis, em vez de estimativas calculadas a partir de velocidade.
- O tempo real passou a ser somado a partir dos intervalos fechados do registo de trabalho, sem estimativa nem responsável atribuído.
- As alterações passaram a ser escritas apenas nos ficheiros de tarefa ou bug; o estado, as pessoas, os registos e as datas dos épicos e histórias passaram a ser calculados na leitura, o que evita conflitos quando várias pessoas trabalham ao mesmo tempo.
- Os identificadores de trabalho passaram a incluir o tipo e a identidade de quem cria, deixando de depender de um contador global partilhado.

### Removido

- Foram removidos os ficheiros gerados `INDEX.md`, `SIZING.md`, `VELOCITY.md` e o README do quadro, incluindo o registo de alterações que era mantido nesse README.
- Foram removidas a velocidade, a calibração de estimativas, as previsões de conclusão e o campo de responsável.
- O ficheiro `REPOS.md` deixou de ser versionado e passou a ser gerado localmente.
- Foram removidos os comandos, scripts e regras do plugin que já não eram utilizados.

### Corrigido

- A configuração inicial deixou de falhar a descobrir quadros de vários repositórios guardados numa pasta única.
- A lista de épicos deixou de falhar quando o cabeçalho de um ficheiro do quadro estava malformado.
- O repositório dedicado do quadro deixou de criar uma pasta `taskmark/` desnecessária.
- O logótipo deixou de ficar colado ao limite inferior da barra de aplicação.
- O tempo real do épico deixou de ser inflacionado quando várias tarefas partilhavam a mesma sessão de trabalho.
- O detalhe deixou de mostrar o item errado quando outro projeto tinha um identificador igual.
- O quadro deixou de rebentar ao abrir o detalhe de um item em certas navegações.
- As tarefas e bugs deixaram de precisar de uma história para poderem pertencer a um épico.
- Esconder concluídos deixou de esconder épicos que ainda tinham trabalho por fazer.
- O comando `npx taskmark` deixou de executar um pacote sem relação e passou a abrir sempre o quadro.
- O quadro passou a ser servido na raiz, sem ciclos de redirecionamento.
- A geração estática do quadro deixou de falhar por causa de caminhos abreviados, de configuração de build incompatível e de ficheiros de build antigos, e deixou de emitir avisos de CSS.
- O quadro alojado no Vercel deixou de falhar por a interface estar declarada como dependência de desenvolvimento.
- Os nomes com acentos deixaram de gerar identidades erradas nos identificadores de trabalho.
