# PHP-Data_Delete-in-Database

<?php 

    $db_id=$_REQUEST['id'];

    $con = mysqli_connect('localhost','root','','student');
    $query = "DELETE FROM std_info WHERE id = $db_id";
    $result = mysqli_query($con,$query);

    if($result){

        header("location: home.php?delete");

    }
    

?>
