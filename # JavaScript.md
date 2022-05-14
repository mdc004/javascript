# JavaScript

## Ternary Operator

`condizione da verificare ? ramo del vero: ramo del falso`

esempio:

```javascript
    count > 1 ? count-- : count++ 
```

## Metodi con la console

stampa in console:
```javascript
    console.log()
```

stampa le proprietà di un oggetto in console:
```javascript
    console.dir()
```

stampa in una tabella in console le celle di un array e il relativo contenuto:
```javascript
    console.table(nome_array)
```

## Stampa nel documento
`document.write("Stringa")`
esempio:
```javascript
    document.write("Hello World!");
```

## Ricerca nel documento

Ricerca per ID
```javascript
    document.getElementById("nome ID")
```

Ricerca per selettore
```javascript
    document.querySelector("nome selettore")
```

> Nota bene:
> questi due metodi restituiscono un solo elemento, nel caso di querySelector viene restituito il primo elemento trovato con quel determinato selettore

Ricerca per classe

```javascript
    document.getElementsByClassName("nome classe")
```

Ricerca per nome del tag

```javascript
    document.getElementsByTagName("nome tag")
```

Ricerca per selettore

```javascript
    document.querySelectorAll("nome selettore")
```

> Nota bene:
> questi metodi restituiscono degli array

## setTimeout

esegue la funzione dopo un determinato periodo di tempo

`setTimeout(funzione, tempo [in millisecondi], parametri funzione);`

esempio:

```javascript
    setTimeout(console.log("10"), 5000)
```

## setInterval

ripete la funzione ogni determinato periodo di tempo

`setInterval(funzione, tempo [in millisecondi])`

esempio:

```javascript
    setInterval(function () {element.innerHTML += "Hello"}, 1000)
```

### clearInterval

interrompe il setInterval

`clearInterval(valore restituito da setInterval)`

esempio:

```javascript
    var repeat = setInterval(function () {element.innerHTML += "Hello"} 1000)

    clearInterval(repeat)
```

## Creare un elemento

`nuovo_elemento = document.createElement("nome elemento")`

`dove_inserire_il_nuovo_elemento.appendChild(nuovo_elemento)`

esempio:

```javascript
    tab = document.createElement("table")

    grid.appendChild(tab)
```

## Inserire un elemento in una precisa posizione

`nuovo_elemento = document.createElement("nome elemento")`

`dove_inserire_il_nuovo_elemento.insertBefore(nuovo_elemento, posizione)`

esempio:

```javascript
    tab = document.createElement("table")

    grid.insertBefore(table, td1)
```

## Aggiungere classi ad un elemento

`elemento.classList.add("nome classe1, nome classe2, ...")`

esempio:

```javascript
    tab.classList.add("table")
```

## Togliere classi ad un elemento

`elemento.classList.remove("nome classe")`

esempio:

```javascript
    tab.classList.remove("table")
```

## Controllare se un elemento contiene una classe

restituisce un boolean: "true" se la contiene, "false" altrimenti

`elemento.classList.contains("nome classe")`

esempio:

```javascript
    if(tab.classList.contains("table"))console.log("yes!!")
```

## Inserire css al foglio di stile

restituisce un array cotenente tutti i fogli di stile del documento

`document.styleSheets[0].insertRule("selettore { proprietà: valore; }")`

esempio:

```javascript
    document.styleSheets[0].insertRule("p { color: dak-green; }")
```

>Nota bene:
>Lo stile viene aggiunto all'inizio del foglio di stile, quindi bisogna verificare che non ci siano, successivamente, altre regole che lo vadano a riscrivere

## GetAttribute

restituisce un determinato attributo di uno specifico elemento

`elemento.getAttribute("nome_attributo")`

esempio:

```javascript
    document.getElementsByTagName("img")[0].getAttribute("width")
```

## SetAttribute

setta un determinato attributo di uno specifico elemento

`elemento.setAttribute("nome_attributo","valore_attributo")`

esempio:

```javascript
    document.getElementsByTagName("img")[0].setAttribute("width","100px")
```

## Reload della pagina (refresh [F5])

ricarica la pagina, è come premere F5

`windows.location.reload()`
