TARGET DECK: Unused::Ciência da computação::3º Semestre::NLP
06/10/2023 - 10:54
Relações: [[Embeddings]]
# Flashcards

Oque é o WMD #flashcard 
Word Mover Distance, é uma forma de comparar dois documentos ou sentenças
<!--ID: 1696849855250-->


Como funciona o WMD? #flashcard 
![[Pasted image 20231006105717.png]]
0- Pré-processamento do documento.
1-Dado um embedding, para cada palavra no documento 1 procurar a palavra de menor distância
no documento 2
2- Fazer isso para todas as palavras do documento 1 e somar essas distâncias mínimas
3- A distância dos dois documentos é o valor desse somatório
<!--ID: 1696849855328-->


Qual é o problema do WMD? #flashcard 
O custo dele é muito alto
<!--ID: 1696849855421-->
