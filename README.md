# my-egarden
Jarding virtuel


# Start

    docker-compose up -d
    go to https://localhost:8443/    

# Dev Tools

Sync DB with Entities: 

    docker-compose exec php bin/console doctrine:schema:update --force

# Reference

Rotation des cultures: https://www.ecoconso.be/fr/content/comment-pratiquer-la-rotation-des-cultures-au-potager

Démarrage a 10m2

# Season

    - spring
    - summer
    - falls
    - winter
    
## Caractèristiques d’une saison
 
    - température
    - taux d’ensoleillement
    - taux d’humidité      
    - taux de pluie
    - force du vent
    - direction du vent     ¼¼¼¼¼¼−−−−−−


# Plot (Parcelle)

- State (état du sol)
    - Fallow land: Jachère
    
- Quality (qualité du sol)
    - pH
    - niveau nutritif

- Water % (pourcentage d’eau présent)




# API

## Plot
POST /plot: 

Request

    - position {x,y}

Response

    - position {x,y}
    - state
    - createdAt
    - updatedAt
