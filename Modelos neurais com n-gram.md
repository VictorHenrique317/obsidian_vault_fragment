TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
06/10/2023 - 10:21
Relações:
# Flashcards

Oque são modelos de linguagem neural n-gram? #flashcard 
Uma rede neural que aprende embeddings para o vocabulário e usa n-grams para prever a próxima palavra
<!--ID: 1696849856964-->


Como usar n-grams em um modelo de linguagem neural? #flashcard 
![[Pasted image 20230922113247.png]]
Organizar os one-hot-encoders em linhas de uma matriz
Para cada one-hot-encoder criar uma linha com $d$ (hiperparâmetro) dimensões em outra matriz (matriz de embedding)
Aleatorizar os valores na matriz de embedding, esses serão aprendidos
Selecionar as linhas do embedding relacionadas as $k$ palavras anteriores (k-grams) através das lookup tables
Concatenar essas linhas selecionadas do embedding na etapa de concat
Usar o vetor 1D resultante como a entrada (features) para a rede neural
Os labels corretos são as próprias próximas palavras que estão no texto (self-training)
O output é uma distribuição de probabilidade
<!--ID: 1695393240876-->

Qual é o principal problema de modelos de linguagem neural que usam n-grams? #flashcard 
O desempenho deles é ruim.
<!--ID: 1695393595877-->