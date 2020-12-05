# Trabalho Prático 2 - Teoria dos Grafos

# Componente
- Paulo Ricardo Gomes Gois Silva

# Tutorial
- Assim que o programa for iniciado, ele pedirá para que o usuário insira para qual perfil de usuário ele deseja recomendações de filmes (variando de 1-610 do banco de dados)
- Em seguida será solicidado para que o usuário insira quantas recomendações deseja obter
- Após inseridos os dados solicitados, o programa levará alguns segundos para processar e recomendar os melhores filmes baseado no perfil escolhido

# Como o programa determina quais filmes são recomendados?
- O código foi desenvolvido de forma que seja coletado os ratings do usuário escolhido e comparado com os demais usuários a fim de criar um perfil de semelhança
- Foi considerado que os usuários eram os vértices do grafo e que o grau de semelhança entre o usuário escolhido e outro seja o peso da aresta que os liga
- Após isso o programa utiliza o algoritmo de ordenação quick sort para ordenar de forma decrescente a lista que armazena o grau de semelhança
- O programa então busca, a partir do usuário que tem os interesses mais semelhantes, filmes que o usuário 1 ainda não tenha assistido e que o usuário 2 tenha dado nota 5 (É possivel alterar a nota necessária para a recomendação a partir de uma linha de código)
- Por fim, o programa imprime uma tabela contendo o id, nome e gênero dos filmes em ordem do mais para o menos recomendado
