var myRegex = /test/;
myRegex.test(stringATester)




pour rendre insensible a la casse 
var myRegex = /tesT/i;






operateur ou |





debut et fin de chaine
/^raclette savoyarde$/




regex d adresse email 
/^[a-z0-9._-]+@[a-z0-9._-]+\.[a-z]{2,6}$/





objet RegExp 
var myRegex1 = /^Raclette$/i;
var myRegex2 = new RegExp("^Raclette$", "i");





Deux methodes de RegExp test et exec 
exec comme group en java





Les parentheses capturantes sont comme java group(1)
==> var reg = new RegExp();
reg.exec();
reg.$1 equivau a group(1)





Les parentheses non capturantes 
(? 





non greedy-search
exemple : (.+) cherche le max possible
(.+?) cherche le minimum qui satisfait la cond





option g comme recherchecher plusieurs fois 
'baba a abbaaba babab dio'.replace(/baba/g,'mimi');
comme replaceAll en java





pour echaper $ dans une capture on ecrit $$




les methodes de l'objet String 
search() pareil k indexof mais avec regex
match() pareil k search mais retourne un tableau d plusieurs match

