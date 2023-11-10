# 36 - Diferenças entre container e imagem

### Imagem
- Equivalente à classe na programação orientada a objetos.
- Modelo de sistema de arquivos somente leitura formado em camadas.
- As camadas formam o sistema de arquivos usado pelo container.

### Container
- Equivalente ao objeto na programação orientada a objetos.
- Processo isolado que tem acesso ao sistema de arquivos da imagem.
- Pode criar muitos sub-processos e fazer alterações na camada do sistema de arquivos.

## Comandos Úteis

### Container
- `docker container --help`: Mostra subcomandos relacionados a containers e documentação.
- `docker container ls --help`: Mostra comandos específicos para listagem de containers.

### Imagem
- `docker image --help`: Mostra subcomandos relacionados a imagens e documentação.
- `docker image ls --help`: Mostra comandos específicos para listagem de imagens.

### Volume
- `docker volume --help`: Mostra subcomandos relacionados a volumes e documentação.
- `docker volume ls --help`: Mostra comandos específicos para listagem de volumes.

## Observações
- Alguns comandos podem não ser abordados neste momento do curso, mas estão disponíveis para referência futura.
