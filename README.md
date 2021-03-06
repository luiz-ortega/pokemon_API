# Pokedex API

A dashboard for add, edit, remove and see details of pokemons made with [NodeJS](https://nodejs.org/en/). 

The frontend for it can be found [here](https://github.com/luiz-ortega/pokemon_client).

## Project setup
```
npm install
```

## Configure the database credentials in database.js file
```
src/config/database.js
````

## Run migrations
```
npx sequelize db:migrate 
````

### Compiles and hot-reloads for development
```
npm run dev
```

### Methods

#### For Pokemon:
- GET    - /pokemons ------> to list pokemons
- DELETE - pokemons/:id ---> to delete pokemons
- PUT    - /pokemons/:id --> to update pokemons
- POST   - /pokemons ------> to store pokemons
  - Body example for PUT and POST:
```
{
  "name": "Bullbasaur",
  "pokedex_number": 1,
  "img_name": "",
  "evolved": true,
  "cross_gen": false,
  "stat_total": 123,
  "atk": 123,
  "def": 123,
  "sta": 123,
  "spawns": true,
  "regional": true,
  "shiny": true,
  "nest": true,
  "new": true,
  "not_gettable": true,
  "future_evolve": true,
  "hundred_percent_cp_40": 123,
  "hundred_percent_cp_39": 123,
  "evolution_stage_id": 5,
  "family_id": null,
  "raidable_id": 2,
  "hatchable_id": 4,
  "aquireable_id": 3,
  "legendary_id":  2,
  "generation_id": 1,
  "type_id_1": 1,
  "type_id_2": 5,
  "weather_id_1": 1,
  "weather_id_2": 3
}
```
##### For selects:
- GET - /aquireables -----------> to list Aquireables
- GET - /evolution_stages ------> to list Evolution Stages
- GET - /generations -----------> to list Generations
- GET - /hatchables ------------> to list Hatchables
- GET - /legendaries -----------> to list Legendaries
- GET - /raidables -------------> to list Raidables
- GET - /types -----------------> to list Types
- GET - /weathers --------------> to list Weathers


## License
[MIT](https://choosealicense.com/licenses/mit/)


