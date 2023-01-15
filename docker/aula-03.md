# Docker parte 1

## O que são imagens e containers

1. **Imagem**: Uma imagem contém tudo que uma aplicação precisa para funcionar, por exemplo:
   1. Uma imagem possui um sistema operacional dentro dela.
   2. Uma imagem possui várias librarys (bibliotecas)
   3. Uma imagem possui os arquivos de uma aplicação que voce vai rodar nela.
   4. Uma imagem possui váriaveis de ambiente.
2. **Container**: Um container é um ambiente isolado. Um container contém um conjunto de processos que são executados a partir de uma imagem, imagem esta que fornece todos os arquivos necessários. Os containers compartilham o mesmo kernel e isolam os processos da aplicação do restante do sistema.
   1. Uma VM (isolado)
   2. Ele pode ser Iniciado, Parado, Excluido e reiniciado.
   3. Container possui dentro dele uma imagem
   ```
   APP -->   Imagem     --> Container
            DockerFile      Imagem
                            Run
                            APP
   ```