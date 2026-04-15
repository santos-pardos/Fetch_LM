## Pokemon
(borrar console log de usuario)
```
fetch("https://pokeapi.co/api/v2/pokemon")
    .then(response => response.json())
    .then(data => console.log(data))
```
```
fetch("https://pokeapi.co/api/v2/pokemon")
    .then(response => response.json())
    .then(data => console.log(data.results))
```

```

const listaPokemon = document.querySelector("#lista-pokemon");

fetch("https://pokeapi.co/api/v2/pokemon")
    .then(response => response.json())
    .then(data => {
        const pokemons = data.results;

        pokemons.forEach(pokemon => {
            const li = document.createElement("li");
            li.innerText = pokemon.name;
            listaPokemon.append(li);
        });
    })

```

```

const listaPokemon = document.querySelector("#lista-pokemon");

fetch("https://pokeapi.co/api/v2/pokemon")
    .then(response => response.json())
    .then(data => {
        const pokemons = data.results;
        console.log(pokemons);
        pokemons.forEach(pokemon => {
            const li = document.createElement("li");
            li.innerText = pokemon.name;
            listaPokemon.append(li);
        });
    })

```
