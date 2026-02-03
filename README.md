<?php
session_start();
// मान लीजिए लॉगिन फॉर्म से क्रेडेंशियल आए हैं
$username = $_POST['pranav'];
$password = $_POST['1234'];

// सही लॉगिन चेक करें
if ($username == "pranav" && $password == "1234") {
    $_SESSION['loggedin'] = true;
    header("Location: dashboard.php"); // इस पेज पर भेजें
    exit();
} else {
    echo "गलत क्रेडेंशियल!";
}
?>
