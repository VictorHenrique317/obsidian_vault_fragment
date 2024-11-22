TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
22/09/2023 - 10:51
Relações:
# Flashcards

Quais são os desafios que a linguagem traz para o aprendizado de máquina? #flashcard 
Ela é:
Discreta (a distância entre palavras não é obvia)
Composicional (uma palavra pode mudar totalmente o sentido)
Esparsa (existem muitas combinações de palavras)
<!--ID: 1695390759065-->

Oque é um token? #flashcard 
Uma unidade parecida com as palavras, mas tokens podem ser
case sensitive ou per caracteres especiais como ponto e virgula
<!--ID: 1695390883407-->

Oque é um vocabulário? #flashcard 
Um conjunto de todos os tokens conhecidos
<!--ID: 1695390925782-->

Como lidar com tokens fora do vocabulário? #flashcard 
Com um token especial (UNK) para tokens que não estão no vocabulário.
<!--ID: 1695391017380-->

Qual é a principal maneira de combater a perda de gradiente? #flashcard 
Usando funções de ativação não lineares como a RELU
<!--ID: 1695391145817-->

Como transformar o output de uma rede neural em uma distribuição de probabilidade? #flashcard 
Usando a função softmax na saída.
<!--ID: 1695391280097-->

Como a temperatura do softmax afeta a distribuição de probabilidade resultante? #flashcard 
Altas temperaturas geram distribuições mais "distribuídas"
Baixas temperaturas geram distribuições mais concentradas em um valor.
<!--ID: 1695391381035-->

Que função de perda é usada para problemas de classificação binária? #flashcard 
A binary-cross-entropy (logloss)
<!--ID: 1695391428441-->

Que função de perda é usada para problemas de classificação múltipla? #flashcard 
A categorical-cross-entropy
<!--ID: 1695391459939-->

Oque é one-hot-encoding? #flashcard 
![[Pasted image 20231006101341.png]]
Representar uma palavra através de um vetor binário de uma entrada 1
<!--ID: 1696849858202-->


Quais utilidades possuem a função de ativação softmax?  #flashcard 
Ela pode ser usada para gerar uma distribuição de probabilidade a partir de um valor
E também para normalizar as saídas de diferentes neurônios para um range de valores
<!--ID: 1696849858282-->
