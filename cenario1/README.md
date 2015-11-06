### Descrição
Uma universidade possui um pacote de classes em C++ que devem ser integradas em um sistema maior com diversos outros componentes escritos em java que funcionarão como o cliente solicitando serviços dos objetos C++. Por questões de desempenho não está sendo cogitada a reescrita do pacote de classes C++ em java.

### Como executar
No sistema operacional Ubuntu, foi necessário instalar libmicrohttpd:
```
sudo apt-get install libmicrohttpd10 libmicrohttpd-dev
```

Após a instalação da biblioteca, compilar o código-fonte:
```
cc hellobrowser.c -o hellobrowser -I$PATH_TO_LIBMHD_INCLUDES -L$PATH_TO_LIBMHD_LIBS -lmicrohttpd
```

Executar o binário:
```
./hellobrowser
```

Acessar no browser:
```
http://localhost:8888
```
