## Caderno de anotações do Matheus

# Vamos anotar as observações importantes sobre esse curso aqui. Aqui estará de forma que o Matheus do presente (momento em que ele estuda esse material) é capaz de se comunicar com o Matheus do futuro (qualquer Matheus no futuro dessa mesma linha temporal).

- TO DO: Colocar esse arquivo no .gitignore para garantir que apenas eu veja ele no futuro próximo
- Objetivo secundário: Aprender a escrever em MarkDown para facilitar o processo de aprendizagem.
- Primeira parte do processo foi executar um comando npm init para dar criação ao package.json
- Após isso também foi necessário executar o comando json-server --watch backend/videos.json para inicializar o json-server
- Após instalar o ESLint usando o comando npm init @eslint/config@0.4.6 é interessante seguir o passo a passo lendo o que ele está perguntando para não ir na empolgação e cancelar funções que são fundamentais para a aplicação.
- É interessante criar um gitignore para não subir uma tralha de arquivos para o github de modo desnecessário.
- Para rodar o ESLint o comando é `npx eslint <nome do arquivo a ser testado>`;
- Para rodar o ESlint em todos os arquivos é o comando `npx eslint .`;
- Existe uma extensão do VSCode para rodar o ESLint de forma nativa e automática. Isso facilita e evita erros manuais (execução mecânica) no projeto. O nome da extensão é: ESLint

## Pacotes locais e globais

- Quando estamos falando de pacotes e dependências sempre virá aquela clássica pergunta. Eu vou precisar disso aqui para todos os projetos ou APENAS para esse? Quando for algo global, durante a instalação do pacote, iremos usar o --global (-g) no comando. Quando fizermos isso, basta só dar o comando como se ele fosse algo específico do SO. Do contrário iremos ter que usar a sintaxe `npx <pacote> <demais argumentos>` pois ele irá ficar apenas local
- E se eu precisar instalar algo das dependências?? Basta confirmar que no package.json o pacote está ausente e você consegue usar o comando `npm install`. Ele irá procurar naquela lista os não instalados e os instalados (mesmo fora da versão escolhida para rodar) e atualizar no segundo caso necessário.

## Número de Versão

- No exemplo citado pelo instrutor, ele cita uma diferença na hora de escolher o versionamento.

Trecho retirado da Alura:

    "
    O número mais à direita, na versão 7.0.0, por exemplo, representa uma atualização de correção. Isso significa que, quando esse número da direita muda, a equipe provavelmente lançou uma nova atualização da ferramenta corrigindo algum bug, chamada em inglês de patch version.

    O número do meio é a versão menor. Geralmente, ela traz novos recursos quando atualizada, além de poder corrigir bugs, mas sempre trazendo novidades.

    O número da esquerda é a versão maior do projeto. Quando esse número muda, a equipe do pacote pode descontinuar recursos antigos ou modificar recursos existentes. Então, uma mudança nesse número maior requer atenção, pois talvez seja necessário consultar um guia de migração, que normalmente é disponibilizado pela equipe, indicando mudanças necessárias na sintaxe ou em outros códigos, ou algum comando pode não existir mais na nova versão.

    Observando como funcionam essas atualizações, quando o número do meio muda, ele sempre reseta o número da direita para 0. Por exemplo, observe a versão 7.3.1. Quando foi para 7.4.0, a versão de correção que estava 1 volta a ser 0. É uma regra que devemos seguir.

    Da mesma forma, ao mudar da versão 7 para 8, todos os números à direita voltam a ser 0. Podemos conferir isso no histórico. Da versão 7.32.0 para a versão 8.0.0, resetou para 0. Isso é o que chamamos de versionamento semântico, uma convenção muito utilizada no mundo do desenvolvimento web, seja no front-end ou no back-end.
    "

- Leitura recomendada: https://www.alura.com.br/artigos/versionamento-semantico-breve-introducao
