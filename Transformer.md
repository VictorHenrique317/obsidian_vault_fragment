TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
22/11/2023 - 09:24
Relações: [[Large Language Model]]
# Flashcards

Oque é positional encoding? #flashcard 
Uma técnica utilizada em transformers para conservar a ordem das
palavras em um sentença dentro do próprio embedding
<!--ID: 1700656126061-->

Como funciona o positional encoding? #flashcard 
![[Pasted image 20231122093213.png]]
![[Pasted image 20231122093014.png]]
Os valores dos embeddings de cada palavra são multiplicados pelo valor de seno ou cosseno 
que está na posição da palavra 
<!--ID: 1700656423572-->

Oque é self attention? #flashcard 
![[Pasted image 20231122093708.png]]
![[Pasted image 20231122093714.png]]
![[Pasted image 20231122093732.png]]
Uma técnica utilizada em transformers que calcula a similaridade de cada palavra em relação a si
mesma e as outras
<!--ID: 1700656649897-->

Como o self attention é implementado no encoder de um transformer? #flashcard 
![[Pasted image 20231122095051.png]]
As similaridades do query da palavra atual em relação as keys da palavra atual e da anterior são calculadas e passadas por uma softmax no final que dá a importância de cada palavra no self-attention da atual
![[Pasted image 20231122095421.png]]
Valores aprendidos a partir dos positional encodings originais são escalados pelo output da softmax
para obter os valores de self-attention finais
<!--ID: 1700657020773-->

Oque são residual connections em um transformer e para que servem? #flashcard 
![[Pasted image 20231124082023.png]]
A soma dos positional encodings depois do calculo de self attention
Servem para minimizar a perda de gradiente
<!--ID: 1700824866498-->

Como o self attention é implementado no decoder de um transformer? #flashcard 
Da mesma forma que no encoder, só que comparando a palavra sendo decodificada com
as que já foram decodificadas
<!--ID: 1700825116422-->

Como funciona o encoder-decoder attention em um transformer? #flashcard 
![[Pasted image 20231124082748.png]]
A palavra sendo decodificada atualmente é comparada com as palavras do encoder da mesma forma
que é feito no self attention
<!--ID: 1700825307047-->

Como funciona um transformer? #flashcard 
![[Pasted image 20231124082947.png]]
1 - Depois de calculado o encoder-decoder attention o resultado serve como input para uma rede neural
2 - A próxima palavra é decodificada seguindo os passos de self attention do decoder, encoder-decoder attention e rede neural normalmente
<!--ID: 1700825510074-->

Qual é a principal vantagem do transformer em relação a LSTM's? #flashcard 
Ele é altamente paralelizável, oque possibilita a utilização de grandes volumes de dados
<!--ID: 1700825764697-->

De que formas podemos fazer o fine tunning de transformers pré-treinados? #flashcard 
![[Pasted image 20231206083655.png]]
<!--ID: 1701862802760-->

Que tipos de transformer que existem? #flashcard 
Encoder only, Decoder only e Encoder-Decode
<!--ID: 1701862358525-->

Para que servem transformers encoder only? #flashcard 
![[Pasted image 20231206083426.png]]
Eles tem uma visão do texto inteiro, logo são bons para tarefas de classificação
no geral
<!--ID: 1701862470160-->

Como treinar transformers encoder only? #flashcard 
![[Pasted image 20231206083554.png]]
Escondendo (mascarando) palavras do input para prever-lás
<!--ID: 1701862802866-->

Para que servem transformers encoder-decoder? #flashcard 
![[Pasted image 20231206083906.png]]
![[Pasted image 20231206084311.png]]
Modelagem de linguagem
<!--ID: 1701862802914-->

Para que servem transformers decoder only? #flashcard 
![[Pasted image 20231206083959.png]]
Geração de texto
<!--ID: 1701862802953-->

