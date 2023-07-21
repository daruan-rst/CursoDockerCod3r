# 11 O que são imagens Docker?


Nesta aula, foi abordado o conceito de imagens Docker e sua importância para a criação e execução de containers. Abaixo estão os principais pontos discutidos:

1. **Imagens como Modelo de Sistema de Arquivos:** Uma imagem Docker é um modelo de sistema de arquivos somente leitura, usado para criar um container. Enquanto o container está associado a um processo em execução, a imagem é um arquivo que contém um sistema de arquivos.

2. **Criação de Imagens:** As imagens podem ser criadas a partir de um processo chamado "build" ou "commit". No entanto, é recomendado o uso de "build" devido à possibilidade de rastrear as alterações feitas na imagem e replicá-las posteriormente.

3. **Registro de Imagens:** As imagens são armazenadas em repositórios dentro de registros. O Docker Hub é um dos principais registros oficiais do Docker, onde as imagens podem ser organizadas em repositórios e diferenciadas por tags, representando diferentes versões do software.

4. **Composição de Camadas:** As imagens são compostas por uma ou mais camadas, também conhecidas como "layers". Cada camada representa uma ou mais mudanças no sistema de arquivos. A junção dessas camadas forma a imagem completa.

5. **Camadas Somente Leitura:** Todas as camadas que compõem a imagem são somente leitura. Isso possibilita o cache desses arquivos, evitando a necessidade de baixar novamente as camadas já existentes.

6. **Alteração no Container:** Quando um container é iniciado, é criada uma camada adicional que permite alterações no sistema de arquivos do container. Essa camada é a única que pode ser alterada, enquanto as demais continuam somente leitura.

7. **Exemplo de Uso:** Ao criar uma nova imagem baseada no sistema operacional Ubuntu versão 16.04, as mudanças feitas na imagem são registradas em camadas adicionais. Essas camadas, em conjunto, formam a imagem final que será usada para montar o sistema de arquivos do container.

A compreensão das imagens Docker é essencial para entender a funcionalidade e a eficiência dos containers. Na próxima aula, serão realizadas comparações mais específicas entre as imagens Docker e os containers para solidificar o conhecimento sobre o assunto.
