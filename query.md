
**Monitoring User Login Status**

* Successful Login | `eventType eq "user.session.start" and outcome.result eq "SUCCESS"`

* Failed Login | `outcome.result eq "FAILURE" and eventType eq "user.authentication.authenticate"`

* Bad Password | `outcome.reason eq "Authentication failed: bad username or password"`

* User Account Lockouts | `eventType eq "user.account.lock"`
