
<ins>**MONITORING USER LOGIN STATUS**<ins>

Successful Login  
`eventType eq "user.session.start" and outcome.result eq "SUCCESS"`

Failed Login   
`outcome.result eq "FAILURE" and eventType eq "user.authentication.authenticate"`

