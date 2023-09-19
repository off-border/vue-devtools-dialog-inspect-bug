# Vue-Devtools dialog inspecting bug

Reproduction of Vue-Devtools inspector bug with HTML5 dialog element

- Run project `yarn && yarn serve`

- open dev page http://localhost:8080

- click "open dialog"

- try to inspect elements inside dialog

### Expected behaviour

Hovered elements on page are hightlighted by vue-devtools

### Actual behaviour

Ho githlighs, but whne you click on element - it shows up in vue-devtools tree
