let nombreUsuario = (prompt("Ingrese su nombre"));
{ alert('Bienvenid@')}
function verNombreUsuario() {

    console.log('Bienvenid@', nombreUsuario)

   
}

function creoID() { return parseInt(Math.random() * 1000) }


const productos = [ 'Cat Chow','Dogui','Pro PLan','Royal Canin','Old Prince','Pedigree','Balanced','Whiskas','Eukanuba'
    
]
function recorrerProductos() {
   
    productos.forEach(elemento => {
        console.table(elemento)
    })
}

const selectProductos = document.querySelector("select")
console.log(selectProductos)



function cargaArrayProductos() {
    productos.sort ()


    productos.forEach (producto => {
        selectProductos.innerHTML += `<option value="">${producto}</option>`
       
    })
}

console.log(productos)
console.log(productos.length)
console.table(productos)

for (let index = 0; index < 9; index++) {
    alert(productos[index]);

}

for (let producto of productos) { 
    
    console.table(producto)

}

function encontrarProducto() {
    let prod = prompt("Ingresa el producto a buscar:")

        const resultado = productos.find(producto => producto === prod)
         console.log(resultado)
         alert ('Tenemos Stock!')
         
         
}




recorrerProductos()
verNombreUsuario()
encontrarProducto()
creoID()
cargaArrayProductos()
