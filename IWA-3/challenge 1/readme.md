# IWA_3.3: Challenge 1
The code below should render the initial HTML, after which it should run the JavaScript code that replaces Loading... with a dynamic copyright message. It is important to keep the configuration values in a separate file for easy editing. However, at the moment the footer never changes from the initial Loading... state.

 

To complete this challenge, answer the following:

Why does the code not work?
What changes do you need to make to achieve the intended behaviour?
Are there any other ways in which it can be been solved?
 
``` js
// configuration.js

const company = 'ACME Inc.'
const year = 2022
 

// scripts.js

import company form 'configuration'
import year form 'configuration'

const message = '© ' + company + ' (' + year + ')'
document.querySelector('footer').innerText = message
 ```

``` html
<!-- index.html -->

<html>
	<head>
		<scripts scr="./scripts">
  </head>

	<body>
		<h1>Welcome</h1>
		<p>This is our website</p>
	</body>

	<footer>Loading...</footer>
</html>
```
## Why does the code not work?
* the configuration.js script is not properly exporting its funstions to the main script
  the main .js script is incorrectly linked in the html
## What changes do you need to make to achieve the intended behaviour?
* create a 2nd .js file with the confiurations code inside than properly export it to the script.js file
  then import the code being exported from configuration.js so that it can be recognized in the script.js file correctly
* dont forget to state src="script.js" type="module" when using the import/export feature in javascript
Are there any other ways in which it can be been solved?
* their are ways to shorten the code instead of listing all the import and exports individually