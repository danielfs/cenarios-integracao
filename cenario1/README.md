Uma universidade possui um pacote de classes em C++ que devem ser integradas em um sistema maior com diversos outros componentes escritos em java que funcionarão como o cliente solicitando serviços dos objetos C++. Por questões de desempenho não está sendo cogitada a reescrita do pacote de classes C++ em java.

### Como executar
1. No sistema operacional Ubuntu, foi necessário instalar libmicrohttpd:
 1. sudo apt-get install libmicrohttpd10 libmicrohttpd-dev

2. Após a instalação da biblioteca, compilar o código-fonte:
 1. cc hellobrowser.c -o hellobrowser -I$PATH_TO_LIBMHD_INCLUDES -L$PATH_TO_LIBMHD_LIBS -lmicrohttpd

3. Executar o binário:
 1. ./hellobrowser

4. Acessar no browser:
 1. http://localhost:8888
