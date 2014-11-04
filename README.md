# Welcome to PHP Value Objects
[Value Objects](http://martinfowler.com/bliki/ValueObject.html) are an essential concept when implementing Domain Driven Design, but they can be used in any PHP project. [@cakper](https://twitter.com/cakper)'s [recent blog post](http://kacper.gunia.me/blog/ddd-building-blocks-in-php-value-object) is a good introduction, and we'll link to more resources in the coming weeks.

## Value Object Basics
The main characteristic of a Value Object is that it is *immutable*. This means that it has

* all properties initialised in the constructor
* no setters

If you want to modify a Value Object, you must create a new one.

You can use a Value Object anywhere you'd normally use an Associative Array. The benefits are many, including:

* it can be a type-hinted parameter in a method
* you won't miss-spell the key when getting values
* you can have Null Value Objects
* it can contain business/domain logic

Using a Value Object will help you encapsulate behaviour that would otherwise have been in code that accesses an associative array. This will make your code easier to understand and reduce the chance of errors.

If you are working with legacy code, refactoring to extract Value Objects is a relatively simple process that will pay dividends.

## Learn more about Value Objects
* [Wikipedia](https://en.wikipedia.org/wiki/Value_object)
* [The Elephant in the Room Podcast, Episode 2](http://elephantintheroom.io/blog/2013/10/episode-2-heart-and-soul-of-oop/) by [@mathiasverraes](https://twitter.com/mathiasverraes) and [@everzet](https://twitter.com/everzet) (2013-10)
* [Value Objects and User Interfaces](http://verraes.net/2013/11/value-objects-and-user-interfaces/) by [@mathiasverraes](https://twitter.com/mathiasverraes) (2013-11)
* [DDD Building Blocks in PHP: Value Objects](http://kacper.gunia.me/blog/ddd-building-blocks-in-php-value-object) by [@cakper](https://twitter.com/cakper) (2014-10)

## Implementations
### Money
* <https://github.com/mathiasverraes/money> by [@mathiasverraes](https://twitter.com/mathiasverraes)
* <https://github.com/sebastianbergmann/money> by [@s_bergmann](https://twitter.com/s_bergmann)

### Libraries
* <https://github.com/gws/php-valueobjects> by [@gws](https://gitlab.com/u/gws)
* <https://github.com/nicolopignatelli/valueobjects> by [@nicolopigna](https://twitter.com/nicolopigna)

## Who to follow on Twitter
* Mathias Verraes [@mathiasverraes](https://twitter.com/mathiasverraes)
* Konstantin Kudryashov [@everzet](https://twitter.com/everzet)
* PHPValueObjects [@phpvalueobjects](https://twitter.com/phpvalueobjects)
* Kacper Gunia [@cakper](https://twitter.com/cakper)

If you want to suggest a resource, email suggestions (at) phpvalueobjects (dot) info.