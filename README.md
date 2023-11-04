# baitap_php_nhom4
<?php 
$username = 'root';
$password = '';
$server = 'localhost';
$dbname ='tao';
$connect = new mysqli($server, $username, $password, $dbname);
if ($connect->connect_error) {
	die("không kết nối:" . $conn->connect_error);
exit();
}
$sql = "INSERT INTO hang (MH, tenhang, dongia, soluong) VALUES ('5', 'ao', '200', '20')";
if ($connect->query($sql) ===TRUE) {
echo "them du lieu thanh cong";
} esle {
echo "error: ";
}
$connect->close();
?>
