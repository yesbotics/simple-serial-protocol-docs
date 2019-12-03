# Development
dev - lorem ipsum durchdeven

## Branches (Gitflow) 
inspiriert durch [GitFlow Examples]
* `master`: live. echte releases. (erst, wenn was published wurde kommt hier zeug aus'm 
develop branch rein)
* `develop`: nur fertige candidates hier drin (getestet und lauffähig)
    * Pufferzone vor Veröffentlichung
* `release`: übergeordneter branch für next-level shit, der klar in versionen
    * Ist dem develop untergeordnet
    * Von hier aus wird published.
        * und zwar nur dev-releases `npm publish --tag dev`
        * installierbar via npm i `@yesbotics/simple-serial-protocol-node`
definiert ist (bsp: `release/2.0.1` oder `release/2.0.1-beta.0`)
* `hotfix`: echte fixes und workarounds für live (published) releases

### Kommunikation, wie?
* modrob/yesbotics tg-channel
* via textdateien wie im hierigen fall
* via issues gitlab

### CodeOps
* git comit message konventionen vereinbaren
* z.b. Kategorien wie:
    * CodeOps, DocOps, DevOps
        * Details
    * kategorielos
        * freitext
     
### DocOps
* Markdown und ggf. transpiler kennenlernen
* Markdown links? [Markdown-Cheatsheet#links]
* simple-serial-protocol-docs aufbauen unter zuhilfenahme von [Markdown: Links and Cross References (dotnet)]
* @kappaj: more examples readme
    * hier kommt kappaj's extrakt rein (aus der `README.md.old`) 
    * einzelinterval-examples zusammenfassen in einem standalone `AdvancedExample`
    * eigenständige node app (wie bei /examples/echo-example)
    * deinen test kram (seh ich als bestandteil - des im nächsten hauptpunkt erwähnten - deployments)

#### Deployment
* das deployment müssen wir entwickeln:
    * npm scripte 
    * halbautomatisches script (also mit bestätigen)
        * npm login
        * npm publish
            * prepublish muss testen
    * jest test
    * ne release ablauf dokumentieren, was abgearbeitet werden muss:
        * getestet?
        * version korrekt erhöht?
        * müssen wir zusammen drüber sprechen

## Links
[GitFlow Examples]:https://gitversion.readthedocs.io/en/latest/git-branching-strategies/gitflow-examples
[Markdown-Cheatsheet#links]:https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links
[Markdown: Links and Cross References]:https://dotnet.github.io/docfx/tutorial/links_and_cross_references.html
[Publishing a beta or alpha version to NPM]:https://medium.com/@kevinkreuzer/publishing-a-beta-or-alpha-version-to-npm-46035b630dd7
[Have `npm version` not prepend “v” to the git tag]:https://stackoverflow.com/questions/37788907/have-npm-version-not-prepend-v-to-the-git-tag
[Arduino library specifications]:https://github.com/arduino/Arduino/wiki/Arduino-IDE-1.5:-Library-specification
[Thoughts on Flash - Apple]:https://www.apple.com/hotnews/thoughts-on-flash/
[Thoughts on Flash - Wikipedia]:https://en.wikipedia.org/wiki/Thoughts_on_Flash

