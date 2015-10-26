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

$obj = new Rahaman();
$obj->hello();
echo $obj->foo();

?>
