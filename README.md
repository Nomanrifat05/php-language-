# PHP Lenguage
Welcome to my php note!



## First php file

#### Example 1:
```php code
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
```php code
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
```php code
<?php 

	$stringOne = 'my email is ';
	$stringTwo = 'mario123@thenetninja.co.uk';

	echo $stringOne.$stringTwo;

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


#### Example 4:
```php code

```



#### Example 4:
```php code

```



#### Example 4:
```php code

```



## DELETE DATA INTO Database Table

#### Way 1:
```sql
DELETE FROM table_name
WHERE [condition];
```

