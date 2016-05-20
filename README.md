# flags-rest-service

This REST Web service contains 241 countries complies with ISO 3166-1. The country name is available in several languages (French and English for now). The Web service also included the 3 digit code of the country, the 2-letter code (used in many applications, including monetary applications ) and the 3-letter code.

For information, the information for country France , will be the following
* Code ISO 3166-1 numérique : 250
* Code ISO 3166-1 alpha2 : FR
* Code ISO 3166-1 alpha3 : FRA

# Supported languages

These are the currently supported languages

* Czech
* German
* English
* Spanish
* French
* Italian
* Dutch
	
Does flags-rest-service not support your language? Please help us with a PR!

# Travis CI status

[![Build Status][travis-image]][travis-url]
[travis-image]: https://travis-ci.org/sgrillon14/flags-rest-service.svg?branch=master
[travis-url]: https://travis-ci.org/sgrillon14/flags-rest-service


# Technology

* HTML
* CSS
* AngularJS 1
* Spring Boot <b style='color:red'>(Caution: This application use 1.4.0.BUILD-SNAPSHOT)</b>
* Spring Web
* SVG
* TestNG
* Travis CI

# Run Anywhere
![RunAnywhere](/screenshots/plateforme.png)

Flags REST Service apps run anywhere the JVM does. Deploy standalone, in an app server, on a Cloud or all of the above.

# Production URL (Example)

UX (AngularJS 1):
* http://localhost:8084/views/index.html

![sampleAngularjs1](/screenshots/sampleAngularjs1.png)

use cases:
* http://localhost:8084/countries return a list of countries (in English) 
* http://localhost:8084/countries?lang=en return a list of countries (in English)
* http://localhost:8084/countries?lang=fr return a list of countries (in French)
* http://localhost:8084/fr return 200 OK and svg (French flag)

Errors cases:
* http://localhost:8084/countries?lang=fakecode return a list of countries (in English)
* http://localhost:8084/fakecode return 204 No Content

# JSON response (Example)

[...,{"num":250,"alpha2":"FR","alpha3":"FRA","label":"France"},...]

# License

BSD, See License.txt for details
