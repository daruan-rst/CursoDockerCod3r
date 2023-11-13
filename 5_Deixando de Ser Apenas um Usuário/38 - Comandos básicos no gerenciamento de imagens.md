# 38 - Comandos básicos no gerenciamento de imagens

Sete comandos essenciais para o gerenciamento de imagens no Docker:

1. **`docker image pull`**: Baixa uma imagem diretamente, sendo muitas vezes acionado implicitamente ao tentar executar um contêiner com uma imagem ausente localmente.

2. **`docker image ls`**: Lista as imagens disponíveis localmente. O comando `ls` é corriqueiro para quem já trabalha com Linux.

3. **`docker image rm`**: Remove uma ou mais imagens. O instrutor menciona a possibilidade de encadear regras para remover várias imagens.

4. **`docker image inspect`**: Inspeciona uma imagem, fornecendo um documento com informações cruciais sobre ela.

5. **`docker image tag`**: Permite adicionar uma nova tag a uma imagem existente. O exemplo mencionado envolve aplicar uma tag a partir de outra imagem.

6. **`docker image build`**: Essencial para criar imagens, será aprofundado nas próximas aulas. O instrutor destaca a importância de entender o processo de build e a criação de Dockerfiles.

7. **`docker image push`**: Publica uma imagem em um registro, sendo útil para distribuir imagens em ambientes específicos, como uma empresa.

O instrutor ressalta que o comando `build` será abordado detalhadamente, pois envolve a criação do Dockerfile, uma peça fundamental no processo de construção de imagens.
