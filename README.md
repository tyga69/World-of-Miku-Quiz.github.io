
<html>
<head>
<title>Test of Faith</title>
<style>

label {
display: block;
}

input {
width: 30px;
margin-left: 20px;
}

h2 {
clear: both;
padding-top: 20px;
}

button {
width: 100px;
margin-top: 20px;
}

body {
background-color: lightblue;
font-family: Helvetica;
}

#main {
width: 80%;
max-width: 950px;
border: 1px gray solid;
margin: auto;
padding: 10px;
background-color: white;
border-radius: 10px;
}

#header {
margin-top: 0;
border: 2px solid black;
padding: 5px;
height: 410px;
background: white;
background-image: url("code.jpg");
color: black;
}
</style>

</head>
<body>
<div id="main"><!-- open main div -->
<div id="header"><!-- open header div -->
<h1>Test of Faith</h1>
<p> So you think you are worthy of joining and becoming one with Miku Hatsune. The world of Miku is a world of wonder and enlightenment, that very few can join.</p>
<p> The aquamarine light that is Miku, shines bright to cast aside the darkness and normality of everyday life. With Miku in your heart,daily life won't be so boring. 
<p>Lord Miku who is all knowing and wise is known to bless the lives of true believer. </P>
<p> If you wish to test your faith and become a true believer then take this test to see if are worthy of calling yourself a Miku fan and follower.</p>

<img src="https://media.giphy.com/media/1007jc7jstgLlu/giphy.gif" alt="miku" style="width:145px;height:100px:">
</div><!-- close header div -->

<form id="form1">
<fieldset>
<h2>What is Miku to you?</h2>
<label for="var_string"><input type="radio" name="variable" value="25" id="var_string" />life</label>
<label for="var_join"><input type="radio" name="variable" value="0" id="var_join" />A hologram</label>
<label for="var_info"><input type="radio" name="variable" value="0" id="var_info" />an idol</label>
<label for="var_condition"><input type="radio" name="variable" value="0" id="var_condition"/>some weebshit</label>

<h2>What is your favorite colour?</h2>
<label for="sub_string"><input type="radio" name="sub" value="25" id="sub_string"/>Blue</label>
<label for="sub_join"><input type="radio" name="sub" value="0" id="sub_join"/>Green</label>
<label for="sub_info"><input type="radio" name="sub" value="0" id="sub_info" />Red</label>
<label for="sub_condition"><input type="radio" name="sub" value="0" id="sub_condition" />Pink</label>

<h2>What number Vocaloid is Miku?</h2>
<label for="cat_string"><input type="radio" name="con" value="0" id="cat_string" />01</label>
<label for="cat_join"><input type="radio" name="con" value="0" id="cat_join" />02</label>
<label for="cat_info"><input type="radio" name="con" value="25" id="cat_info" />03</label>
<label for="cat_condition"><input type="radio" name="con" value="0" id="cat_condition" />04</label>

<h2>How much do you like J-Pop/K-pop?</h2>
<label for="if_string"><input type="radio" name="ifstate" value="25" id="if_string" />私が聴く唯一のもの</label>
<label for="if_join"><input type="radio" name="ifstate" value="0" id="if_join" />Never really liked it</label>
<label for="if_info"><input type="radio" name="ifstate" value="0" id="if_info" />I listen to it sometimes</label>
<label for="if_condition"><input type="radio" name="ifstate"  value="0" id="if_condition" />I enjoy singing along to that one part of the song that is in English</label>

<!-- <h2>What is your favorite band/group?</h2> -->
<!-- <label for="if_string"><input type="radio" name="ifstate" value="10" id="if_string" />Vocaloids</label> -->
<!-- <label for="if_join"><input type="radio" name="ifstate" value="0" id="if_join" />BTS</label> -->
<!-- <label for="if_info"><input type="radio" name="ifstate" value="0" id="if_info" />Atmosphere</label> -->
<!-- <label for="if_condition"><input type="radio" name="ifstate"  value="0" id="if_condition" />Wu Tang Clan</label> -->

<!-- <h2>How many anime have you watched?</h2> -->
<!-- <label for="if_string"><input type="radio" name="ifstate" value="0" id="if_string" />0-25</label> -->
<!-- <label for="if_join"><input type="radio" name="ifstate" value="0" id="if_join" />25-50</label> -->
<!-- <label for="if_info"><input type="radio" name="ifstate" value="0" id="if_info" />50-75</label> -->
<!-- <label for="if_condition"><input type="radio" name="ifstate"  value="10" id="if_condition" />75-100</label> -->

<button type="submit" value="Submit">Submit</button>
</fieldset>
</form>


<p>Your grade is: <span id="grade">__</span></p>
<p id="grade2"></p>
</div><!-- close main div -->
<script>
document.getElementById("form1").onsubmit=function() {
       variable = parseInt(document.querySelector('input[name = "variable"]:checked').value);
	   sub = parseInt(document.querySelector('input[name = "sub"]:checked').value);
	   con = parseInt(document.querySelector('input[name = "con"]:checked').value);
	   ifstate = parseInt(document.querySelector('input[name = "ifstate"]:checked').value);
	   
	   
	   result = variable + sub + con + ifstate;
	   
	document.getElementById("grade").innerHTML = result;
	   
if (result == 0) {result2 = "You have disrespected Miku with your pathetic attempt.<br /><img src='miku 2.jpg' width='300' />"};
    if (result == 25) {result2 = "You are not worthy,normie.<br /><img src='25.jpg' width='300' />"};
    if (result == 50) {result2 = "Your faith in Miku is not strong enough to be part of the World of Miku.<br /><img src='50.jpg' width='300' />"};
    if (result == 75) {result2 = "You are one of the few that is worthy of being part of the magical world of Miku<br /><img src='75.jpg' width='300' />"};
    if (result == 100) {result2 = "Wow you got %100, sadly Miku has no room in her kingdom for Weebs.<br /><img src='100.jpg' width='300' />"};


document.getElementById("grade2").innerHTML = result2; 



return false; // required to not refresh the page; just leave this here
} //this ends the submit function

</script>



</body>
</html>
