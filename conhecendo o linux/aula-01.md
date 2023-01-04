# Executando Ubuntu

Executando o ubuntu em uma maquina windows, mac ou outra sem ter que baixar a imagem.

1. Abra o terminal do seu pc
2. Digite `docker run -it ubuntu`
   1. Onde `docker run` é o comando para executar uma ação no docker
   2. `-it` neste comando estamos usando os parâmetros -it onde i significa o modo interativo e o t para que possamos ter acesso ao terminal bash:
      1. -i é o parâmetro para interagir(vai manter o STDIN aberto).
      2. -t é para alocar um TTY(Talk to you) que é um terminal.
   3. `ubunto` é a imagem que estamos executando.