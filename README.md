# Angular.js v1.1.5 - IE8 compatible

AngularJS v.1.1.5 - fixed to work in IE8.

Since version 1.3 Angular is officially not compatible with IE8. However, we found angular versions 1.2.x equally not working. Here is a version that works for IE8.

Based on: https://github.com/jasonm23/angular.js-v1.1.5

Changes made to IE8 compatible:

1. Added console object creation, if console does not exists
2. Added check for IE8
3. Changed: e.apply does not run for ie<9

See .js file for details

== Notes ==

In most cases you should not want to support IE8, unless you have to. IE8 has a browser use share < 5%. Not supporting IE6,7,8 makes developer life easier. 

If this library does not work for you, try: 
* https://github.com/fergaldoyle/angular.js-ie8-builds
* https://github.com/YanagiEiichi/angular-ie8provider

Additional angular libraries (angular-cookies, angular-resource, angular-sanitize, etc.) can be retrieved from official AngularJS Git repository.

Do not use HTML5 elements together with angular (main, section, article, aside, etc), it doesn't work well in IE8.

