var wordletter = ['N', 'i', 'c', 'e'];
var guessedletter = ['_', '_', '_', '_'];

function guessletter(letter) {

    var correct = false; 
	var continuetoguess = false;
	
	for (var i = 0; i < 
	
wordletter.length; i++) {
	
	if (wordletter[i] == letter) {
		
		guessedletter[i] = letter;
		
		correct = true;
		
	}
	
	if (guessedletter[i] == '_') {
		
		continuetoguess = true;
		
	}
	
}

if (correct) {
	
	console.log('you found a letter!');
	
console.log(guessedletter.join(''));

    if (!continuetoguess) {
    	
    	console.log('YOU WIN');
    	
    }
    
  } else {
  	
  	console.log ('that is not correct');
  	
  }
  }
  guessletter('N');
  guessletter('i');
  guessletter('p');
  guessletter('c');
  guessletter('e');
