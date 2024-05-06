# 42 Uso das Instruções de Povoamento

Neste exemplo, é demonstrado como utilizar as instruções `COPY` e `RUN` para popular uma imagem Docker com arquivos locais.

Primeiramente, é criado um diretório chamado "Build" onde serão armazenados os arquivos necessários. Em seguida, é criado um arquivo HTML básico dentro desse diretório.

No Dockerfile, é especificado que a imagem será baseada no Debian, é definido o mantenedor e é criado um arquivo HTML chamado "conteúdo.html" usando o comando `RUN echo`, que adiciona conteúdo a esse arquivo.

Posteriormente, é utilizada a instrução `COPY` para copiar qualquer arquivo HTML presente na pasta do Dockerfile para dentro do contêiner, garantindo que o arquivo "conteúdo.html" seja incluído na imagem final.

Após salvar o Dockerfile, o comando `docker build` é executado para construir a imagem Docker, especificando o nome da imagem e a pasta onde está localizado o Dockerfile. Em seguida, o contêiner é executado a partir dessa imagem, mapeando a porta 80 do contêiner para a porta 80 do host.

Ao acessar a página através do navegador, é possível verificar que a imagem foi criada com sucesso e que o arquivo HTML foi copiado corretamente para dentro do contêiner, permitindo sua visualização.
