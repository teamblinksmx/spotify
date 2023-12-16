# HI! BLINKS

# VERSIÓN EN ESPAÑOL


```js
var conteoStreams = 0;
function ObtenerEnteroRandom(minimo, maximo) {
  minimo = Math.ceil(minimo);
  maximo = Math.floor(maximo);
  return Math.floor(Math.random() * (maximo - minimo) + minimo);
}

function hacerAlgo() {
  var button = document.querySelector('[aria-label="Siguiente"]').click();
  conteoStreams++;
}

(function loop() {
  var rand = ObtenerEnteroRandom(35000, 40000);
  console.log(" Conteo Streams: " + conteoStreams);
  setTimeout(function () {
    hacerAlgo();
    loop();
  }, rand);
})();
```


# ENGLISH VERSION

```js
var streamsCount = 0
function getRandomInt(min, max) {
  min = Math.ceil(min);
  max = Math.floor(max);
  return Math.floor(Math.random() * (max - min) + min);
}

function doSomething() {
  var button = document.querySelector('[aria-label="Next"]');
  button.click();
  streamsCount++;
}

(function loop() {
  var rand = getRandomInt(33000, 37000);
  console.log(" Streams Count: " + streamsCount);
  setTimeout(function () {
    doSomething();
    loop();
  }, rand);
})();

```
