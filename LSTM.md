TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
18/10/2023 - 08:42
Relações: [[Seq2Seq]]
# Flashcards

Oque é uma LSTM? #flashcard 
Long Short Term Memory, um tipo de rede neural recorrente que foi feita
para solucionar o problema de explosão/desaparecimento do gradiente das redes recorrentes
clássicas
<!--ID: 1697629414944-->

Como funciona uma LSTM? #flashcard 
![[Pasted image 20231020093818.png]]
Se encadeia uma célula LSTM para cada exemplo que se deseja lembrar, no final coloca uma rede neural
<!--ID: 1697805501969-->

Como funciona uma célula LSTM? #flashcard 
![[Pasted image 20231020094006.png]]
![[Pasted image 20231020094323.png]]
1 - O primeiro bloco define o quanto da memória de longo prazo se vai manter
2 - O segundo e terceiro definem o quanto do exemplo atual e da memória de curto prazo serão incorporados na memória de longo prazo
3 - Os dois últimos definem o output final, levando em consideração as duas memórias
<!--ID: 1697805726844-->
