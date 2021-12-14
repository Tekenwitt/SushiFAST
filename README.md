# SushiFAST
Sushifast est une application web, qui a pour but de saisir des commandes et les envoyer

--- 
## Technologies 
NodeJS, Angular, MongoDB

---
## Diagramme UserCase
![image](https://user-images.githubusercontent.com/73754457/146093904-e98224b2-93d3-4b7d-a3a2-756bfdc8db72.png)

Dans ce diagramme ont peu y voir les différentes intéraction entre l'operateur(serveur) et le  système (l'application SushiFAST ) mais aussi avec l'api. 
Ce diagramme sert à comprendre les divers possibilités d'utilisation de l'application.

## Diagramme 3 tiers 
![image](https://user-images.githubusercontent.com/73754457/146094250-dcaa3db5-5317-4cae-becb-a1ce57f4d417.png)
Dans ce diagramme nous voyons clairement les 3 tiers utilisé par l'application 
Le premier étant le client c'est l'application crée à l'aide d'angular
Le second étant le serveur on se sert de l'api qui envoie les requetes a la base de donnée qui est le troisième et dernier tiers. 
Cette derniere va lui répondre en retournant les JSON.

---

## Structure JSON 
interface BoxesCommande {
    nom: string,
    quantite: number,
    prix: number
}
export interface Commande {
    client: string,
    composition: BoxeCommande[],
    prixTotal: number
    }`
