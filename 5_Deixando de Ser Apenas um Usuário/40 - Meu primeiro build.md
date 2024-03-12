# 40 Meu primeiro build

Nesta aula, é abordado o processo de construção da primeira imagem Docker. O instrutor destaca a importância desse momento, onde os usuários passam a ser capazes de criar suas próprias imagens.

O primeiro passo é criar um arquivo de descrição sem extensão, chamado "Dockerfile", que contém as instruções para construir a imagem. Em seguida, é necessário especificar a imagem base com o comando `FROM`, que define a versão base do sistema operacional a ser utilizada.

Após definir a imagem base, são adicionadas as instruções para a configuração da imagem, como instalação de pacotes, configuração de portas, entre outras. No exemplo fornecido, é utilizado o comando `RUN` para executar um simples "Hello World" em um arquivo HTML.

Depois de definir as instruções no Dockerfile, o próximo passo é executar o comando `docker build`, apontando para o diretório onde está o Dockerfile. Este comando irá compilar as instruções e gerar a imagem Docker.

Por fim, é possível testar a imagem criada executando um contêiner a partir dela, usando o comando `docker run`. Este comando especifica as portas a serem usadas e o nome da imagem a ser executada.

É enfatizado que o Dockerfile precisa ter o nome exato, com "D" maiúsculo e sem extensão, para que o processo de construção ocorra corretamente.

É importante o uso do Docker não apenas para desenvolvimento, mas também para ambientes de produção, onde é crucial ter ambientes consistentes e reproduzíveis.
