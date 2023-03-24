
<!DOCTYPE html>
<html>
<head>
	<title>Secret Websites</title>
	<link href="https://fonts.googleapis.com/css?family=Montserrat" rel="stylesheet">
	<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css" rel="stylesheet">
	<style>
		body {
			background-color: #f7f7f7;
			font-family: 'Montserrat', sans-serif;
			padding: 50px;
		}

		h1 {
			margin-bottom: 50px;
		}

		form {
			background-color: #fff;
			border-radius: 10px;
			box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
			padding: 30px;
			margin-bottom: 50px;
		}

		input[type=text] {
			padding: 10px;
			font-size: 16px;
			border: 2px solid #ccc;
			border-radius: 5px;
			outline: none;
			width: 70%;
			margin-right: 10px;
		}

		input[type=submit] {
			padding: 10px 20px;
			font-size: 16px;
			background-color: #4CAF50;
			color: #fff;
			border: none;
			border-radius: 5px;
			cursor: pointer;
			transition: all 0.3s ease;
		}

		input[type=submit]:hover {
			background-color: #3e8e41;
		}

		label {
			display: flex;
			align-items: center;
			margin-bottom: 20px;
		}

		.icon {
			font-size: 24px;
			margin-right: 10px;
		}

        #form4 {
            display: none;
        }
	</style>
</head>
<body>
	<h1>Revival</h1>
	<form id="form1">
		<label for="secret1">Secret word 1:</label>
		<input type="text" id="secret1" name="secret1">
		<input type="submit" value="Submit">
	</form>

	<form id="form2">
		<label for="secret2">Secret word 2:</label>
		<input type="text" id="secret2" name="secret2">
		<input type="submit" value="Submit">
	</form>

	<form id="form3">
		<label for="secret3">Secret Word 3:</label>
		<input type="text" id="secret3" name="secret3">
		<input type="submit" value="Submit">
	</form>
	
    <form id="form4">
		<label for="secret4">Enter Final Word To Reveal Birthday Gift:</label>
		<input type="text" id="secret4" name="secret4">
		<input type="submit" value="Submit">
	</form>

	<script>
		const form1 = document.getElementById("form1");
		const secretInput1 = document.getElementById("secret1");

		const form2 = document.getElementById("form2");
		const secretInput2 = document.getElementById("secret2");

		const form3 = document.getElementById("form3");
		const secretInput3 = document.getElementById("secret3");
		
        const form4 = document.getElementById("form4");
		const secretInput4 = document.getElementById("secret4");

		form1.addEventListener("submit", (event) => {
			event.preventDefault();
			const secret1 = secretInput1.value.trim().toLowerCase();
			if (secret1 === "art") {
                window.open("https://mywordle.strivemath.com/?word=hwkhcepiih");
			} else {
				alert("Incorrect secret word, please try again.");
			}
		});

		form2.addEventListener("submit", (event) => {
			event.preventDefault();
			const secret2 = secretInput2.value.trim().toLowerCase();
			if (secret2 === "literature") {
				window.open("https://crosswordlabs.com/embed/clue-2-162");
			} else {
				alert("Incorrect secret word, please try again.");
			}
		});

		form3.addEventListener("submit", (event) => {
			event.preventDefault();
			const secret3 = secretInput3.value.trim().toLowerCase();
			if (secret3 === "music") {
				window.open("https://www.onelook.com/thesaurus/");
                form4.style.display = "block";
                form4.style.backgroundColor = "gold";
                
                
			} else {
				alert("Incorrect secret word, please try again.");
			}
		});
		
        form4.addEventListener("submit", (event) => {
			event.preventDefault();
			const secret4 = secretInput4.value.trim().toLowerCase();
			if (secret4 === "renaissance") {
				window.open("https://beyonce.com");
			} else {
				alert("Incorrect secret word, please try again.");
			}
		});
	</script>
</body>
</html>
