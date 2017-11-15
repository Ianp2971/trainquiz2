# trainquiz2
<!DOCTYPE html>
<html lang="en">
<h1>Main Menu</h1>
<head>
	<title>train quiz</title>
	<meta name="description" content="A simple interactive quiz for web pages using HTML, CSS, and jQuery">
	<meta name="author" content="Alan Simpson">
	<!-- I've intentionally put all the code in one file and kept it simple for the benefit
	of students who are just learning this stuff. -->
	<style>
		body {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
			font-size: 14pt;
		}

		#wrapper {
			width: 80%;
			padding: 1%;
			margin: 1em auto;
			border: solid 1px silver;
		}
		/* Text of the questions */
		.question p:first-child {
			font-weight: bold;
		}

		/* Each possible answer */
		.ans {
			margin-left: 10px;

		/* Take hidden feedback out of hiding when applied */
		.show {
		display: block;
		{
	</style>

	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
</head>
<body>
<p>To start quiz on Chrome
<form action="questions 1 and 2.html">
<input type="submit" value="Go to start of quiz">
</form>
</body>

<!DOCTYPE html>
<html lang="en">

<head>
	<title>Interective Quiz</title>
	<meta name="description" content="A simple interactive quiz for web pages using HTML, CSS, and jQuery">
	<meta name="author" content="Alan Simpson">
	<!-- I've intentionally put all the code in one file and kept it simple for the benefit
	of students who are just learning this stuff. -->
	<style>
		body {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
			font-size: 14pt;
		}

		#wrapper {
			width: 80%;
			padding: 1%;
			margin: 1em auto;
			border: solid 1px silver;
		}
		/* Text of the questions */
		.question p:first-child {
			font-weight: bold;
		}

		/* Each possible answer */
		.ans {
			margin-left: 10px;
		}
		/* Answer feedback */
		.ans span {
			display: none;
			margin-left: 20px;
			padding-top: 0.5em;
		}

		/* Take hidden feedback out of hiding when applied */
		.show {
		display: block;
		{
	</style>

	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script>
		$(document).ready(function () {
			$("p.ans").click(function () {
				//Get the id of the div
				var qnum = "#" + $(this).parent().attr("id");
				//Clear previous freeback:
				$(qnum + " p.ans").removeClass("right wrong");
				$(qnum + " p span").css("display", "none");
				//Apply right or wrong class to p and span.
				var applyclass = "wrong"
				var spancolor = "red"
				if ($(this).hasClass("correct")) {
					applyclass = "right";
					spancolor = "green"
				}
				$(this).addClass(applyclass);
				$(this).children(":first").css("display", "block").css("color", spancolor);
			})
		});
	</script>
</head>

<body>
	<div id="wrapper">
		<!-- Each question should be in its own div with a unique ID like q1, q2, and so forth -->
		<!-- Each optional answer has a class of "ans" and the correct answer (only) has an additional class of "correct" -->
		<!-- Use p tags the question and for each answer -->
		<div class="question" id="q1">
			<p>1. who is the manager of CrossCountry?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
		<div class="question" id="q2">
			<p>2. who is the manager of London Midland?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
			<form action="questions 3 and 4.html">
<input type="submit" value="Go to the next two questions">
</form>
	</div>
	<!-- Images -->

	</p>

	
</body>

</html>

<!DOCTYPE html>
<html lang="en">

<head>
	<title>Interective Quiz</title>
	<meta name="description" content="A simple interactive quiz for web pages using HTML, CSS, and jQuery">
	<meta name="author" content="Alan Simpson">
	<!-- I've intentionally put all the code in one file and kept it simple for the benefit
	of students who are just learning this stuff. -->
	<style>
		body {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
			font-size: 14pt;
		}

		#wrapper {
			width: 80%;
			padding: 1%;
			margin: 1em auto;
			border: solid 1px silver;
		}
		/* Text of the questions */
		.question p:first-child {
			font-weight: bold;
		}

		/* Each possible answer */
		.ans {
			margin-left: 10px;
		}
		/* Answer feedback */
		.ans span {
			display: none;
			margin-left: 20px;
			padding-top: 0.5em;
		}

		/* Take hidden feedback out of hiding when applied */
		.show {
		display: block;
		{
	</style>

	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script>
		$(document).ready(function () {
			$("p.ans").click(function () {
				//Get the id of the div
				var qnum = "#" + $(this).parent().attr("id");
				//Clear previous freeback:
				$(qnum + " p.ans").removeClass("right wrong");
				$(qnum + " p span").css("display", "none");
				//Apply right or wrong class to p and span.
				var applyclass = "wrong"
				var spancolor = "red"
				if ($(this).hasClass("correct")) {
					applyclass = "right";
					spancolor = "green"
				}
				$(this).addClass(applyclass);
				$(this).children(":first").css("display", "block").css("color", spancolor);
			})
		});
	</script>
</head>

<body>
	<div id="wrapper">
		<!-- Each question should be in its own div with a unique ID like q1, q2, and so forth -->
		<!-- Each optional answer has a class of "ans" and the correct answer (only) has an additional class of "correct" -->
		<!-- Use p tags the question and for each answer -->
		<div class="question" id="q3">
			<p>3. who is the manager of Virgin Trains?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
		<div class="question" id="q4">
			<p>4. How many trains does london midlands have on the tracks at rush hour?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
			<form action="questions 5 and 6.html">
<input type="submit" value="Go to the next two questions">
</form>

<!DOCTYPE html>
<html lang="en">

<head>
	<title>Interective Quiz</title>
	<meta name="description" content="A simple interactive quiz for web pages using HTML, CSS, and jQuery">
	<meta name="author" content="Alan Simpson">
	<!-- I've intentionally put all the code in one file and kept it simple for the benefit
	of students who are just learning this stuff. -->
	<style>
		body {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
			font-size: 14pt;
		}

		#wrapper {
			width: 80%;
			padding: 1%;
			margin: 1em auto;
			border: solid 1px silver;
		}
		/* Text of the questions */
		.question p:first-child {
			font-weight: bold;
		}

		/* Each possible answer */
		.ans {
			margin-left: 10px;
		}
		/* Answer feedback */
		.ans span {
			display: none;
			margin-left: 20px;
			padding-top: 0.5em;
		}

		/* Take hidden feedback out of hiding when applied */
		.show {
		display: block;
		{
	</style>

	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script>
		$(document).ready(function () {
			$("p.ans").click(function () {
				//Get the id of the div
				var qnum = "#" + $(this).parent().attr("id");
				//Clear previous freeback:
				$(qnum + " p.ans").removeClass("right wrong");
				$(qnum + " p span").css("display", "none");
				//Apply right or wrong class to p and span.
				var applyclass = "wrong"
				var spancolor = "red"
				if ($(this).hasClass("correct")) {
					applyclass = "right";
					spancolor = "green"
				}
				$(this).addClass(applyclass);
				$(this).children(":first").css("display", "block").css("color", spancolor);
			})
		});
	</script>
</head>

<body>
	<div id="wrapper">
		<!-- Each question should be in its own div with a unique ID like q1, q2, and so forth -->
		<!-- Each optional answer has a class of "ans" and the correct answer (only) has an additional class of "correct" -->
		<!-- Use p tags the question and for each answer -->
		<div class="question" id="q5">
			<p>5. how many trains do london midlands have?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
		<div class="question" id="q6">
			<p>6. how many trains do virgin train have?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
			<form action="questions 7 and 8.html">
		<input type="submit" value="Go to the next two questions">
		</form>
</body>

<!DOCTYPE html>
<html lang="en">

<head>
	<title>Interective Quiz</title>
	<meta name="description" content="A simple interactive quiz for web pages using HTML, CSS, and jQuery">
	<meta name="author" content="Alan Simpson">
	<!-- I've intentionally put all the code in one file and kept it simple for the benefit
	of students who are just learning this stuff. -->
	<style>
		body {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
			font-size: 14pt;
		}

		#wrapper {
			width: 80%;
			padding: 1%;
			margin: 1em auto;
			border: solid 1px silver;
		}
		/* Text of the questions */
		.question p:first-child {
			font-weight: bold;
		}

		/* Each possible answer */
		.ans {
			margin-left: 10px;
		}
		/* Answer feedback */
		.ans span {
			display: none;
			margin-left: 20px;
			padding-top: 0.5em;
		}

		/* Take hidden feedback out of hiding when applied */
		.show {
		display: block;
		{
	</style>

	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script>
		$(document).ready(function () {
			$("p.ans").click(function () {
				//Get the id of the div
				var qnum = "#" + $(this).parent().attr("id");
				//Clear previous freeback:
				$(qnum + " p.ans").removeClass("right wrong");
				$(qnum + " p span").css("display", "none");
				//Apply right or wrong class to p and span.
				var applyclass = "wrong"
				var spancolor = "red"
				if ($(this).hasClass("correct")) {
					applyclass = "right";
					spancolor = "green"
				}
				$(this).addClass(applyclass);
				$(this).children(":first").css("display", "block").css("color", spancolor);
			})
		});
	</script>
</head>

<body>
	<div id="wrapper">
		<!-- Each question should be in its own div with a unique ID like q1, q2, and so forth -->
		<!-- Each optional answer has a class of "ans" and the correct answer (only) has an additional class of "correct" -->
		<!-- Use p tags the question and for each answer -->
		<div class="question" id="q7">
			<p>7. how many trains do CrossCountry have?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
		<div class="question" id="q8">
			<p>8. how many trains do Chiltern Railways have?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
			<form action="questions 9 and 10.html">
<input type="submit" value="Go to the next two questions">
</form>
</body>

<!DOCTYPE html>
<html lang="en">

<head>
	<title>Interective Quiz</title>
	<meta name="description" content="A simple interactive quiz for web pages using HTML, CSS, and jQuery">
	<meta name="author" content="Alan Simpson">
	<!-- I've intentionally put all the code in one file and kept it simple for the benefit
	of students who are just learning this stuff. -->
	<style>
		body {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
			font-size: 14pt;
		}

		#wrapper {
			width: 80%;
			padding: 1%;
			margin: 1em auto;
			border: solid 1px silver;
		}
		/* Text of the questions */
		.question p:first-child {
			font-weight: bold;
		}

		/* Each possible answer */
		.ans {
			margin-left: 10px;
		}
		/* Answer feedback */
		.ans span {
			display: none;
			margin-left: 20px;
			padding-top: 0.5em;
		}

		/* Take hidden feedback out of hiding when applied */
		.show {
			display: block;
		}
	</style>

	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script>
		$(document).ready(function () {
			$("p.ans").click(function () {
				//Get the id of the div
				var qnum = "#" + $(this).parent().attr("id");
				//Clear previous freeback:
				$(qnum + " p.ans").removeClass("right wrong");
				$(qnum + " p span").css("display", "none");
				//Apply right or wrong class to p and span.
				var applyclass = "wrong"
				var spancolor = "red"
				if ($(this).hasClass("correct")) {
					applyclass = "right";
					spancolor = "green"
				}
				$(this).addClass(applyclass);
				$(this).children(":first").css("display", "block").css("color", spancolor);
			})
		});
	</script>
</head>

<body>
	<div id="wrapper">
		<!-- Each question should be in its own div with a unique ID like q1, q2, and so forth -->
		<!-- Each optional answer has a class of "ans" and the correct answer (only) has an additional class of "correct" -->
		<!-- Use p tags the question and for each answer -->
		<div class="question" id="q9">
			<p>9. How many stations on the east coast railway?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
		<div class="question" id="q10">
			<p>10. How many trains do Greater Anglia have?</p>
			<input type="text" name="Answer" id="Answer" size="20" maxlength="15">
		</div>
			<form action="Thank you screen1.html">
<input type="submit" value="Go to Thank you screen">
</form>

<doctype>
<html lang="en">

<head>
	<title>Thank you screen</title>
	<meta name="description" content="A simple interactive quiz for web pages using HTML, CSS, and jQuery">
	<meta name="author" content="Alan Simpson">
	<!-- I've intentionally put all the code in one file and kept it simple for the benefit
	of students who are just learning this stuff. -->
	<style>
		body {
			font-family: Verdana, Geneva, Tahoma, sans-serif;
	</style>
	<body>
		<h1>Thank you for doing my quiz
		<h2>If you dont mind please can you do a review of my quiz on either one of this links
		<h3><a href="https://www.surveylegend.com/s/gq1">Visit surveylegend</a>
		<h4><a href="https://survey.zohopublic.com/zs/79CujB">Visit survey</a>
		<h5><a href="https://docs.google.com/forms/d/e/1FAIpQLSeCU3tSp6iy2JewMAG6J0wvk6-cl-x2ojAyjKP5LY-ha6V4Pw/viewform?usp=sf_link">Visit google forms</a>
    </div>
</html>
