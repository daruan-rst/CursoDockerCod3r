# 31 - Rodar um servidor web em background

Nesta seção, abordaremos como executar contêineres em segundo plano, no modo "daemon". O modo "daemon" é útil quando você deseja que o contêiner seja executado como um processo em segundo plano, sem interação direta no console. Isso é particularmente útil para cenários de produção, como servidores web, bancos de dados e outros serviços que precisam ser executados de forma contínua.

**Executando um Contêiner em Segundo Plano:**

Para iniciar um contêiner em segundo plano, use o seguinte comando Docker:

```
docker container run -d
```

- `-d`: Este sinalizador indica que você deseja que o contêiner seja executado em segundo plano, no modo "daemon".

Por exemplo, para criar um contêiner chamado "exercicio_fisico" mapeando a porta 8080 para a porta 80 interna e montando um volume, você pode usar o seguinte comando:

```
docker container run -d -p 8080:80 -v $(pwd)/ExercicioVolume:/var/www/html apache
```

Neste comando:
- `-d`: Inicia o contêiner em segundo plano.
- `-p 8080:80`: Mapeia a porta 8080 do host para a porta 80 interna do contêiner.
- `-v $(pwd)/ExercicioVolume:/var/www/html`: Monta um volume, permitindo que o Apache acesse arquivos da pasta local "ExercicioVolume" e servindo-os no diretório "/var/www/html" do contêiner.
- "apache": Especifica a imagem a ser usada.

Com isso, o contêiner Apache será executado em segundo plano, pronto para servir conteúdo.

Para listar contêineres em execução, use:

```
docker ps
```

Para parar um contêiner em execução, use:

```
docker stop NOME_DO_CONTÊINER
```

Lembre-se de que o modo "daemon" é ideal para ambientes de produção, onde você deseja que os contêineres funcionem como processos em segundo plano, interagindo entre si para fornecer serviços complexos. O Docker oferece flexibilidade e eficiência, mesmo quando você não está criando suas próprias imagens, como vimos nestes exemplos.

 
