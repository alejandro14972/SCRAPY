
# Scrapy puppeteer

Node Puppeteer es una biblioteca de Node.js que proporciona una interfaz de programación para controlar y automatizar el navegador web Chrome o Chromium. Utiliza el protocolo de depuración de Chrome para interactuar con el navegador de manera programática, lo que permite realizar acciones como navegar por páginas web, completar formularios, hacer capturas de pantalla, extraer datos y mucho más.
Puppeteer es especialmente útil para realizar pruebas automatizadas, scraping web (extracción de datos de páginas web) y generar archivos PDF o capturas de pantalla de manera automatizada. Al ejecutar el código de Puppeteer, se crea una instancia de Chrome o Chromium en segundo plano que se puede controlar mediante comandos de programación.
Node Puppeteer ofrece una API fácil de usar y una amplia gama de funciones para interactuar con el navegador. Puedes controlar la navegación, interactuar con elementos de la página, manipular el contenido, ejecutar scripts en la página, capturar y manipular eventos, entre otras acciones. Es una herramienta poderosa para realizar tareas automatizadas relacionadas con la interacción con navegadores web.

Código para instalar dependencias. Importante hacerlo en una carpeta nueva y tener node.js instalado.

```
npm install puppeteer
```




## Documentation

[Documentación](https://pptr.dev/)

Métodos de la librería:
1. `page.goto(url[, options])`: permite navegar a una URL especificada en la página actual. Los parámetros opcionales incluyen un objeto con opciones como tiempo de espera, tiempo de espera para carga de recursos, etc.
2. `page.waitForSelector(selector[, options])`: espera a que el elemento que coincide con el selector especificado se cargue en la página. Las opciones incluyen tiempo de espera máximo y visibilidad del elemento.

3. `page.$$(selector)`: devuelve un arreglo de elementos que coinciden con el selector especificado.
4. `page.evaluate(pageFunction[, ...args])`: ejecuta una función en el contexto de la página y devuelve el resultado. Los argumentos opcionales se pasan a la función.
5. `page.type(selector, text[, options])`: ingresa texto en un elemento que coincide con el selector especificado. Las opciones incluyen un retraso entre pulsaciones de teclas, retraso inicial, etc.
6. `page.click(selector[, options])`: hace clic en el elemento que coincide con el selector especificado. Las opciones incluyen un botón de clic, coordenadas de clic, tiempo de espera después del clic, etc.
7. `page.screenshot([options])`: toma una captura de pantalla de la página actual. Las opciones incluyen un área de recorte, calidad de imagen, formato de archivo, etc.
8. `page.waitForNavigation([options])`: espera a que la página se cargue después de hacer clic en un enlace o enviar un formulario. Las opciones incluyen tiempo de espera máximo, estado de respuesta, etc.
9. `page.goBack([options])`: navega hacia atrás en el historial de la página. Las opciones incluyen tiempo de espera máximo, estado de respuesta, etc.
10. `page.waitFor(...events)`: espera a que ocurra uno o varios eventos en la página. Los eventos pueden ser cadenas de texto o funciones que devuelven una promesa.
11. `page.setViewport(viewport)`: establece la resolución y el tamaño de la ventana de la página. El argumento debe ser un objeto con propiedades `width`, `height` y `deviceScaleFactor`.

Estos son solo algunos de los métodos que ofrece la librería Puppeteer de JavaScript para hacer web scraping. Dependiendo de la tarea específica, es posible que se deban utilizar otros métodos o combinar varios de ellos para lograr los resultados deseados.

## Authors

- [@alejandro14972](https://github.com/alejandro14972?tab=repositories)

