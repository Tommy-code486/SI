# Secteur de la construction - *Gestion de construction d'une maison* 

## Donnee d'entree :
- Le budget total du client incluant une somme d'argent en plus pour les imprévus.
- Donnee geometrique :
    - Les mesures recommander du client (par exemple : Le client veut construire une maison sur une terrain de 30 m²)
    - Ou se situe la maison
    - Combien d'etage veut le client       
- Ressources materiels necessaire :
    - Les nombres total de materiel utilise (ciment,gravier,fer,brique)
    - Choisir le nombre d'ouvriers par métier (chef, maçon, aide)  
    - Le nombre d'ouvrier necessaire pour la contruction
- Plannning du travail 
    - Duree de construction imposer par le client

## Dispositif d'entree :
- Formulaire web
- Fichier (.pdf,.csv,.xlsx)


## Traitement (Logique metier) :
- Calcul budget de la construction : 
    - Transformer les données géométriques (m2, nombre d'étages) en quantités réelles de matériaux (sacs de ciment, kilos de fer)
        - Formule : <span style=color:blue>*Quantite totale = (Mesures geometriques × Coefficient technique de resistance)*</span>
    - Le client impose son budget pour la construction de sa maison et nous on doit calculer les prix du brique et toutes les restes pour la construction (par exemple : les prix du fer ,les ciments...)
        - Formule : <span style=color:blue>*∑(Quantite de materiaux × Prix unitaire)*</span>
- Étude de faisabilité :
    - Connaitre si le budget imposer par le logiciel depasse le budget du client
        - Formule : <span style=color:blue>*Budget du logiciel - Depense total*</span>
    - Il faut aussi calculer les salaires des ouvrier
        - Imposer les salaire des ouvrier en fonction de leur travail
        - Formule : ** 
    - Calculer automatiquement le coût total en fonction des salaires de chacun et augmenter le prix si le client veut finir les travaux plus vite.
- Gestion des risques : 
    - Inclure des algorithmes pour anticiper les dérapages budgétaires, les retards de livraison de matériaux

## Sortie :
- Un document qui prouve que la maison a été construite exactement selon les plans et les normes de sécurité
- Les depenses total pour la construction
- Reporting et Tableaux de bord : 
    - Rapports sur l'avancement du chantier, comparaison entre budget prévu et dépenses réelles

## Dispositif de sortie :
- Une fichier (excel,pdf,docx)
- Une page web