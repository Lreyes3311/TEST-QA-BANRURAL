A continuacion las lineas de codigo que fueron corregidas para el buen funcionamiento del sistema:

  let randomNumber = Math.floor(Math.random() * 100) + 1; <!--Error, lo correcto es: randomNumber = Math.floor(Math.random() * 100) + 1-->

  const ATTEMPS = 10; <!--El numero permitido a ingresar es 10 -->

  const lowOrHi = document.querySelector('.lowOrHi'); <!--Faltaba el punto-->


    let userGuess = parseInt(guessField.value); <!--Convertir userGuess a numero compara-->


    if(userGuess == randomNumber) { <!--En este if va la condiciona de igualar el numero random a resultado exitoso-->

      lastResult.style.backgroundColor = 'green'; <!--Se cambio el color correcto que es el verde -->     

    } else if(guessCount === ATTEMPS) { <!--En este if else va la condiciona de limitar el numero de intentos a 10, si sobre pasa debe mostrar el mensaje de Perdiste-->
      lastResult.textContent = '!!!Perdistes!!!'; <!--Se corrige la escritura del mensaje-->
      lastResult.style.backgroundColor = 'red'; <!--Se cambio el color correcto que es el rojo -->

      lastResult.style.backgroundColor = 'black'; <!--Se cambio el color correcto que es el negro -->

  guessSubmit.addEventListener('click', checkGuess); <!--Lo correcto es: addEventListener en lugar de: addeventListener -->


	  resetButton.addEventListener('click', resetGame); <!--Lo correcto es: addEventListener en lugar de: addeventListener -->


	  randomNumber = Math.floor(Math.random() *10) + 1; <!--Error, lo correcto es: randomNumber = Math.floor(Math.random() * 10) + 1-->
