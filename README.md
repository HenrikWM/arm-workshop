# ARM-workshop

### Forhåndsvisning

<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FHenrikWM%2Farm-workshop%2Fmaster%2Fazuredeploy.json" target="_blank">
  <img src="http://armviz.io/visualizebutton.png"/>
</a>

### Deploy

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

**Deploy to Azure** er en del av Kudu-verktøykassen og er drevet av [SlingShot]. 

## Workshop 

Workshoppen handler om provisjonering av ressurser og tjenester i Azure via [Azure Resource Manager] 

Oppgavene tar deg igjennom GitHub-prosjekter og artikler som bruker ARM-templates for å deploye tjenester til Azure. Gå til [oppgavene].

Kontakt: [@henrikwm84] / henrik.walker.moe at bekk.no

## Verktøy

* Visual Studio - Forfatte **Resource Groups** med `azuredeploy.json`, `azuredeploy.parameters.json` og `metadata.json`
* [Visual Studio Code] - Syntax highlighting, parsing av ARM-templates via [ARM-extension].
* [Resource Explorer] - [Lær mer](https://azure.microsoft.com/en-us/blog/azure-resource-explorer-a-new-tool-to-discover-the-azure-api/).
* [armviz.io] - Visualiser ARM-templates
* [Azure CLI]
* [Azure Powershell]

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
[oppgavene]: <https://github.com/HenrikWM/arm-workshop/blob/master/Oppgaver.md>
[Azure Resource Manager]: <https://azure.microsoft.com/en-us/documentation/articles/resource-group-overview/>
[remark-themet til BEKK]: <https://github.com/bekk/remark>
[SlingShot]: <https://github.com/projectkudu/slingshot>
[Resource Explorer]: <https://resources.azure.com/>
[armviz.io]: <http://armviz.io/>
[Azure CLI]: <https://azure.microsoft.com/en-us/documentation/articles/xplat-cli-install/>
[Azure Powershell]: <https://azure.microsoft.com/en-us/documentation/articles/powershell-install-configure/>
[Visual Studio Code]: <https://code.visualstudio.com/>
[ARM-extension]: <https://marketplace.visualstudio.com/items?itemName=msazurermtools.azurerm-vscode-tools&Wt.mc_id=DX_MVP8656>
