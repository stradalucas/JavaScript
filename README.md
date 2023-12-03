# JavaScript

### Fetch JSON
fetch('https://api.github.com/users/manishmshiva')
    // Exito
    .then(response => response.json())  // convertir a json
    .then(json => console.log(json))    //imprimir los datos en la consola
    .catch(err => console.log('Solicitud fallida', err)); // Capturar errores

### Global Event
document.body.addEventListener("click", ev => {
    const closeBtn = ev.target.closest(".closeBtn")
    if(closeBtn){
    
        const closeTarget = closeBtn.getAtributte("closeTraget")
        document.querySelector("#closeTarget)
    }
})
<span closeTarget="createUserContainer" class="closeBtn"></span>
