# 2) actions:
    - écrire la représentation de contenu html à l'aide d'emmet
    - une fois compris comment xa marche et le contenu html généré, veiller à garder une trace de cette "commande emmet" en tant que commentaire dans votre fichier

    ===> on construit une règle emmet de la manière suivante:
    nom_balise{contenu textutelle}>balise_enfant[attribut0="value_attribut0" attribut1="value_attribut1"]{text}+balise_frere_ou_balise_adjascente>(li>a{lien ancre})*3

    ex: header{text exemple}>h1[class="jajouteUneClass"]{JE SUIS UNE GROS TITRE}+(ul>(li>a)*3{lien ancre})+p{j'ai plus rien à redire...}
    ===>>> ce qui veut dire:
    créer un balise header contenant le text "text exemple" et ayant trois enfant: 
    - une balise de titre h1 contenant "JE SUIS UNE GROS TITRE"
    - une liste contenant trois ancres  avec écrit "lien ancre" dedans
    - et une balise p contenant le texte "j'ai plus rien à redire..."
    
## nextStep:
    - quand on code vaut mieux y aller par étapes et ne pas tenter de tout coder d'une traite (xa ne marche pas souvent et c'est très chronophage in fine, l'organisation est maître dans ce métier!!)
    - on a coder le header => codons le reste maintenant ! let's ocde the rest !
    avec emmet, générer le reste du document (3 sections avec titre et commentare à l'intérieur)


# 1)  actions:
    - créer le fichier style.css (utiliser le panneau "explorer" de vscode pour créer votre fichier)
    - "link" => emmet   ===>>>   dans le <head/>, créer une balise link pointant vers le fichier style.css
    - ajouter une règle css dans style.css (sur la balise <body/> par exemple)
    ===> on contruit une règle css de la manière suivante:
    selection_de_la_balise{
        rule-type: rule value;
        rule-type: rule value;
        rule-type: rule value;
        ....
    }
    ex: 
    body>header p~span+i{
        border:solid;
        box-shadow: 0 0 10px 1px inset;
    }
    ===>>> ce qui veut dire:
    -sélectionner la balise i, frère directe d'une balise span, elle-même frère adjascente d'une balise p , balise p se trouvant à l'interieur de la balise header enfant direct de la balise body,
    - puis lui rajouter instructions css se situants entre les accolades


## nextStep:
créer tous les balises et contenus html demandés dans le premier exercice du cours, at: https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/6725196-entrainez-vous-en-structurant-votre-cv