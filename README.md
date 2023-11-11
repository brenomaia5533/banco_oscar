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

comando: select * from filmes;

resposta: Janet Gaynor, em 1928


7- Em qual edição do Oscar "Crash" ganhou o prêmio principal?

comando: SELECT ano_filmagem FROM filmes WHERE nome_filme = 'Crash' 
SELECT edicao_cerimonia FROM filmes WHERE ano_cerimonia = '2005' 

resposta: edição 78

8- Bom... dê um Oscar para um filme que merece muito, mas não ganhou.

comando: 
INSERT INTO filmes (id_filme, ano_filmagem, ano_cerimonia, edicao_cerimonia, nome_filme, vencedor) VALUES ('10396', '1976', '2023','93', 'Taxi Driver', 'Sim' );


9- O filme Central do Brasil aparece no Oscar?

comando:
SELECT COUNT(*) FROM filmes WHERE nome_filme = 'Central do Brasil';

resposta: Não

10- Inclua no banco 3 filmes que nunca foram nem nomeados ao Oscar, mas que merecem ser. 

comando: 
INSERT INTO filmes (nome_filme, ano_filmagem, vencedor) VALUES 
('Dr.fantastico', '1964', 'Não'),
('Need for speed', '2014', 'Não'),
('Kung fu panda 4', '2024', 'Não');



