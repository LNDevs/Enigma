URLS and Routes
=

Routes and/or URLs are listed below, with their responses, request type and other useful information
<table>
<tr><td>ROW</td><td>URL</td><td>HTTP METHOD</td><td>RESPONSE TYPE</td><td>RESPONSE DATA</td><td>OTHER</td></tr>
<tr><td>1</td><td>/api/v0/accounts/login</td><td>POST + JSON DATA</td><td>JSON {}</td><td>{ account: Account, LoginStatus: boolean }</td><td>This url sets a cookie on response as to if you are logged in or not, resets any old cookies, lasts for a set time, TBD</td></tr>
<tr><td>2</td><td>/api/v0/accounts/fetch</td><td>POST + JSON DATA</td><td>JSON {}</td><td>{ account: PublicAccount }</td><td>Responds with an account object which <strong>excludes password and email and other personal data</strong></td></tr>
<tr><td>3</td><td>/api/v0/accounts/post</td><td>POST + JSON DATA {username, email, passwordUnHashed}</td><td>JSON {}</td><td>{ validity: boolean, LoginStatus: boolean }</td><td>This url also sets a cookie on response which denotes your login status</td></tr>
<tr><td>4</td><td></td><td></td><td></td><td></td><td></td></tr>
<tr><td>5</td><td></td><td></td><td></td><td></td><td></td></tr>
<tr><td>6</td><td></td><td></td><td></td><td></td><td></td></tr>
<tr><td>7</td><td></td><td></td><td></td><td></td><td></td></tr>
</table>
