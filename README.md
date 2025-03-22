# ponderada_traducao_automatica

## 9.5.7.1
Quando alteramos o valor do argumento num_examples na função load_data_nmt, isso impacta diretamente os tamanhos dos vocabulários tanto do idioma de origem quanto do idioma de destino. Basicamente, quanto maior o número de exemplos carregados, maior tende a ser o número de palavras únicas presentes nos dados, resultando em um vocabulário mais extenso. Isso acontece porque mais sentenças trazem mais diversidade de palavras e expressões, enquanto um número reduzido de exemplos limita a variedade de palavras que aparecem, diminuindo assim o tamanho do vocabulário.

## 9.5.7.2
A tokenização em nível de palavra para idiomas como chinês e japonês não é uma boa ideia. Isso se deve ao fato de que esses idiomas não utilizam espaços para separar palavras, como acontece em português ou inglês. Sendo assim, identificar os limites entre uma palavra e outra é um processo bem mais complexo e sujeito a erros. Por conta disso, usar tokenização em nível de caractere costuma ser mais eficiente nesses casos, já que cada caractere possui um significado próprio e o vocabulário gerado é menor e mais consistente. Outra alternativa bastante utilizada é a tokenização em subwords, como o BPE, que também ajuda a capturar padrões sem depender da segmentação explícita de palavras.







