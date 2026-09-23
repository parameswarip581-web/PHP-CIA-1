# PHP-CIA-1
Program 
<html>
<head>
<style>
body {
    font-family: Arial;
}
form {
    width: 300px;
    padding: 20px;
    border: 1px solid black;
}
</style>
</head>

<body>

<h2>Simple Calculator</h2>

<form method="post">

Number 1:
<input type="number" name="num1"><br><br>

Number 2:
<input type="number" name="num2"><br><br>

<input type="submit" name="submit" value="Calculate">

</form>

<?php

if(isset($_POST['submit']))
{
    $num1 = $_POST['num1'];
    $num2 = $_POST['num2'];

    $sum = $num1 + $num2;
    $difference = $num1 - $num2;
    $product = $num1 * $num2;
    $quotient = $num1 / $num2;

    echo "Sum: $sum<br>";
    echo "Difference: $difference<br>";
    echo "Product: $product<br>";
    echo "Quotient: $quotient";
}

?>

</body>
</html>

Output:

Simple Calculator

Number 1: [20]

Number 2: [5]

[Calculate]


Sum: 25
Difference: 15
Product: 100
Quotient: 4
