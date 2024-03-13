# 41 - Uso das instruções de preparação

Nesta aula é demonstrado como criar um Dockerfile capaz de receber parâmetros durante a execução, permitindo uma maior personalização na criação da imagem Docker.

Para isso, é criado um novo arquivo Dockerfile na pasta "Build" com a instrução `FROM Debian` como imagem base. Em seguida, é adicionada uma linha para especificar o mantenedor da imagem, e um argumento chamado "S3" é definido para permitir a personalização na hora de construir a imagem.

Após salvar o arquivo Dockerfile, o comando `docker build` é executado, passando o argumento `-t` para especificar o nome da imagem e `-build-arg` para passar o valor do parâmetro "S3". Assim, a imagem é construída com base nas instruções do Dockerfile e no valor do argumento passado.

É destacado que cada instrução no Dockerfile gera uma nova camada na imagem Docker, e que é possível concatenar vários comandos em uma única instrução para otimizar o processo de construção.

Além disso, é mencionado que é possível acessar as variáveis de ambiente definidas no sistema durante o processo de construção da imagem, permitindo uma maior flexibilidade na personalização.

Por fim, é demonstrado como utilizar o comando `docker inspect` para filtrar informações específicas sobre a imagem Docker, como o mantenedor, mostrando a versatilidade e personalização oferecidas pelo Docker.
