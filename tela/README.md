## tela - conjunto de funções simples para manuseio de tela gráfica

O arquivo [tela.h](tela.h) contém a declaração de um conjunto de funções que permitem realizar algumas operações em uma tela gráfica, suficientes para a implementação de programas não muito complexos que usem esse tipo de interface.
Ela possui funções para (olhe o conteúdo do arquivo para mais detalhes):
- criação de uma janela, deve ser a primeira função desse arquivo a ser chamada
- finalização da tela gráfica, deve ser a última função desse arquivo a ser chamada
- desenho de círculo, linha, retângulo, texto, desenham em uma representação da tela na memória
- definição de nova cor, além das 10 pré-definidas
- atualização da tela - copia da representação em memória para a janela, e limpa a representação em memória
- obtenção da posição e estado atual do botão esquerdo do mouse
- informação sobre o mouse ter sido clicado e onde isso ocorreu a última vez
- obtenção do caractere que tenha sido digitado no teclado
- obtenção do tempo transcorrido desde o início da execução do programa

A implementação dessas funções está no arquivo [tela.c](tela.c). Você não precisa olhar esse arquivo. Para implementá-las, é usada a biblioteca allegro, que deve estar disponível para que o programa possa ser compilado.
Para que as funções de desenho de texto funcionem, é necessário um arquivo com o desenho das letras. A implementação em tela.c usa para isso o arquivo [DejaVuSans.ttf](DejaVuSans.ttf), que deve estar presente.
O arquivo [exemplo.c](exemplo.c) tem um pequeno programa que exemplifica o uso dessas funções.
Para compilar um programa que use essas funções, deve-se compilar o programa, mais o arquivo tela.c e pedir para o compilador incluir diversas bibliotecas de função do allegro. Tem um comentário no início do arquivo exemplo.c com a linha de comando para compilar com o gcc.

Caso não esteja conseguindo a execução local do programa, tem uma cópia funcional desses arquivos no [replit](https://replit.com/@BenhurStein/testeallegro); faz um fork. A execução no replit é bem menos confortável que a execução local, por causa do atraso.

Um segundo exemplo ([exemplo2.c](exemplo2.c)) tem um programa um pouco mais elaborado (não tá no replit).
