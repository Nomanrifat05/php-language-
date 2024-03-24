# PHP Lenguage
Welcome to my php note!



## First php file

#### Example 1:
![image](https://github.com/Nomanrifat05/php-language-/assets/128896891/732a1330-43c9-4952-8f2b-d21e8ff83f9e)

``` Your First PHP File
<?php 

	// echo 'hello, ninjas';

?>

<!DOCTYPE html>
<html>
<head>
	<title>my first PHP file</title>
</head>
<body>
	<h1><?php echo 'hello, ninjas' ?></h1>
</body>
</html>
```

#### Example 2:
![image](https://github.com/Nomanrifat05/php-language-/assets/128896891/ebd4783e-6d1e-4b2a-a8d0-fc87c7e048e6)

``` Variables & Constants
<?php 

	define('NAME', 'Yoshi');

	// $name = 'Yoshi';
	$age = 30;

	// $name = 'Mario';
	define('NAME', 'Mario');

?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

	<h1>User profile page</h1>

	<div><?php echo NAME; ?></div>
	<div><?php echo $age; ?></div>

</body>
</html>
```

#### Example 3:
![image](https://github.com/Nomanrifat05/php-language-/assets/128896891/78b25ed5-dec4-4f01-aad8-abe09562c984)

```Strings
<?php 

	$stringOne = 'my email is ';
	$stringTwo = 'mario123@thenetninja.co.uk';

	echo $stringOne.$stringTwo;

	//new line
	echo "<br>";echo "</br>";



	$name = 'mario';

	// concatenation
	echo 'Hey, my name is '.$name;

	 


	// variable interpolation
	echo "Hey, my name is $name"; 

	 

	// escaping characters
	echo "the ninja screamed \"whaaa\"";

	 


	echo 'the ninja scream "whaaa"';

	 


	// get single characters
	echo $name[1];

	 

	// string functions
	echo strlen($name);

	 

	echo strtoupper($name);

	 

	echo strtolower($name);

	 

	echo str_replace('m', 'w', $name);

?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

	<p><?php echo $name; ?></p>

</body>
</html>
```






#### Example 4:
```php code
<?php 

	$radius = 25;
	$pi = 3.14;

	// basic operators - *, /, +, -, ^

	echo $pi * $radius^2;

	// order of operation (B I D M A S)

	echo 2 * (4 + 5) / 3;

	// increment & decrement operators

	echo $radius++;
	echo $pi--;

	// shorthand operations

	$age = 20;
	$age += 10; // age becomes 30
	$age -= 5; // age becomes 25
	$age *= 2; // age becomes 50

	echo $age;

	// number functions

	echo floor($pi);
	echo ceil($pi);
	echo pi();

?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

	<p><?php echo $age; ?></p>

</body>
</html>

```

#### Example 5:
```php code
<?php 

	// indexed arrays

	$peopleOne = ['shaun', 'crystal', 'ryu'];
	//echo $peopleOne[1];

	$peopleTwo = array('ken', 'chun-li');
	//echo $peopleTwo[1];

	$ages = [20, 30, 40, 50];

	//print_r($ages);

	$ages[1] = 25;
	//print_r($ages);

	$ages[] = 10;
	array_push($ages, 70);
	//print_r($ages);

	//echo array_pop($ages);
	//print_r($ages);

	//echo count($ages);

	$peopleThree = array_merge($peopleOne, $peopleTwo);
	//print_r($peopleThree);

	// associative array (key & value pairs)

	$ninjasOne = ['shaun' => 'black', 'mario' => 'orange', 'luigi' => 'brown'];
	//echo $ninjasOne['mario'];
	//print_r($ninjasOne);

	$ninjasTwo = array('bowser' => 'green', 'peach' => 'yellow');
	//print_r($ninjasTwo);

	$ninjasTwo['toad'] = 'pink';

	//echo count($ninjasTwo);

	$ninjasThree = array_merge($ninjasOne, $ninjasTwo);
	print_r($ninjasThree);



?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

	<p></p>

</body>
</html>
```


#### Example 6:
```php code
<?php 

	// multidimensional array

	$blogs = [
		['title' => 'mario party', 'author' => 'mario', 'content' => 'lorem'],
		['title' => 'mariokart cheats', 'author' => 'toad', 'content' => 'lorem'],
		['title' => 'zelda hidden chests', 'author' => 'link', 'content' => 'lorem']
	];

	//print_r($blogs);
	//print_r($blogs[2]);
	//echo $blogs[1]['title'];
	//echo count($blogs);

	$blogs[] = ['title' => 'castle party', 'author' => 'peach', 'content' => 'lorem'];
	//print_r($blogs);

	$popped = array_pop($blogs);
	//print_r($popped);


?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

	<p></p>

</body>
</html>


```



#### Example 7:
```php code
<?php 

	$ninjas = ['shaun', 'ryu', 'yoshi'];

	// for($i = 0; $i < count($ninjas); $i++){
	// 	echo $ninjas[$i] . '<br />';
	// }

	// foreach($ninjas as $ninja){
	// 	echo $ninja . ' <br/>';
	// }

	$products = [
		['name' => 'shiny star', 'price' => 20],
		['name' => 'green shell', 'price' => 10],
		['name' => 'red shell', 'price' => 15],
		['name' => 'gold coin', 'price' => 5],
		['name' => 'lightning bolt', 'price' => 40],
		['name' => 'banana skin', 'price' => 2]
	];

	// foreach($products as $product){
	// 	echo $product['name'] .' - '. $product['price'];
	// 	echo '<br />';
	// }

	$i = 0;

	while($i < count($products)){
		echo $products[$i]['name'];
		echo '<br />';
		$i++;
	}


?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

	<h1>Products</h1>
	<ul>
		<?php foreach($products as $product){ ?>
			<h3><?php echo $product['name']; ?></h3>
			<p>£<?php echo $product['price']; ?></p>
		<?php } ?>
	</ul>

</body>
</html>
```



#### Example 8:
```php code
<?php 

	// comparisons & booleans (true or false)
	//echo true // echo's "1"
	//echo false // echo's ""

	// numbers
	//echo 5 < 10;
	//echo 5 > 10;
	//echo 5 == 10;
	//echo 10 == 10;
	//echo 5 != 10;
	//echo 5 <= 5;
	//echo 5 >= 5;

	// strings
	//echo 'shaun' < 'yoshi';
	//echo 'shaun' > 'yoshi';
	//echo 'shaun' > 'Shaun';
	//echo 'mario' == 'mario';
	//echo 'mario' == 'Mario';

	// loose vs strict equal comparison

	//echo 5 == '5';
	//echo 5 === '5';
	//echo 5 === 5;

	//echo true == 1;
	echo true === 1;
	
?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

</body>
</html>
```

#### Example 9:
```php code
<?php 

	// conditional statements
	
	// $price = 20;

	// if($price < 30){
	// 	echo 'if condition met';
	// } elseif($price === 20) {
	// 	echo 'elseif condition met';
	// } else {
	// 	echo 'condition not met';
	// }

	$products = [
		['name' => 'shiny star', 'price' => 20],
		['name' => 'green shell', 'price' => 10],
		['name' => 'red shell', 'price' => 15],
		['name' => 'gold coin', 'price' => 5],
		['name' => 'lightning bolt', 'price' => 40],
		['name' => 'banana skin', 'price' => 2]
	];

	foreach($products as $product){

		// if($product['price'] < 15 && $product['price'] > 2){
		// 	echo $product['name'] . '<br />';
		// }

		// if($product['price'] > 20 || $product['price'] < 10){
		// 	echo $product['name'] . '<br />';
		// }

	}

?>

<!DOCTYPE html>
<html>
<head>
	<title>PHP Tutorials</title>
</head>
<body>

	<div>
		<ul>
			<?php foreach($products as $product){ ?>
				<?php if($product['price'] > 15){ ?>
					<li><?php echo $product['name'] ?></li>
				<?php } ?>
			<?php } ?>
		</ul>
	</div>

</body>
</html>
```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```

#### Example 8:
```php code

```




## DELETE DATA INTO Database Table

#### Way 1:
```sql
DELETE FROM table_name
WHERE [condition];
```

