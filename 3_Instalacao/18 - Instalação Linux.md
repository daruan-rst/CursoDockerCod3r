# 18: Instalação Linux

Se você usa Linux, terá uma facilidade maior, já que está acostumado a trabalhar com o terminal.

## Passos para instalação do Docker no Linux:

1. Primeiro, faça um update e garanta que tudo esteja atualizado:

   ``` sudo apt-get update ```
   ``` sudo dpkg --add-architecture amd64 ```
   ``` sudo apt-get update ```

2. Em seguida, adicione o repositório do Docker:

   ``` sudo apt-get install apt-transport-https ca-certificates curl software-properties-common ```
   ``` curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg ```
   ``` echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null ```

3. Novamente, atualize o repositório após a adição do Docker:

   ``` sudo apt-get update ```

4. Finalmente, execute o comando de instalação do Docker:

   ``` sudo apt-get install docker-ce ```

   Durante a instalação, quando solicitado, digite Y ou S para confirmar.

5. Verifique se o Docker foi instalado corretamente:

   ``` docker --version ```

   Após a instalação, você verá a versão do Docker instalada no seu sistema.

Pronto! A instalação do Docker em ambiente Linux foi concluída com sucesso. Agora você tem o Docker instalado e pronto para uso.

Em caso de dúvidas, você pode consultar a documentação oficial do Docker ou procurar por tutoriais específicos para a sua distribuição Linux.

