# 28 - Mapear portas dos containers

# Mapeamento de Portas e Interação Básica com Contêineres no Docker

Nesta fase inicial do uso do Docker, estamos explorando as funcionalidades básicas do Docker, ainda como usuários, sem criar nossas próprias imagens ou ambientes mais complexos. Nesta aula, vamos aprender como mapear uma porta para permitir a comunicação entre o host e um contêiner.

## Mapeamento de Portas

Para começar, vamos instalar um servidor chamado Engineers e mapear a porta 80 do contêiner para a porta 80 do host. No terminal, digite o seguinte comando:

```
docker run -p 80:80 enginx
```

Neste comando:
- ```docker run -p 80:80 enginx```: Inicia um novo contêiner e mapeia a porta 80 do host para a porta 80 do contêiner.
  
Após executar o comando, o Docker irá baixar a imagem do Nginx (se você ainda não a tiver) e iniciar um contêiner com o servidor web Nginx na porta 80.

Você pode verificar se o contêiner está em execução usando o comando:

```
docker ps
```

Para acessar o servidor web Nginx do contêiner, basta abrir um navegador e digitar `http://localhost:80`. Você verá a página padrão do Nginx.

Para parar o contêiner, você pode usar o comando:

```
docker stop <ID ou Nome do Contêiner>
```

Lembre-se de substituir `<ID ou Nome do Contêiner>` pelo ID ou nome real do contêiner que você deseja parar.

E é isso! Agora você aprendeu como mapear uma porta para permitir a comunicação entre um contêiner Docker e o host. Na próxima aula, vamos explorar outro tipo de interação entre a máquina host e o contêiner: o mapeamento de volumes, um aspecto crucial no mundo do Docker.
 
