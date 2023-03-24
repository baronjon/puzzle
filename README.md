# fruity

<!DOCTYPE html>
<html>
<head>
	<title>Word Guessing Game</title>
	<style>
		body {
			font-family: Arial, sans-serif;
			background-color: #f2f2f2;
			text-align: center;
		}
		h1 {
			color: #444444;
		}
		#guesses {
			margin: 20px auto;
			display: flex;
			justify-content: center;
		}
		#guesses input {
			width: 30px;
			height: 30px;
			font-size: 18px;
			text-align: center;
			margin: 0 10px;
			border: none;
			border-radius: 5px;
			background-color: #e2e2e2;
		}
		button {
			font-size: 16px;
			padding: 10px 20px;
			background-color: #3f51b5;
			color: #ffffff;
			border: none;
			border-radius: 5px;
			cursor: pointer;
			margin-top: 20px;
		}
		#result {
			margin-top: 20px;
			font-size: 24px;
			font-weight: bold;
			color: #444444;
		}
	</style>
</head>
<body>
	<h1>Word Guessing Game</h1>
	<p>Guess the secret five-letter word:</p>
	<div id="guesses">
		<input type="text" maxlength="1" />
		<input type="text" maxlength="1" />
		<input type="text" maxlength="1" />
		<input type="text" maxlength="1" />
		<input type="text" maxlength="1" />
		
		
	</div>
	<button onclick="checkGuess()">Check Guess</button>
	<div id="result"></div>

	<script>
		// Define the secret word
		const secretWord = "apple";

		// Function to check the guess
		function checkGuess() {
			// Get the guess from the input fields
			const guess1 = document.querySelector("#guesses input:nth-of-type(1)").value.toLowerCase();
			const guess2 = document.querySelector("#guesses input:nth-of-type(2)").value.toLowerCase();
			const guess3 = document.querySelector("#guesses input:nth-of-type(3)").value.toLowerCase();
			const guess4 = document.querySelector("#guesses input:nth-of-type(4)").value.toLowerCase();
			const guess5 = document.querySelector("#guesses input:nth-of-type(5)").value.toLowerCase();
			const guess = guess1 + guess2 + guess3 + guess4 + guess5;

			// Check if the guess is correct
			if (guess === secretWord) {
				document.querySelector("#result").innerHTML = "Congratulations! You guessed the word!";
				document.querySelector("#result").style.color = "#008000";
			} else {
				document.querySelector("#result").innerHTML = "Sorry, that's not the word.";
				document.querySelector("#result").style.color = "#ff0000";
			}
		}
	</script>
</body>
</html>
