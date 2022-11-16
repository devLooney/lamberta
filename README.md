# lamberta
Jogo Lamberta, projeto para a faculdade.

Devemos criar um jogo de tabuleiro que se chama lamberta.

Regras do jogo Lamberta
O jogo Lamberta decorre entre dois jogadores, num tabuleiro linear, preenchido com marcas O e X. Exemplo
de uma posição inicial com 9 casas:
X O O X O O O X X
Os jogadores jogam alternadamente, selecionando um segmento do tabuleiro. O resultado da seleção é a
troca de todas as marcas no segmento. Exemplo de duas jogadas:
Jogada Tabuleiro
1 X O O X O O O X X
2 X O O O X X X X X
3 X O X X O X X X X
Na jogada 1 o segmento selecionado a verde tem as marcas trocadas na posição seguinte, da jogada 2, tendo
sido marcadas a laranja. Na jogada 2 há novo segmento que é invertido na posição seguinte da jogada 3.
Uma jogada para ser válida tem de obedecer às seguintes regras:
• Selecionar pelo menos uma casa com X
• O número de elementos do segmento tem de ser igual ou inferior ao tamanho do tabuleiro menos
o número da jogada. Caso o número da jogada seja igual ou superior ao tamanho do tabuleiro, são
aceites segmentos de tamanho 1.
De acordo com as regras em cima, na primeira jogada num tabuleiro de 9 casas são permitidos segmentos
até 8 elementos (9-1). Na jogada 2 são aceites segmentos até 7 elementos (9-2). No caso da jogada 9 e
superior são aceites apenas segmentos com 1 elemento.
O objetivo do jogo é forçar o adversário a fazer uma jogada inválida.
Exemplo de um jogo:
Jogada Tabuleiro Maior segmento
1 O X X O X X O O X 8
2 O X O X O O O O X 7
3 O X O O X X X X O 6
4 O X O O O O O O X 5
5 X O X O O O O O X 4
6 X O O X X O O O X 3
7 X O O X O X O O X 2
8                   1
9                   1
10                  1
Jogador azul faz uma jogada inválida na jogada 7, não selecionando nenhum X, pelo que perde. Assim, não
são permitidas mais jogadas, terminando o jogo. Caso não tivesse existido uma jogada inválida, na jogada 8
e seguintes apenas são permitidos segmentos com 1 elemento.
