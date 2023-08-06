# 21: Meu querido amigo run

Nesta aula, vamos entender o comando "docker run", que é a porta de entrada para o mundo do Docker e permite realizar uma série de ações, incluindo o download de imagens, criação e execução de containers.

Antes de continuar, é importante mencionar que, a partir da versão 17.06 do Docker, houve uma mudança significativa nos comandos, incluindo o "docker run". No curso, trabalharemos com a versão mais recente dos comandos, e muitos dos comandos antigos ainda funcionam, mas estaremos nos concentrando na nova sintaxe.

O comando "docker run" agrupa várias ações em um só. Vejamos os principais passos que ele executa:

1. Baixar uma imagem pública do registro oficial do Docker para a sua máquina local, caso ela ainda não esteja presente no cache.

2. Criar um contêiner com base na imagem baixada.

3. Iniciar o contêiner que acabou de ser criado.

4. Executar o contêiner no modo interativo, permitindo interagir com ele diretamente.

Ao executar o comando "docker run" pela primeira vez, ele fará o download da imagem e executará o contêiner no modo interativo, mostrando a saída correspondente. Na próxima vez que você executar o mesmo comando, como a imagem já estará presente no cache, o processo será mais rápido e ele apenas executará o contêiner no modo interativo.

Lembre-se de que, para garantir o correto funcionamento do Docker, é essencial ter seguido corretamente os passos de instalação apresentados nas aulas anteriores. Em caso de dúvidas ou problemas, compartilhe no fórum do curso, detalhando o que aconteceu para que possamos ajudá-lo da melhor forma possível.

Pronto! Agora você compreende melhor o comando "docker run" e sua importância para a utilização do Docker. Na próxima aula, vamos explorar mais sobre os recursos dos contêineres Docker.

