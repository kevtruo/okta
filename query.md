
<ins>**MONITORING USER LOGIN STATUS**<ins>

SUCCESSFUL LOGIN 
`eventType eq "user.session.start" and outcome.result eq "SUCCESS"`

FAILED LOGIN 
`outcome.result eq "FAILURE" and eventType eq "user.authentication.authenticate"`

