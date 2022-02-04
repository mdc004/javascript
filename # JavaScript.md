# JavaScript

## If: sintassi veloce

`condizione da verificare ? ramo del vero: ramo del falso`

esempio:

```
    count > 1 ? count-- : count++ 
```

## Metodi con la console

stampa in console:
```
    console.log()
```

stampa le proprietà di un oggetto in console:
```
    console.dir()
```

stampa in una tabella in console le celle di un array e il relativo contenuto:
```
    console.table(nome_array)
```

## Ricerca nel documento

Ricerca per ID
```
    document.getElementById("nome ID")
```

Ricerca per selettore
```
    document.querySelector("nome selettore")
```

> Nota bene:
> questi due metodi restituiscono un solo elemento, nel caso di querySelector viene restituito il primo elemento trovato con quel determinato selettore

Ricerca per classe

```
    document.getElementsByClassName("nome classe")
```

Ricerca per nome del tag

```
    document.getElementsByTagName("nome tag")
```

Ricerca per nome del tag

```
    document.querySelectorAll("nome selettore")
```

> Nota bene:
> questi metodi restituiscono degli array

## setTimeout

esegue la funzione dopo un determinato periodo di tempo

`setTimeout(funzione, tempo [in millisecondi], parametri funzione);`

esempio:

```
    setTimeout(console.log("10"), 5000)
```

## setInterval

ripete la funzione ogni determinato periodo di tempo

`setInterval(funzione, tempo [in millisecondi])`

esempio:

```
    setInterval(function () {element.innerHTML += "Hello"}, 1000)
```

### clearInterval

interrompe il setInterval

`clearInterval(valore restituito da setInterval)`

esempio:

```
    var repeat = setInterval(function () {element.innerHTML += "Hello"} 1000)

    clearInterval(repeat)
```

## Creare un elemento

`nuovo_elemento = document.createElement("nome elemento")`

`dove_inserire_il_nuovo_elemento.appendChild(nuovo_elemento)`

esempio:

```
    tab = document.createElement("table")

    grid.appendChild(tab)
```

## Aggiungere classi ad un elemento

`elemento.classList.add("nome classe")`

esempio:

```
    tab.classList.add("table")
```
