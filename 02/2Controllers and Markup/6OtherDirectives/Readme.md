# Other Directives

- ngApp
- ngBind
- ngBindTemplate
- ngBindHtml
- ngBindHtmlUnsafe


## ng-bind

Bind single value

<h2 ng-bind="{{event.name}}"> </h2>


## ng-bind-template

Bind multiple values

<h2 ng-bind-template="{{event.name}} {{event.date}}"> </h2>


## ng-bind-html and ng-bind-html-unsafe

* Need to call  <script src="/lib/angular/angular-sanitize.js"></script> library

<div ng-bind-html="snippet">
	some title
</div>

$scope.snippet ='<<span style="color:red">Hi ngBindHtml</span>';

- ngHide
- ngShow

- ng-cloak


- ng-style
- ngClass

We used in ng-repeat.
- ngClassEven
- ngClassOdd


#Quiz

1. What is the purpose of ng-cloak directive ?

To avoid a flash of unbound html

2. ng-bind supports multiple binds?

No, ng-bind not supported.
The ng-bind-template directive is the directive only support multiple bindings

3. The ngClass directive has two companion directives. What are they ?

- ngClassEven
- ngClassOdd