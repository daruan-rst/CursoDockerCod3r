# 30 - Mapear diretórios para o container

Nesta aula, foi discutido o conceito de mapeamento de volumes no Docker, uma técnica crucial para compartilhar dados entre o host e os contêineres. Um exemplo prático foi dado, onde uma estrutura de arquivos específica foi criada no host e a imagem do Apache foi usada para ilustrar o processo de mapeamento.

Primeiro, uma estrutura de arquivos foi criada no host. Uma pasta chamada "CursoDocker" foi criada no desktop, contendo uma subpasta chamada "ExercicioVolume" e um arquivo HTML chamado "index.html" dentro desta última pasta.

Em seguida, o Docker foi usado para criar um contêiner Apache, mapeando a porta 80 do contêiner para a porta 8080 do host. O mapeamento de volumes foi feito usando a opção `-v` do Docker. No exemplo, a pasta "ExercicioVolume" no host foi mapeada para a pasta padrão do Apache, onde os arquivos são servidos.

```bash
``` 
docker run -p 8080:80 -v $(pwd)/ExercicioVolume:/var/www/html apache 
```
```


Essa abordagem permite que o Apache no contêiner acesse e manipule os arquivos na pasta "ExercicioVolume" do host. Qualquer alteração feita nessa pasta no host é automaticamente refletida dentro do contêiner, possibilitando uma eficiente comunicação de dados entre o host e o ambiente contido no Docker.

Esse exemplo prático demonstra a praticidade e flexibilidade do mapeamento de volumes no Docker, sendo uma técnica essencial para o desenvolvimento e implantação de aplicações de forma eficaz e organizada.
 
