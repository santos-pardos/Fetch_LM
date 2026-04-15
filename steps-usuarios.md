## Usuarios
```
fetch("https://jsonplaceholder.typicode.com/todos/1")
    .then(response => response.json())
    .then(json => console.log(json))

```
```
fetch("https://jsonplaceholder.typicode.com/todos")
    .then(response => response.json())
    .then(json => console.log(json))

```
```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";

console.log(fetch(urlUsuarios));

```

```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";

fetch(urlUsuarios)
    .then( (response) => console.log(response) )

```

```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";


fetch(urlUsuarios)
    .then( (response) => response.json() )
    .then(data=> console.log(data))

```


```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";
const listaUsuarios = document.querySelector("#lista-usuarios");

fetch(urlUsuarios)
    .then( (response) => response.json() )
    .then( (data) => { 
        console.log(data);
    })
```




```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";
const listaUsuarios = document.querySelector("#lista-usuarios");

fetch(urlUsuarios)
    .then( (response) => response.json() )
    .then( (data) => { 
        console.log(data[0]);
    })

```

```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";
const listaUsuarios = document.querySelector("#lista-usuarios");

fetch(urlUsuarios)
    .then( (response) => response.json() )
    .then( (data) => {
        data.forEach(usuario => {
            const li = document.createElement("li");
            li.textContent = usuario.name;
            listaUsuarios.append(li);
        })
    } )

```


```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";
const listaUsuarios = document.querySelector("#lista-usuarios");

fetch(urlUsuarios)
    .then( (response) => response.json() )
    .then( (data) => {
        console.log(data);
        data.forEach(usuario => {
            const li = document.createElement("li");
            li.textContent = usuario.name;
            listaUsuarios.append(li);
        })
    } )
```

```
const urlUsuarios = "https://jsonplaceholder.typicode.com/users";
const listaUsuarios = document.querySelector("#lista-usuarios");

fetch(urlUsuarios)
    .then( (response) => response.json() )
    .then( (data) => {
        console.log(data);
        data.forEach(usuario => {
            const li = document.createElement("li");
            li.innerHTML = usuario.name + "<br>Teléfono: " + usuario.phone;
            listaUsuarios.append(li);
        })
    } )

 ```    
