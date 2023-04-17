IWA_2.6: Challenge 3
The following code should print a warning to the console, indicating that security scanning has started. It should also print an info message to the console, informing users that they should wait for the scan to complete before closing the browser. It is important that these comments are kept in the code for context to future developers.

 

Currently, the code fails to even run at all.

 
``` js
// 
It is important to show the following message in order to:
- to assure users
- to scare hackers
- to impress investors
//

console.warn(Security scan starting)

/* It is important to let user know when they can close the page  /*

cnosole.info('Please wait for scan to complete before closing the browser.)
```

## what is wrong with the above code
* the multi line comment is incorrectly typed and is inputed as a single line comment.
  the second comment as an incorrectly placed astrix placed at ln19:69 that is including the console log into the comment,
  console.warn at ln17 is not correct javascript syntax and wont display the inside string
   the string inside ln17 is written as a variable and not as a string
   ln21 is spelt incorrectly and also written as a syntax error