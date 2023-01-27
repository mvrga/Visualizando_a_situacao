#Qual o nome do jogo melhor avaliado?
select `name`, positive_ratings from steam_table order by positive_ratings desc limit 1; 
#Counter-Strike: Global Offensive	2644404

#Qual o genero do jogo mais caro? 
select `name`, genres, price from steam_table order by price desc limit 1;
#3DCoat 4.8	Animation & Modeling	95.99

#Quantos jogos apenas multiplayer possuem?
select `name`, categories from steam_table where categories = "Multi-player";
#Victoria I Complete	Multi-player
#Sword of the Stars II: Enhanced Edition	Multi-player
#Dungeon-Party	Multi-player
#Jeklynn Heights	Multi-player;

#Qual o jogo com mais conquistas alcançadas?
select `name`, achievements from steam_table order by achievements desc limit 1;
#Tales of Maj'Eyal	1746

#Quais os 10 jogos com mais conquistas alcançadas em ordem descrescente?  
select `name`, achievements from steam_table order by achievements desc limit 10; 
#Tales of Maj'Eyal	1746
#Dofus	1448
#Train Simulator 2019	1165
#PAYDAY 2	1130
#Guns of Icarus Online	849
#Champions Online	709
#Assetto Corsa	709
#Fallen Earth Free2Play	650
#Team Fortress 2	520
#Men of War: Assault Squad 2	490

#Qual a data de lançamento dos jogos no top 3?
select `name`, realease_date from steam_table order by positive_ratings desc limit 3; 
#Counter-Strike: Global Offensive	2012-08-21
#Dota 2	2013-07-09
#Team Fortress 2	2007-10-10