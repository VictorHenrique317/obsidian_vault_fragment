TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
06/10/2023 - 10:52
Relações:
# Flashcards

Oque é uma ConvNet? #flashcard 
É uma rede neural convolucional de texto utilizada para classificar frases inteiras
<!--ID: 1696849857653-->


Como funciona uma ConvNet? #flashcard 
1-Cria um filtro aleatório que se move sobre as palavras da frase calculando a convolução
![[Pasted image 20231006111536.png]]
![[Pasted image 20231006111634.png]]
2-Se faz isso com múltiplos filtros de tamanho variado
![[Pasted image 20231006111655.png]]
3-Fazer o pooling das viagens de cada filtro
![[Pasted image 20231006111832.png]]
4-Se concatena os resultados dos poolings, e normaliza com uma softmax. Por fim dá para a rede neural como input, ela irá corrigir os filtros e pesos com base na categoria final
![[Pasted image 20231006112004.png]]
<!--ID: 1696849857730-->
