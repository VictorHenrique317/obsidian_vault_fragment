TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
10/11/2023 - 09:58
Relações:
# Flashcards

Onde o mecanismo de attention é aplicado? #flashcard 
Em LSTM's
<!--ID: 1699621258970-->

Qual é a ideia geral do mecanismo de attention?  #flashcard 
Fazer com que a LSTM se lembre das palavras mais importantes
<!--ID: 1699621233609-->

Como funciona o mecanismo de attention? #flashcard 
![[Pasted image 20231110100415.png]]
1- O LSTM é rodado até o decoder gerar o output dele
2- É calculada a semelhança das memórias de curto prazo de cada célula do encoder com a memória de curto prazo da célula atual do decoder
![[Pasted image 20231110100147.png]]
3- As semelhanças passam por uma softmax para escalar a distribuição para ficar entre 0 e 1
4- Cada memória de curto prazo é multiplicada por seu valor de semelhança normalizada
5- Todos esses produtos anteriores são somados e colocados em um vetor de input para uma MLP junto com a saída original do decoder
6- A MLP aprende como construir uma palavra a partir disso
![[Pasted image 20231110101318.png]]
7- Esse processo é repetido para cada output do decoder
<!--ID: 1699621980145-->