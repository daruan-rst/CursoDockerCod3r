# 9 Por que não uma VM?


Nesta aula, foi abordada a pergunta sobre por que não usar uma máquina virtual (VM) em vez do Docker. Embora as VMs tenham revolucionado o mercado de tecnologia e sejam amplamente utilizadas, o Docker oferece benefícios distintos. O Docker é uma tecnologia de virtualização baseada em contêineres, que apresenta vantagens em termos de consumo de recursos.

## Características do Docker
1. Vantagens das máquinas virtuais:

- Isolamento do sistema: As VMs permitem isolar completamente o sistema operacional e as aplicações.
- Elasticidade: É possível ajustar a quantidade de recursos alocados para uma VM de acordo com a necessidade.

2. Vantagens do Docker em relação às VMs:

- Consumo de recursos reduzido: Os contêineres do Docker consomem menos recursos em comparação com uma VM completa. O tempo de inicialização de um contêiner é muito rápido, em torno de segundos.
- Compartilhamento de recursos: O Docker compartilha o kernel do sistema operacional com os contêineres, resultando em economia de recursos, como memória.
- Facilidade de uso: O Docker fornece uma camada de acesso amigável, tornando mais fácil a criação e gerenciamento de contêineres.

3. Comparação entre o Docker e as VMs:

- Ambos têm um servidor físico como base e um sistema operacional instalado.
- No caso das VMs, cada uma possui um sistema operacional completo, enquanto os contêineres do Docker compartilham o kernel do sistema operacional do host.
- Os contêineres do Docker são executados como processos isolados com sistemas de arquivos isolados, permitindo a execução de aplicações com suas dependências em ambientes controlados.
- O Docker utiliza a tecnologia LXC (Linux Containers) para gerenciar os contêineres, proporcionando uma camada amigável para acessá-los.

O Docker oferece a maioria das vantagens das VMs, como isolamento e elasticidade, enquanto consome menos recursos. No entanto, existem casos específicos em que as VMs são necessárias, como quando é preciso executar sistemas operacionais diferentes do Linux ou usar tecnologias específicas disponíveis apenas em determinadas VMs.

O Docker simplificou o uso da tecnologia de contêineres, tornando-a mais acessível e popular. Sua adoção tem crescido rapidamente, sendo amplamente utilizado tanto no desenvolvimento quanto em ambientes de produção.
