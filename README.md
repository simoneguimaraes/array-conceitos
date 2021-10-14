## Arrays


```javascript
// adicionar e remover elementos
let myArray = ['hello', 'goodbye', 'good morning', 'good day', 'bye']

let lastElement = myArray.pop()
let firstElement = myArray.shift()
myArray.push(firstElement)
myArray.unshift(lastElement)

console.log(myArray)

// remover e substituir elementos com splice

let newArray = ['ana', 'bernardo', 'catia', 'douglas', 'emmy']
newArray.splice(0, 1, 'amanda')

console.log(newArray)

// usando FOR loop com arrays
let names = ['ana', 'bernardo', 'catia', 'douglas', 'emmy']

for(let contador = 0; contador < names.length; contador++) {
  console.log(`Ganhador ${contador}: ${names[contador]}`)
}

// usando WHILE loop com arrays

let names = ['ana', 'bernardo', 'catia', 'douglas', 'emmy']

let contador = 0
while(contador < names.length) {
  console.log(`Ganhador ${contador}: ${names[contador]}`)
  contador++
}

// Exercicio de Soma de Itens da Array

const prices = [10.99, 44.56, 112.79, 3, 5];
let sum = 0;

for(contador = 0; contador < prices.length; contador++) {
  sum += prices[contador]
}

sum = sum.toFixed(1)
console.log(sum)

// Exercício Séries 

let seriesPending = ['Breaking Bug', 'Game of Drones', 'Boolean 99', 'Arrested Developer'];

seriesPending.push('The Evening Show')

for(let contador = 0; contador < seriesPending.length; contador++) {
    console.log(`Série ${contador}: ${seriesPending[contador]}`)
    if(seriesPending[contador] == 'Boolean 99') {
      console.log("Found it!")
    }
}

// Exercício Assistindo Séries

let seriesPending = ['Breaking Bug', 'Game of Drones', 'Boolean 99', 'Arrested Developer'];
let seriesWatching = ['The Evening Show']

seriesWatching.push(seriesPending.shift())
console.log(seriesPending.length)
console.log(seriesWatching.length)

for(let contador = 0; contador < 4; contador++) {
  seriesWatching.push(seriesPending.shift())
}


seriesWatching.splice(0, seriesWatching.length)

console.log(seriesWatching)
console.log(seriesPending)


// imprimir todos os elementos de uma array

clientData = ['edson', 67, 'loner', 'public', 99, 'exercise']

for(let contador = 0; contador < clientData.length; contador++) {
  console.log(`Dado ${contador}: ${clientData[contador]}`)
}  

*/

// imprimir todos os elementos de uma array usando Function

function showData(array) {
  for(let contador = 0; contador < array.length; contador++) {
    console.log(`Dado ${contador}: ${array[contador]}`)
  }  
}

clientData = ['edson', 67, 'loner', 'public', 99, 'exercise']

showData(clientData)
```
