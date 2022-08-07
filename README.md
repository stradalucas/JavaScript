# JavaScript

### Fetch JSON
fetch('https://api.github.com/users/manishmshiva')
    // Exito
    .then(response => response.json())  // convertir a json
    .then(json => console.log(json))    //imprimir los datos en la consola
    .catch(err => console.log('Solicitud fallida', err)); // Capturar errores
   
### Fetch XML
fetch('https://codetogo.io/api/users.xml')
  .then(response => response.text())
  .then(data => {
    const parser = new DOMParser();
    const xml = parser.parseFromString(data, "application/xml");
    console.log(xml);
  })
  .catch(console.error);
  
  
  const request = async (url) => {
  const response = await fetch(url);
  if (!response.ok)
    throw new Error("WARN", response.status);
  const data = await response.text();
  return data;
}

const resultOk = await request("/robots.txt");
const resultError = await request("/nonExistentFile.txt");


let str = "42";
Number.parseInt(str, 10); 

let number = 42
number.toString()

Una nota importante sobre const es que no crea una constante o un valor inmutable. Esto se explicará a fondo una vez que aprendamos sobre matrices y objetos. Lo que necesita saber, por ahora, es que solo puede usar el signo igual una vez, pero aún puede cambiar elementos dentro de una matriz u objeto.

