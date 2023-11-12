# 37 - Entendendo melhor as imagens

- Imagens e containers têm identificadores únicos (hash sha256), mas trabalhar diretamente com esses hashes não é prático para humanos.
- Geralmente, você acessa imagens através de nomes únicos atribuídos a elas.
- As imagens são organizadas em registros, como o Docker Hub, que contém vários repositórios. Exemplo: "docker.io/library/ruby".
- Cada repositório pode ter várias tags, indicando diferentes versões ou variantes da imagem.
- Comum usar o nome do repositório e a tag para baixar uma imagem. Exemplo: `docker pull ruby:latest`.

Observação: No exemplo mencionado, a sintaxe antiga `docker pull ruby:latest` foi usada. O instrutor menciona que a sintaxe nova será usada no console.

