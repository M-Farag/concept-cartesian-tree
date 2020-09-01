## Cartesian tree
A Laravel package that implements the cartesian algorithm to generate permutations out of a sequence of arrays.
<br><br>
#### What is this package?
If you want to generate all of the possible permutations by combining multiple arrays, 
This package will do it for you.
<br><br>

#### How to install it?
Run this comman within your Laravel application
    ```
    composer require concept/cartesian-tree
    ```
<br><br>
#### How to use it?
* Use the package within any class in your codebase by importing the package's model 		
* Within any method, Call the static method __buildPermutations__ to combine any given array and generate a single array of all permutations.

```
<?php
 use Concept\CartesianTree\Cartesian;
 
 $permutations = Cartesian::buildPermutations([[1,2,3],['a','b','c']]);
 
 dd($permutations);
?>
```
_Results will be like this:_

```
Array
(
    [0] => Array
        (
            [0] => 1
            [1] => a
        )

    [1] => Array
        (
            [0] => 1
            [1] => b
        )

    [2] => Array
        (
            [0] => 1
            [1] => c
        )

    [3] => Array
        (
            [0] => 2
            [1] => a
        )

    [4] => Array
        (
            [0] => 2
            [1] => b
        )

    [5] => Array
        (
            [0] => 2
            [1] => c
        )

    [6] => Array
        (
            [0] => 3
            [1] => a
        )

    [7] => Array
        (
            [0] => 3
            [1] => b
        )

    [8] => Array
        (
            [0] => 3
            [1] => c
        )

)
```
<br><br>
#### Please Note 
* You can combine as many arrays as you want.
* I used this package to combine up to 7 different arrays.
<br><br>
#### Upcoming updates
* PHPUNIT Testing.
