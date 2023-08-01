# 13: Arquitetura

Vamos falar um pouco sobre a arquitetura do Docker e aqui eu tenho uma imagem que vai ajudar a explicar isso melhor.

O Docker é dividido, pelo menos, em duas partes:

1. Docker Daemon: Também chamado de Docker, Docker server ou Docker engine. Esses três termos são sinônimos e representam esse passaporte azul aqui. O Docker Daemon é responsável por gerenciar os serviços do Docker.

2. Cliente: Essa é a Interface de Linha de Comando (CLI) disponibilizada pelo Docker, e é a forma padrão de acessar os serviços gerenciados pelo daemon. A partir da CLI, você pode fazer coisas como criar uma imagem. O Docker Daemon recebe essa requisição, vai ao Registry do Docker e, lembrando que na aula passada mostrei rapidamente o Docker Hub, onde você pode obter um conjunto de imagens já prontas, ele faz o download dessas imagens e traz para o seu computador local. A partir dessas imagens locais, você pode criar e executar contêineres na sua máquina.

Os contêineres são instanciados e criados para serem executados na máquina local. Então você tem o seu host, que é o dono da imagem. O cliente (CLI) também roda no host, na sua máquina, e ele pega as imagens do hub que estão na nuvem. Essas imagens são armazenadas localmente em cache.

Esse é um processo mais simples, porque quando você tem uma imagem baseada em outra, você só precisa baixar as diferenças entre as imagens. As partes que você já tem no seu computador não precisam ser baixadas novamente, o que torna o processo mais rápido.

A partir disso, monta-se a imagem, geram-se os contêineres e você pode ter vários contêineres gerenciados pelo Docker, que recebe o Docker CLI.

Além disso, existem outras formas de você acessar o servidor do Docker. Por exemplo, você pode criar sua própria aplicação e acessar a partir da API REST disponibilizada pelo Docker. Essa opção existe e há uma ferramenta gráfica também disponibilizada pelo Docker para quem não gosta muito de linha de comando. No entanto, a maior parte do tempo, vamos trabalhar na linha de comando, pois é a forma padrão de se interagir com os componentes do Docker.

Resumindo a arquitetura do Docker:

- Docker Registry: É o ambiente de nuvem onde as imagens são armazenadas. O principal é o Docker Hub, que possui vários repositórios de imagens, e cada imagem é marcada com sua tag.

- Docker Daemon: Recebe as requisições dos clientes, sejam eles clientes da CLI ou aplicações que consomem a API do daemon. Ele faz o download das imagens necessárias e gerencia os contêineres na máquina local.

- Cliente (CLI): Interage com o Docker Daemon, e existem diferentes formas de fazer isso, incluindo a CLI e ferramentas gráficas.

Existem outras formas de interagir com o servidor do Docker, como clientes de linha de comando e aplicações que consomem a API REST. Além disso, ferramentas gráficas também estão disponíveis para gerenciar os seus containers, incluindo o monitoramento oficial.

Você também pode listar os processos que estão ativos, verificar quais são as imagens que você tem localmente e outras ações do tipo.

