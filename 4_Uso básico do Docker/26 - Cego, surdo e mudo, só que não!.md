# 25 - Reutilizar containers

Nesta aula, será abordado como reutilizar contêineres previamente criados em vez de criar novos do zero. Essa prática economiza tempo e recursos, permitindo que você use contêineres existentes quando necessário.

Primeiro, o console será limpo para começar com um ambiente limpo. Para verificar os contêineres que estão atualmente em execução, utiliza-se o comando docker ps. Esse comando lista todos os contêineres em execução no momento.

Para listar os arquivos no diretório atual de um contêiner, é utilizado o comando ls. Isso é semelhante ao comando ls em sistemas Unix. O seguinte comando é executado:

``` docker exec -it meu-container ls ```

Aqui, docker exec é usado para executar o comando ls dentro do contêiner chamado "meu-container". Isso resultará na listagem dos arquivos no diretório atual dentro do contêiner.

Em seguida, é possível acessar interativamente o contêiner usando o comando docker exec. Eis o comando:

``` docker exec -it meu-container bash ```

Esse comando concede acesso ao terminal interno do contêiner, de modo semelhante a executar bash no modo interativo.

Uma vez dentro do contêiner, é possível criar um arquivo chamado curso-doc.txt usando o comando touch. Eis o comando:

``` touch curso-doc.txt ```

Agora, ao sair do contêiner e desejar acessá-lo novamente, basta utilizar o mesmo contêiner em vez de criar um novo. O comando a seguir permite entrar novamente no mesmo contêiner:

``` docker exec -it meu-container bash ```

Dentro do contêiner, ao usar o comando ls, será possível observar que o arquivo curso-doc.txt ainda estará presente, indicando que o mesmo contêiner está sendo reutilizado.

Portanto, para reutilizar contêineres de forma eficaz, é fundamental nomeá-los com nomes descritivos, como exemplificado com "meu-container". Essa prática facilita o acesso aos contêineres quando necessário, seja no modo interativo ou em outras situações.

