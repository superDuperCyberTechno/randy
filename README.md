# randy
#### The Mersenne Twister in PHP - A seedable pseudorandom number generator

Based on [this](https://www.dr-chuck.com/csev-blog/2015/09/a-mersenne_twister-implementation-in-php/).

Install it using composer:

```
composer install superdupercybertechno/randy
```

To use it, add the following to your file:

```
use superDuperCyberTechno\Randy;
```

When you need it, simply invoke it and request numbers.

```
$randy = new Randy($seed);
$number = $randy->num(0,100);
```

Where `$seed` is a string of your choosing. If you leave out `$seed`, Randy will seed itself with a random number.
Each time you run the method `num` you will receive a new number within the limits passed (`0` and `100` in the above example). Using the same seed will produce a predictable batch of numbers.
