# Laravel Lightning Talk

### What is Laravel?
Laravel is an open-source PHP framework, for building MVC web applications.

### PHP Artisan
PHP Artisan is the CLI included with Laravel. Many of the commands are very similar to what we are used to with the Angular CLI(eg. creating models, controllers, etc..)

Laravel also has an included REPL, Tinker. Tinker allows you to interact with the entire Laravel application on the command line.


### Templating and Blade
Laravel provides a templating engine called blade. Blade compiles all of the applications views into plain PHP code and caches them until they are modified. This means that Blade adds virtually zero overhead to the project.


### @extends, @includes, @section/content & @yield
In true MVC-fashion, Laravel allows us to 'separate our concerns' and breaking our views into different components. Our parent component will include the children components to bring them into the view. You also have the ability to include sections of content on a child component, and then yield that content on the parent view. 


### csrf tokens
# From the Laravel Documentation: 
Laravel makes it easy to protect your application from cross-site request forgery (CSRF) attacks. Cross-site request forgeries are a type of malicious exploit whereby unauthorized commands are performed on behalf of an authenticated user.

Laravel automatically generates a CSRF "token" for each active user session managed by the application. This token is used to verify that the authenticated user is the one actually making the requests to the application.

Anytime you define a HTML form in your application, you should include a hidden CSRF token field in the form so that the CSRF protection middleware can validate the request.

### Resources
* Documentation: [docs](https://laravel.com/docs/5.5)
* Laracasts: [tutorial](https://laracasts.com/series/laravel-from-scratch-2017)