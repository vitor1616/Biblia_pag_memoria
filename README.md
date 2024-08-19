# Biblia_pag_memoria

    O QUE O PROGRAMA FAZ?

Este programa utiliza páginas de memória virtual do sistema operacional para gerenciar dados em arquivos, permitindo realizar operações de leitura e escrita diretamente na memória. Como exemplo, ele escreve o conteúdo da Bíblia em um arquivo .txt a partir da memória virtual.

    PARA RODAR, USE O main.c com:
gcc -o main main.c

./main

Conteúdo:
> Main.c - Arquivo principal que faz a manipulação de memória e leitura e escrita dos arquivos.

> BIBLIA_COMPLETA.txt - Biblia em espanhol no formato de texto

> biblia.txt - arquivo criado com o conteúdo de BIBLIA_COMPLETA.txt

    DESCRIÇÃO
O programa faz o mapeamento do arquivo BIBLIA_COMPLETA.txt para a mem usando o mmap. Criar o arquivo biblia.txt e alterar para o tamanho do arquivo origem usando ftruncate, o programa mapeia biblia.txt para memoria. BIBLIA_COMPLETA.txt é copiado para biblia.txt utilizando memcpy. No final o programa desmapea os dois arquivos da memoria utilizando munmap.
