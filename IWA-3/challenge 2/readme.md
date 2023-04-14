IWA_3.4: Challenge 2
You have been supplied with the following four JavaScript files and an HTML file. Each JavaScript file corresponds to an individual that is part of the team. Each file should replace its associated Loading... section in the HTML once it loads.

 

The client has requested that each individual’s information is kept in a separate JavaScript file for easier updating/management. However, at the moment nothing is being shown except the Loading... text. You have been requested to fix this, while still separating individual information into separate files.

 

In addition to the above, the browser should also log the following information in the console:

 

Roles: CEO, Intern, Head of Marketing


 
``` js
// nwabisa.js

private firstname = "Nwabisa"
private surname = "Gabe"
public role = "CEO"

private display= firstname + " " + surname + " (" + role + ")"
document.querySelector('#nwabisa').innerText = display
 ```

``` js
// johannes.js

private firstname = "Johannes"
private surname = "Potgieter"
public role = "Intern"

private display= firstname + " " + surname + " (" + role + ")"
document.querySelector('#johannes').innerText = display
 ```

``` js
// alex.js

private firstname = "Alex"
private surname = "Naidoo"
public role = "Head of Marketing"

private display= firstname + " " + surname + " (" + role + ")"
document.querySelector('#alex').innerText = display
 

// scripts.js

console.log('Roles:', nwabisa.role, johanes.role, alex.role)
 ```

``` html
<!-- index.html -->

<html>
    <script module="nwabisa">
    <script module="johannes">
    <script module="alex">
    <script nomodule="scripts">

    <body>
        <h1>Our Team</h1>
        
        <ul>
            <li id="nwabisa">Loading...</li>
            <li id="johannes">Loading...</li>
            <li id="alex">Loading...</li>
        </ul>
    </body>
</html>
```