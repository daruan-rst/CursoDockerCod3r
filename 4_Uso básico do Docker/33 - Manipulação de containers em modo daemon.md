# 33 - Manipulação de containers em modo daemon

### Listar todos os containers em execução
``` docker container ls ```

### Listar todos os containers (incluindo os parados)
``` docker container ls -a ```

### Visualizar os logs de um container
``` docker container logs <nome_do_container> ```

### Inspecionar um container para obter informações detalhadas
``` docker container inspect <nome_do_container> ```

### Executar um comando dentro de um container
``` docker container exec <nome_do_container> <comando> ```
