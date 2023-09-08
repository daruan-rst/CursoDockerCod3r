# 24 - Containers devem ter nomes únicos

Para atribuir um nome a um contêiner, pode-se usar a opção `--name` ao executar o comando `docker run`. Por exemplo:

``` docker run -it --name meu-container debian bash ```

Neste comando, utilizamos as opções `-it` para acesso ao terminal interativo, `--name meu-container` para nomear o contêiner como "meu-container", `debian` como a imagem base e `bash` como o comando a ser executado no contêiner.

Após executar esse comando, você entrará rapidamente no terminal do contêiner Debian. Para sair do contêiner, basta digitar `exit`.


Ao tentar criar um novo contêiner com o mesmo nome:

``` docker run -it --name meu-container debian bash ```

Você notará que o comando gera um erro. Isso ocorre porque os contêineres devem ter nomes únicos. Se você tentar criar um contêiner com um nome que já foi usado, o Docker não permitirá e gerará um erro.

É importante lembrar que os contêineres devem ter nomes exclusivos. Se for preciso criar um novo contêiner com o mesmo nome, primeiro remova o contêiner existente com o nome já usado.

Além disso, é preciso lembrar que o comando `docker run` sempre cria um novo contêiner, mesmo que um contêiner com o mesmo nome já exista. Portanto, cada execução do comando `docker run` gera um novo contêiner, e esses contêineres devem ser nomeados de forma exclusiva.



