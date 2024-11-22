TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
20/10/2023 - 09:45
Relações: [[Seq2Seq com attention]], [[Transformer]]
# Flashcards

Oque é sequence2sequence? #flashcard 
Uma rede neural que usa LSTM's para produzir uma sequência (texto) a partir de outra.
<!--ID: 1697806029844-->

Como funciona o seq2seq depois de treinado? #flashcard 
![[Pasted image 20231020100102.png]]
1 - O encoder joga os embeddings na primeira camada da LSTM que são propagados para as outras e para frente
2 - As memórias finais de todas as camadas (vetores de contexto) são a entrada do decoder
3 - Baseado nos vetores de contexto e no SOS (start of sentence) o decoder prevê a próxima palavra ao passar os vetores pela LSTM e o resultado disso pela rede neural
4 - A palavra prevista é usada como input para o nível seguinte que irá prever a palavra seguinte
<!--ID: 1697807143018-->

Como treinar o seq2seq? #flashcard 
![[Pasted image 20231020100102.png]]
1 - O encoder joga os embeddings na primeira camada da LSTM que são propagados para as outras e para frente
2 - As memórias finais de todas as camadas (vetores de contexto) são a entrada do decoder
3 - Baseado nos vetores de contexto e no SOS (start of sentence) o decoder prevê a próxima palavra ao passar os vetores pela LSTM e o resultado disso pela rede neural
4 - A palavra prevista é comparada com a verdadeira para se atualizar os pesos com backpropagation
5 - A palavra verdadeira é usada como input para o nível seguinte que irá prever a palavra seguinte
<!--ID: 1697807268043-->

Qual é o problema do seq2seq? #flashcard 
A qualidade dele diminui muito com frases um pouco maiores pois ele esquece das palavras iniciais
<!--ID: 1699621166821-->
