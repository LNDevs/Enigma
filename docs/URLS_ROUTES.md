URLS and Routes
=

Routes and/or URLs are listed below, with their responses, request type and other useful information
<table>
<tr><td>ROW</td><td>URL</td><td>HTTP METHOD</td><td>REQUIRED DATA</td><td>RESPONSE TYPE</td><td>RESPONSE DATA</td><td>OTHER</td></tr>
<tr><td>1</td><td>/api/v0/accounts/login</td><td>{ legacyname, password(unhashed) }</td><td>POST + JSON DATA</td><td>JSON {}</td><td>{ account: PublicAccount }</td><td>This url sets a cookie on response as to if you are logged in or not, resets any old cookies, lasts for a set time, 48h</td></tr>
<tr><td>2</td><td>/api/v0/accounts/fetch</td><td>{ legacyname || userid }</td><td>POST + JSON DATA</td><td>JSON {}</td><td>{ account: PublicAccount }</td><td>Responds with an account object which <strong>excludes password and email and other personal data</strong></td></tr>
<tr><td>3</td><td>/api/v0/accounts/post </td><td>{ legacyname: string, displayname: string, password: string }</td><td>POST + JSON DATA</td><td>JSON {}account on the server, returns with an error if an account with this legacyName is already a thing!</td></tr>
<tr><td>4</td><td>/api/v1/messages/fetch</td><td>{ messageid }</td><td>POST + JSON DATA</td><td>JSON {}</td><td>{id: EnigmaID, content: "message limited to a TBD size limit"</td><td>This requires data to retrieve a message</td></tr>
<tr><td>5</td><td>/api/v1/messages/fetch/all</td><td>{ none }</td><td>GET</td><td>JSON {}</td><td>{messages: { (array of messages) } }</td><td>This fetches all messages within a set limit e.g 200 messages</td></tr>
<tr><td>6</td><td>/api/v1/messages/post</td><td>{ content }</td><td>POST + JSON DATA</td><td>JSON {}</td><td>{ sent: boolean }</td><td>Sends a message (POSTs) returns status if sent or not, bool t/f</td></tr>
</table>

[Documentation Index](https://github.com/LNDevs/Enigma/blob/main/README.md)
