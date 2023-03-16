# html_snippets_vsc
#### Html5 snippets for Visual Studio Code configuration.

**FRAGMENTO DE CÓDIGO  PARA AUTOCOMPLETAR  LA ESTRUCTURA DE HTML CON `!`  EN VSC**
A continuación les dejo la configuración en formato `.json`, que tienen que copiar en su totalidad para luego pegar en la configuración de snippets de  Visual Studio Code. ¿Para qué sirve esto?, sirve para autocompletar la estructura de HTML con el carácter `!` y elegir la opción configurada.  

La configuración se abre desde:
> "archivo" -> "preferencias" -> "configurar fragmentos de usuario" -> "html.json"

Otra opción es:
>  control [ctrl]) + shift ([↑    ]) + [p]  --->  escribir: "user snippets" ---> "html.json"
 
Abajo del fragmento dado, está un video tutorial que muestra cómo hacerlo. Una vez completado, solamente hay que poner normalmente el `!` y enter en las opciones nuevas y ¡listo!, tu html se autocompleta.  

Cabe destacar que podes modificar el código json para hacer tu propia estructura.

---

##### Copiar y pegar este fragmento(básico) en la ubicación indicada:

```json
{
    "HTML5|lang=es": {
      "prefix": "!es",
      "body": [
        "<!DOCTYPE html>",
        "<html lang=\"es\">",
        "    $0",
        "<head>",
        "    <!---------- METAS ---------->",
        "    <meta charset=\"UTF-8\">",
        "    <meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">",
        "    $0",
        "    <!---------- LINKS ---------->",
        "    <link rel=\"stylesheet\" href=\"style.css\">",
        "    $0",
        "    <!---------- SCRIPTS -------->",
        "    <script src=\"\" type=\"text/javascript\"></script>",
        "    $0",
        "    <!---------- TITLE ---------->",
        "    <title>${1:Document}</title>",
        "</head>",
        "    $0",
        "<body>",
        "    $0",
        "</body>",
        "    $0",
        "</html>"
      ],
      "description": "HTML5 language=es"
    },
      "HTML5|lang=es|complete": {
        "prefix": "!escomp",
        "body": [
        "<!DOCTYPE html>",
        "<html lang=\"es\">",
        "    $0",
        "<!--===========HEAD=============-->",
        "<head>",
        "    <!---------- metas ---------->",
        "    <meta charset=\"UTF-8\">",
        "    <meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">",
        "    $0",
        "    <!---------- links ---------->",
        "    <link rel=\"stylesheet\" href=\"style.css\">",
        "    $0",
        "    <!---------- scripts -------->",
        "    <script src=\"\" type=\"text/javascript\"></script>",
        "    $0",
        "    <!---------- title ---------->",
        "    <title>${1:Document}</title>",
        "</head>",
        "    $0",
        "<!--===========BODY=============-->",
        "<body>",
        "    <header class=\"\">",
        "    </header>",
        "    $0",
        "    <main class=\"\">",
        "    </main>",
        "    $0",
        "    <footer class=\"\">",
        "    </footer>",
        "</body>",
        "    $0",
        "</html>"
        ],
        "description": "HTML5/esp/more"
    }
  }

```
[ver solo archivo json](https://raw.githubusercontent.com/Jesparzarom/html_snippets_vsc/main/html-snippets.json)



