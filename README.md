# ipi-6
1.<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Toggle Heading Text</title>
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<style>
    #heading {
        font-size: 24px;
    }
</style>
</head>
<body>

<h1 id="heading">Original Text</h1>
<button id="toggleButton">Toggle Text</button>

<script>
$(document).ready(function(){
    $("#toggleButton").click(function(){
        var currentText = $("#heading").text();
        if(currentText === "Original Text") {
            $("#heading").text("Hello, World!");
        } else {
            $("#heading").text("Original Text");
        }
    });
});
</script>



</body>
</html>

2.<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Count Vowels</title>
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
</head>
<body>

<label for="inputText">Enter a string:</label>
<input type="text" id="inputText">
<button id="countButton">Count Vowels</button>
<p id="result"></p>

<script>
$(document).ready(function(){
    $("#countButton").click(function(){
        var inputString = $("#inputText").val().toLowerCase();
        var vowelCount = 0;
        for(var i = 0; i < inputString.length; i++) {
            if(inputString[i] === 'a' || inputString[i] === 'e' || inputString[i] === 'i' || inputString[i] === 'o' || inputString[i] === 'u') {
                vowelCount++;
            }
        }
        $("#result").text("Number of vowels: " + vowelCount);
    });
});
</script>

</body>
</html>




