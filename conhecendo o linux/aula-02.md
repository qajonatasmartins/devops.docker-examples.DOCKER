# Aprendendo comandos linux

1. `whoami`: Para descobrir o nome do usuário do linux
2. `echo`: É para retornar um texto. Exemplo: `echo olá`, então ele imprime no terminal `olá`
3. Falar qual diretório está `echo $0` retorna o diretorio/pasta que vc está.
4. O comando `apt list` lista pacotes dentro da distribuição linux. [veja aqui o que é apt(advanced package tools)](https://www.guiafoca.org/guiaonline/intermediario/ch20s02.html#:~:text=O%20apt%20%C3%A9%20sistema%20de,sendo%20bastante%20f%C3%A1cil%20de%20usar.).
5. O comando `apt update` atualiza os pacotes mais utilizados e também atualizados.
6. Para instalar um pacote use o `apt install nome_do_pacote`
7. Ler conteúdo de um arquivo com o comando `cat nome_arquivo.extensao`
8. Add informações dentro de um arquivo com comando `echo`, basta somente executar o comando `echo mensagem que vc quer > nome_arquivo.txt`
9. Usando o GREP (global regular expression print) para fazer buscas no conteúdo dos arquivos procurando linhas que encontrem a expressão regular mencionada. Todas as linhas encontradas são mostradas na saída padrão. Executem o comando `grep hello nome_arquivo.txt` ou `grep palavra_que_vc_quer nome_arquivo.txt nome_arquivo2.txt` ou `grep palavra_que_vc_quer parteDoNomeDoArquivo(s)**` ou `grep -i -r palavra_que_vc_quer .`. [mais formas](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/)
10. Usando o FIND para pesquisar os arquivos dentro de uma pasta ou listar todos os arquivos inclusive os ocultos. usa só o `find` ou `find nome_do_arquivo`. 
    1.  Outras formas: 
        1.  `find -type f`: lista todos os arquivos do diretorio
        2.  `find -type d`: lista todos os diretorios (pastas)
        3.  `find -type f -name "nomeDoArquivo.extensao"`: verifica se no diretorio tem aquele arquivo. o valor do arquivo pesquisado tem que ser exatamente o que vc quer.
        4. `find -type f -name "nomeDo**"`: pesquisa um arquivo que comece com 'nomeDo'.
11. multiplos comandos no terminal:
    1.  separamos por ';', exemplo: `mkdir teste1 ; cd teste1 ; echo ok`. Aqui se houver erro no primeiro comando ele continua os proximos.
12. operado and para rodar um comando e se o primeiro der erro ele para: `mkdir teste1 && cd teste1 && echo ok`
13. Visualizar os processos executados na maquina, para isso execute o `ps`
14. matar o processo em execução: `kill number_PID` o pid é pego pelo comando do `ps`.