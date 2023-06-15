# Avaliação para o Mercado Livre
## Atividade 1

Consiste nos arquivos "Atividade 1 - Geral.ipynb" e "Atividade 1 - Sem Nulos.ipynb"
* "Atividade 1 - Geral.ipynb" - Foi uma análise inicial com todas as tuplas, considerando nulos etc.
* "Atividade 1 - Sem Nulos.ipynb" - Uma análise mais rebuscada com filtro de não nulos (promoções que venderam algo)

### Comentários
> Rentabilidade = preço / quantidade
1. Os principais horários de início de promoções são às 01h, 07h e 19h;
2. Os principais horários de término de promoções são às 01h, 07h e 13h;
3. As promoções se iniciam mais nas quinta-feiras e menos aos domingos;
4. O tempo médio de promoções é de 5 horas e 57 minutos, porém com mediana em 6 horas;
5. O tempo máximo de promoções foi de 14 horas e 40 minutos e o menor de 5 minutos;
6. Aproximadamente 80% das promoções são finalizadas no ínicio da hora (no minuto 0);
7. O DOM_DOMAIN_AGG mais vendido foi PHARMACEUTICS, seguido por BEAUTY EQUIPMENT e HOME&DECOR;
8. O DOM_DOMAIN_AGG mais valioso foi PHARMACEUTICS, seguido por MOBILE e ELECTRONICS;
9. DOMAIN_ID mais vendido e valioso foi o MLM-SURGICAL_AND_INDUSTRIAL_MASKS, porém o mais rentável foi o MLM-WASHING_MACHINES seguido por MLM-LIVING_ROOM_SETS;
10. Dos DOMAIN_ID mais vendidos, 4 estão influenciados diretamente pela pandemia, 1º MLM-SURGICAL_AND_INDUSTRIAL_MASKS, 2º MLM-DISPOSABLE_GLOVES, 3º MLM-OXIMETERS e 5º MLM-THERMOMETERS;
11. Os DOM_DOMAIN_AGG mais rentáveis são em 1º WHEELS & TIRES, 2º MOBILE e 3º ELECTRONICS;
12. O freeship teve menor quantidade de vendas, porém com um volume de dinheiro maior, reforçando que a partir de determinado valor, o frete é grátis;
13. Com base no jupyter anterior (Atividade 1 - Geral), 24167 promoções não tiveram vendas.


### Insights

1. A pandemia elevou as vendas dos produtos da classe PHARMACEUTICS com os MLM-SURGICAL_AND_INDUSTRIAL_MASKS, MLM-DISPOSABLE_GLOVES, MLM-OXIMETERS e MLM-THERMOMETERS;
2. Oferecer frete grátis tem uma maior quantidade de produtos rentáveis;
3. Raramente inicia-se uma promoção em hora útil (8h às 18h), sendo que o comerciante prefere iniciar ou antes do cliente sair de casa ou após o mesmo retornar para sua respectiva residência
> Com base no jupyter anterior (Atividade 1 - Geral);
4. Nesse período o maior aproveitamento de promoções do DOM_DOMAIN_AGG foram de PHARMACEUTICS, BEAUTY EQUIPMENT, SUPLEMENTS e ANTIQUES & HOBBIES. Todos acima de 60% de aproveitamento de promoções, podendo criar um grupo separado para eles (Criando um banner de "saúde" na tela principal);
5. O DOM_DOMAIN_AGG Agro só teve uma única promoção e mesmo assim não teve nenhuma venda.

## Atividade 2
Consiste nos arquivos "Atividade 2.ipynb" e "atividade2_output.csv"
* "Atividade 2.ipynb" - Análise e preparação do output de comparação entre todos os objetos do "items_titles_test.csv"
* "atividade2_output.csv" - Output com a matrix de comparação de similaridade entre todos os objetos

### Output
* https://we.tl/t-GnfcqiRDEi

## Atividade 3
Consiste no arquivo "Atividade 3.ipynb"
* "Atividade 3.ipynb" - Análise e previsão utilizando alguns algoritmos do tipo MLP, KNN, SVC, Tree e XGBoost. Como foi por teste, os modelos não foram salvos e o output mostra como matriz de confusão e classification report.

### Comentários
1. A classe de falha está totalmente desbalanceada com apenas 8% dos dados tem falha;
  1.1. O recomendado é balancear ou utilizar uma técnica de data augmentation;
2. O algoritmo de Árvore (Tree) deu um resultado melhor, porém esse resultado foi apenas com dois objetos classificados como 'falha' que ele conseguiu definir corretamente, utilizando a ideia de lookback. Outro que conseguiu identificar apenas uma instância foi o XGboost sem lookback.

### Próximos passo:
1. Implementar RNN para realizar a classificação com base no lookback (GRU, LSTM etc.).
