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