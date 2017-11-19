# \<credit-evaluator\>

Polymer component that creates a generic, customizable and dynamic credit evaluator.

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

## Styles

### Custom properties

|Custom property  | Description   | Default value |
|---------------- |:-------------:|:----------:|
|--credit-evaluator-height| height |400px|
|--credit-evaluator-width| width |100%|
|--credit-evaluator-mixin| host mixin | {}|
|--credit-evaluator-header-display| header display |flex|
|--credit-evaluator-header-flex-direction| header flex-direction |row|
|--credit-evaluator-header-align-items| header align-items |center|
|--credit-evaluator-header-justify-content| header justify-content |center|
|--credit-evaluator-header-height| header height |10%|
|--credit-evaluator-header-width| header width |100%|
|--credit-evaluator-header-border| header border |1px solid white|
|--credit-evaluator-header-bg-color| header bg-color |black|
|--credit-evaluator-header-color| header color |lightgray|
|--credit-evaluator-header-font-size| header font-size |2rem|
|--credit-evaluator-header-mixin| header mixin mixin | {}|
|--credit-evaluator-main-display| main display |flex|
|--credit-evaluator-main-flex-direction| main flex-direction |column|
|--credit-evaluator-main-justify-content| main justify-content |center|
|--credit-evaluator-main-height| main height |80%|
|--credit-evaluator-main-width| main width |100%|
|--credit-evaluator-main-border| main border | 1px solid white|
|--credit-evaluator-main-bg-color| main bg-color |white|
|--credit-evaluator-main-color| main color |black|
|--credit-evaluator-main-mixin| main mixin | {}|
|--credit-evaluator-footer-display| footer display |flex|
|--credit-evaluator-footer-flex-direction| footer flex-direction |row|
|--credit-evaluator-footer-align-items| footer align-items |center|
|--credit-evaluator-footer-justify-content| footer justify-content |center|
|--credit-evaluator-footer-height| footer height |10%|
|--credit-evaluator-footer-width| footer width |100%|
|--credit-evaluator-footer-border| footer | 1px solid white|
|--credit-evaluator-footer-bg-color| footer bg-color |lightgray|
|--credit-evaluator-footer-color| footer color |white|
|--credit-evaluator-footer-font-size| footer font-size |1rem|
|--credit-evaluator-footer-mixin| footer mixin | {}|


## Properties

### Custom properties

|Custom property  | Description   |
|---------------- |:-------------:|
|titleHeader    | titulo que se pinta sobre el header del formulario|
|titleFooter    | titulo o leyenda que se pinta sobre el footer|
|url    | url de la api que se va consumir a traves del componente|
|body   | body de la peticion que se va a realizar con base en los formulario|
|config   | propiedad usada cuando no se tiene un api realiza el calculo basico de un prestamo personal|
|params   | parametros de la peticion|
|request    | json que se envia en la solicitud de la api|
|form   | arreglo con los objetos que forman el formulario|
|response   | respuesta que arroja la api|
|titleMessage   | titulo que se genera con la respuesta del servicio|
|message    | mensaje que se genera con la respuesta del servicio|


## Methods

### Custom events

|Custom property  | Description   | Parametros |
|---------------- |:-------------:|:----------:|
|_generateReques  | metodo que genera la peticion a la API si es que se encuentra seteada la propiedad url| ninguno |
|_generateBody  | metodo que convierte los valores del formulario a un objeto| Array |
|_handleFormSubmit  | metodo que se invoca cuando se escucha el evento de submit en el formulario| event|
|_handleAproved | metodo invocado cuando la respuesta de la API es afirmativa(autoriza el crédito)| event|
|_handleDenegade  | metodo invocado cuando la respuesta de la API es negativa(no se autoriza el crédito)| event|
|_handleError | metodo invocado cuando la petición falla| response|
|_generateTitleMessage  | metodo que genera automaticamente el titulo del mensaje| response|
|_generateMessage | metodo que genera el cuerpo del mensaje mostrado al solicitar un crédito| reponse|
