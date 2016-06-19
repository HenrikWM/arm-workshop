# ARM-workshop

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FHenrikWM%2Farm-workshop%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FHenrikWM%2Farm-workshop%2Fmaster%2Fazuredeploy.json" target="_blank">
  <img src="http://armviz.io/visualizebutton.png"/>
</a>

Deploy en enkel HelloWorld Web App til Azure og visualiser deployet infrastruktur.

## Workshop 

Workshoppen handler om provisjonering av ressurser via [Azure Resource Manager], holdt av [@henrikwm84] for .NET-faggruppen i BEKK.

## Slides

Slides for workshopen dekker:

- Konsept
- Template format
- Verktøy
- Cheat sheet med ressurser

For å bygge slidene behøver du Node + NPM installert globalt i tillegg til [remark-themet til BEKK].

Bygg ved å kjøre følgende:

```sh
$ git clone https://github.com/henrikwm/arm-workshop
$ cd slides
$ npm install bekk/remark
```

Deretter åpner du `index.html` i en nettleser.

[@henrikwm84]: <http://twitter.com/henrikwm84>
[slides]: <https://github.com/henrikwm/arm-workshop/slides>
[Azure Resource Manager]: <https://azure.microsoft.com/en-us/documentation/articles/resource-group-overview/>
[remark-themet til BEKK]: <https://github.com/bekk/remark>
