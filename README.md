# angularjs1-5-case-insensitive-match
AngularJS 1.5 Case-Insensitive Match

Based on 'Case-Insensitive Match' at https://www.youtube.com/watch?v=OdRuVyi7NuI&index=35&list=PL6n9fhu94yhWKHkcL7RJmmXyxkuFB3KSl

#Case-Insensitive Match

Uses angular ```caseInsensitiveMatch``` property.

Routes are case sensitive by default. 

To make a route case-insensitive, set ```caseInsensitiveMatch``` property to ```true```.

```javascript
$routeProvider
    .when("/home", {
        templateUrl: "templates/home.html",
        controller: "homeController",
        controllerAs: "ctrl",
        caseInsensitiveMatch: true
    })
```

To make ***all*** routes case-insensitive, set ```caseInsensitiveMatch``` property on ```$routeProvider```.

```javascript
$routeProvider.caseInsensitiveMatch = true;
```

See script.js, index.html and styles.css how to implement this.
