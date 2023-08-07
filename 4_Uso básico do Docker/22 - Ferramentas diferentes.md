# 22: Ferramentas diferentes

Nesta aula, vamos aprender sobre os dois modos básicos de execução no Docker: o modo Daemon e o modo Interativo.

O modo Daemon é o modo primordial do Docker, no qual você executa um contêiner e ele permanece rodando em background, como um processo em execução contínua. Esse modo é ideal para deixar serviços em execução, como bancos de dados ou servidores, que precisam estar disponíveis o tempo todo.

Já o modo Interativo é mais utilizado para fins de testes, experimentos e configurações. Nele, você pode entrar no contêiner e interagir diretamente com ele, executando comandos e verificando resultados.

Ao longo do curso, vamos explorar principalmente o modo Interativo, pois ele nos permite entender melhor o funcionamento dos contêineres Docker e realizar diversos exercícios práticos.

Vamos fazer um exercício para testar a execução de um contêiner em modo Interativo. Abra o terminal e digite o seguinte comando:

``` docker run debian echo "Olá Mundo" ```

Nesse comando, estamos executando um contêiner baseado na imagem "debian" e pedindo para ele imprimir a mensagem "Olá Mundo" no console. O Docker fará o download da imagem do Debian, criará e iniciará o contêiner e executará o comando em modo interativo.

Agora, vamos executar um comando semelhante, mas com uma pequena diferença. Digite o seguinte comando:

``` docker run -it --rm debian echo "Olá Mundo" ```

Nesse comando, adicionamos a opção "-it" para que o Docker execute o contêiner em modo interativo e a opção "--rm" para que ele seja automaticamente removido da lista de contêineres após a conclusão do processo.

Observe que, ao executar o primeiro comando novamente, a execução será mais rápida, pois o Docker utilizará a imagem já presente no cache local.

Esses são apenas alguns exemplos de como podemos utilizar os comandos no Docker. Nas próximas aulas, vamos explorar mais recursos e conceitos importantes relacionados ao Docker.

