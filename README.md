# banco_oscar
respondendo algumas questões sobre uma tabela dos indicados ao oscar criada com banco de dados

Este repositório contém uma série de consultas e operações SQL para trabalhar com dados relacionados ao Oscar. As atividades abrangem desde informações sobre indicados e vencedores

Atividades para trabalhar com o Oscar:

1- Quantas vezes Natalie Portman foi indicada ao Oscar?

comando:
SELECT COUNT(*) FROM filmes WHERE nome_do_indicado = 'Natalie Portman';

resposta: 3 vezes

2- Quantos Oscars Natalie Portman ganhou?

comando: 
SELECT COUNT(*) 
FROM filmes 
WHERE vencedor = 'Sim' AND nome_do_indicado = 'Natalie Portman';

resposta: 1 vez

3- Amy Adams já ganhou algum Oscar?

comando: 
SELECT COUNT(*) 
FROM filmes 
WHERE vencedor = 'Sim' AND nome_do_indicado = 'Amy Adams';

resposta: Não

4- A série de filmes Toy Story ganhou um Oscar em quais anos?

comando:
SELECT ano_filmagem FROM filmes WHERE nome_filme = 'Toy Story';

resposta: 1996

5- A partir de que ano que a categoria "Actress" deixa de existir? 

resposta: a categoria "Actress" nunca deixou de existir. Portanto, não há um ano específico para isso.

6- O primeiro Oscar para melhor Atriz foi para quem? Em que ano?



7- Na coluna/campo "Vencedor", altere todos os valores com "Sim" para 1 e todos os valores "Não" para 0.

8- Em qual edição do Oscar "Crash" ganhou o prêmio principal?

9- Bom... dê um Oscar para um filme que merece muito, mas não ganhou.

10- O filme Central do Brasil aparece no Oscar?

11- Inclua no banco 3 filmes que nunca foram nem nomeados ao Oscar, mas que merecem ser. 

14 - Pensando no ano em que você nasceu: Qual foi o Oscar de melhor filme, Melhor Atriz e Melhor Diretor?
