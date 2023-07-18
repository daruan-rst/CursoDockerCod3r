# 8 O que é Docker?


A aula aborda o significado e os conceitos básicos do Docker, uma tecnologia de virtualização. No entanto, o Docker difere da virtualização tradicional baseada em máquinas virtuais. Através de uma pincelada sobre esses conceitos, é possível entender o Docker como uma engine de administração de contêineres, que permite testar e executar aplicações de forma isolada do sistema host.

## Características do Docker
1. Não é um sistema de virtualização tradicional:

- O Docker não utiliza máquinas virtuais completas, como na virtualização tradicional. Ele trabalha com contêineres, que são processos segregados e isolados do sistema host.
- Os contêineres possuem um sistema de arquivos isolado, permitindo a execução de software com suas dependências e bibliotecas específicas dentro de um ambiente controlado.

2. Engine de administração de contêineres:

- O Docker é uma engine de administração de contêineres que permite criar e gerenciar contêineres a partir do Docker.
- Os contêineres são processos segregados e isolados do sistema host, nos quais é possível testar e executar aplicações.
- Cada contêiner possui seu próprio sistema de arquivos isolado, proporcionando um ambiente controlado para a execução do software.

3. Utiliza os serviços do LXC (Linux Containers):

- O Docker se baseia na tecnologia LXC, que pertence ao Linux. Isso significa que os contêineres Docker são baseados em sistemas operacionais Linux, como Debian, Ubuntu ou Red Hat.
- Os contêineres não podem ser baseados em sistemas operacionais como Mac ou Windows, pois dependem do kernel do sistema host.

4. Open Source e escrito em Go:
- O Docker é uma tecnologia open source, o que contribuiu para seu grande crescimento.
- Foi desenvolvido utilizando a linguagem de programação Go, criada pelo Google.

5. Sistema de virtualização baseado em software (SO):

- O Docker utiliza a virtualização baseada em software, ou seja, virtualização baseada no sistema operacional.
- Ao contrário da virtualização tradicional, o Docker compartilha o kernel da máquina host com os contêineres, o que resulta em menor consumo de recursos, maior velocidade e isolamento eficiente.

6. Host e contêiner compartilham o kernel:

- O Docker compartilha o kernel da máquina host com os contêineres, mas não utiliza diretamente o kernel do host.
- Além disso, algumas bibliotecas e binários também são compartilhados, o que contribui para a eficiência do Docker.

7. Empacota software com vários níveis de isolamento:
- O Docker oferece diversos níveis de isolamento para os contêineres.
- É possível isolar a quantidade de memória, o uso da CPU, a rede e o sistema de arquivos de cada contêiner.
- Cada contêiner possui um endereço IP próprio, permitindo o acesso através desse endereço.
- O isolamento do sistema de arquivos é fundamental para o controle e isolamento efetivo do Docker, garantindo que os processos executem apenas dentro do sistema de arquivos do contêiner.


Compreender essas características é importante para desenvolver um entendimento sólido do Docker e se aprofundar nos conceitos específicos que serão abordados nas aulas subsequentes.
