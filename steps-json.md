## JSON

```
fetch("./js/productos.json")
    .then(response => console.log(response))
 ```


```
fetch("./js/productos.json")
    .then(response => response.json())
    .then(data => {
	console.log(data);
    })

```
```
const listaProductos = document.querySelector("#lista-productos");

fetch("./js/productos.json")
    .then(response => response.json())
    .then(data => {
        data.forEach(producto => {
       	    const li = document.createElement("li");
       	    li.innerText = producto.nombre + " - $" + producto.precio;
       	    listaProductos.append(li);
        });  
    })
```


```
const listaProductos = document.querySelector("#lista-productos");

fetch("./js/productos.json")
    .then(response => response.json())
    .then(data => {
        mostrarProductos(data);
    })

function mostrarProductos(productos) {
    productos.forEach(producto => {
        const li = document.createElement("li");
        li.innerText = producto.nombre + " - $" + producto.precio;
        listaProductos.append(li);
    });
}
```
