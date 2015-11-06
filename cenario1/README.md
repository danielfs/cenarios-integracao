Uma universidade possui um pacote de classes em C++ que devem ser integradas em um sistema maior com diversos outros componentes escritos em java que funcionarão como o cliente solicitando serviços dos objetos C++. Por questões de desempenho não está sendo cogitada a reescrita do pacote de classes C++ em java.

### Como executar
1. No sistema operacional Ubuntu, foi necessário instalar libmicrohttpd: 1
    1. sudo apt-get install libmicrohttpd10 libmicrohttpd-dev 1.1

2. Após a instalação da biblioteca, compilar o código-fonte: 2
    1. cc hellobrowser.c -o hellobrowser -I$PATH_TO_LIBMHD_INCLUDES -L$PATH_TO_LIBMHD_LIBS -lmicrohttpd 2.1

3. Executar o binário: 3
    1. ./hellobrowser 3.1

4. Acessar no browser: 4
    1. http://localhost:8888 4.1
