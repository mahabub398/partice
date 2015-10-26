# partice
#This is my php partice Directory
<?php
abstract class Mahabub{
	public function hello()
	{
		echo "Hello ";
	}
	
	public function world()
	{
		echo "World";
	}
	
	abstract function foo();
/*	{
		//return "Foo";
	}*/
}

class Rahaman extends Mahabub{
	public function hello()
	{
		echo "Hello ";
	}
	
	public function foo()
	{
		return "Foo ";
	}
}

trait Mahabub{
	public function hello()
	{
		echo "Hello ";
	}
}

trait Rahaman1{
	public function world()
	{
		echo "World";
	}
}

class MyHelloWorld{
	use Mahabub, Rahaman;
	
	public function sayExclamationWorld()
	{
		echo "!";
	}
}

$obj = new Rahaman();
$obj->hello();
echo $obj->foo();

?>
