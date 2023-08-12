# 23 - Run cria sempre novos containers

Um conceito importante sobre o comando `docker run` é que ele sempre cria um novo contêiner quando é invocado. Isso já foi observado anteriormente ao utilizarmos o comando `docker ps`.

Vamos explorar esse conceito com um exemplo prático.

Primeiro, vamos limpar o console e executar o seguinte comando:

``` docker run -it --name meu-container debian bash ```

Nesse comando, utilizamos as opções `-it` para ter acesso ao terminal interativo do contêiner e `--name meu-container` para nomear o contêiner como "meu-container". O `debian` é a imagem base que estamos utilizando, e `bash` é o comando que estamos executando no contêiner, o que nos permitirá interagir com o terminal.

Ao executar esse comando, você verá que entra no terminal do contêiner, e a partir daí, poderá realizar comandos dentro dele. Vamos criar um arquivo chamado "curso-docker.txt" dentro do contêiner utilizando o comando `touch curso-docker.txt`.

Agora, saia do contêiner digitando `exit`.

Em seguida, vamos criar um novo contêiner com o mesmo comando:

``` docker run -it --name meu-container-2 debian bash ```

Ao entrar neste novo contêiner, tente verificar a existência do arquivo que criamos anteriormente:

``` ls curso-docker.txt ```

Você verá que o arquivo não está presente. Isso ocorre porque o comando `docker run` cria um novo contêiner a cada execução e, portanto, não compartilha o estado do contêiner anterior.

Ao utilizar o comando `docker ps`, você notará que os contêineres têm nomes gerados automaticamente, como "admiring_turing" e "happy_shirley". Na próxima aula, exploraremos como nomear contêineres de forma mais significativa.


