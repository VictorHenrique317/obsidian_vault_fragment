TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
06/10/2023 - 10:23
Relações: [[Bag of words]]
# Flashcards

Oque é o word2vec? #flashcard 
Uma rede neural com uma camada de entrada. uma oculta e uma de saída
O objetivo é criar embeddings das palavras com base nas palavras ao redor
<!--ID: 1696849854058-->


Que tipos de implementações temos do word2vec? #flashcard 
CBOW (Continuous bag of words)
Skip-gram
<!--ID: 1696849854435-->


Como funciona a implementação CBOW do word2vec? #flashcard 
1- Da uma frase, por exemplo "O cachorro correu atrás do gato" e uma janela de contexto,
por exemplo 2, criamos todas as combinações possíveis de contexto-palavra
![[Pasted image 20231006103124.png]]
2- Para cada um desses dados de treino (contexto) calcular o bag of words do contexto
que é dado como entrada para a rede neural
3- A rede gera uma distribuição de probabilidade que indica qual é a palavra mais provável
de ser a palavra alvo dado o contexto
4- Se compara essa saída com o one-hot-encoder da palavra alvo para corrigir os pesos
<!--ID: 1696849854801-->


Como funciona a implementação Skip-gram do word2vec? #flashcard 
1- Da uma frase, por exemplo "O cachorro correu atrás do gato" e uma janela de contexto,
por exemplo 2, criamos todas as combinações possíveis de palavra-contexto
![[Pasted image 20231006103933.png]]
2- Para cada um desses dados de treino (palavra alvo) projetar o one-hot-encoder em um vetor de
dimensionalidade menor e usar isso como entrada para a rede
3- A rede gera uma distribuição de probabilidade que representa as palavras mais prováveis de
estarem no contexto
4- Se compara essa saída com a soma dos one-hot-encoders do contexto para corrigir os pesos
<!--ID: 1696849854988-->


Quais as vantagens do word2vec? #flashcard 
Ele gera bons embeddings para serem usados em redes neurais
<!--ID: 1696849855067-->


Qual o problema do word2vec? #flashcard 
A semântica das palavras é definida totalmente pelo fato delas estarem perto ou não então temos que:
Palavras com significado contrário são ditas como sendo muito parecidas
Biases do mundo real são refletidos se uma palavra é repetida erroneamente com outras
Uma palavra pode ter múltiplos significados diferentes
<!--ID: 1696849855167-->


