# Angular.js v1.1.5 - IE8 compatible

AngularJS [v.1.1.5] working on IE8.

Angular is not compatible with IE8 since version 1.3. Versions 1.2.x should work, but didn't do it for us. Here is a version that works for IE8.

Based on: https://github.com/jasonm23/angular.js-v1.1.5

Changes made to IE8 compatible:
1. Added console object creation, if console does not exists
2. Added check for IE8
3. Added ie<9 if statement: e.apply will not run for ie<9

See .js file for details

== Notes ==

In most cases you should not want to support IE8, unless you have to. IE8 has a browser share < 5%. Not supporting IE6,7,8 makes developer life easier. 

If this library does not work for you, try: 
* The minified version vs unminified version
* https://github.com/fergaldoyle/angular.js-ie8-builds
* https://github.com/YanagiEiichi/angular-ie8provider

Additional angular libraries (angular-cookies, angular-resource, angular-sanitize, etc.) can be retrieved from official AngularJS Git repository.

Do not use HTML5 elements together with angular (main, section, article, aside, etc), it doesn't work well in IE8.

