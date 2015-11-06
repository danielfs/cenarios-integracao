### Descrição
Hello World da biblioteca libmicrohttpd, na linguagem C.

### Recursos utilizados
https://www.gnu.org/software/libmicrohttpd/tutorial.pdf

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
