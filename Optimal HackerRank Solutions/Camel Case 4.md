
```js
function capitalize(word) {
	const firstLetter = word.charAt(0);
	
	const firstLetterCap = firstLetter.toUpperCase();
	
	const remainingLetters = word.slice(1);
	
	return firstLetterCap + remainingLetters;
}

function splitWord(type, text) {
	if (type === "V") {
		
		let allWords = text.split(/(?=[A-Z])/);
		
		let result = allWords.map((word, i) => {
		
		return word.toLowerCase();
		
		});
		
		console.log(result.join(" "));
		
	} else if (type === "M") {
		
		let allWords = text.split(/(?=[A-Z])/);
		
		let result = allWords.map((word, i) => {
			return word.toLowerCase();
		});
		
		console.log(result.join(" ").replace("()", ""));
		
	} else {
		
		let allWords = text.split(/(?=[A-Z])/);
		
		let result = allWords.map((word, i) => {
			
			return word.toLowerCase();
		});
		console.log(result.join(" "));
	}
}

  

function combineWord(type, text) {
	if (type === "V") {
		let allWords = text.split(" ");
		
		let result = allWords.map((word, i) => {
			if (i === 0) return word;
			
			return capitalize(word);
		});
		console.log(result.join(""));
		
	} else if (type === "M") {
		let allWords = text.split(" ");
		
		let result = allWords.map((word, i) => {
			if (i === 0) return word;
			
			return capitalize(word);
		});
		console.log(result.join("") + "()");
	} else {
		let allWords = text.split(" ");
		
		let result = allWords.map((word) => {
			return capitalize(word);
		});
		console.log(result.join(""));
	}
}

function processData(input) {
	let allData = input.split(/\r?\n/);
	
	for (let i = 0; i < allData.length; i++) {
		let currentLine = allData[i].split(";");
		
		if (currentLine[0] === "S") {
			splitWord(currentLine[1], currentLine[2]);
		} else {
			combineWord(currentLine[1], currentLine[2]);
		}
	}
}
```