# 12: Imagem vs. Container
Nesta aula, foi realizada uma comparação entre imagens e containers, utilizando o conceito de orientação a objetos como analogia. Abaixo estão os principais pontos discutidos:

- **Relação entre Imagem e Container:** Assim como na orientação a objetos, onde temos uma classe como modelo para criar múltiplos objetos, no Docker, a imagem é usada como um modelo para criar múltiplos containers.

- **Imagem como Classe:** A imagem Docker é comparada à classe no paradigma de orientação a objetos. Ela atua como o "molde" ou "modelo" para a criação de containers.

- **Container como Objeto:** O container é a realização concreta da imagem. Quando um container é iniciado, ele é como um objeto criado a partir de uma classe, ou seja, uma instância específica da imagem.

- **Uso de uma Única Imagem para Múltiplos Containers:** A partir de uma única imagem, é possível iniciar diversos containers. Cada container é independente, mas compartilha a mesma estrutura e configurações definidas na imagem.

- **Funcionamento do Container:** O container, quando iniciado, é o processo que está em execução na memória do computador. Ele monta o sistema de arquivos somente leitura baseado nas camadas da imagem, permitindo a execução de aplicativos, bibliotecas e binários.

A comparação com orientação a objetos ajuda a entender a relação entre imagens e containers, tornando mais claro o conceito de como uma imagem é usada como modelo para criar e executar múltiplos containers.
