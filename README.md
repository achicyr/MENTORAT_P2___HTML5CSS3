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


# nextStep:
créer tous les balises et contenus html demandés dans le premier exercice du cours, at: https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/6725196-entrainez-vous-en-structurant-votre-cv