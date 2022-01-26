<?php
mysql_connect('localhost', 'user', '123') or die(mysql_error());
mysql_select_db('phpajax') or die(mysql_error());

$Nome = $_REQUEST['Nome']
$Sobrenome = $_REQUEST['Sobrenome']
$Hora = $_REQUEST['Hora']
$Dia = $_REQUEST['Dia']

try
{
	$sql = "INSERT INTO dados (Nomebd, Sobrenomebd) VALUES('".trim($Nome, $Sobrenome, $Hora, $Dia)."','".
	$result = mysql_query($sql) or die(mysql_error());

	echo "1"
}

catch (Exception $ex)
{
	echo "0";
	
}
?>
