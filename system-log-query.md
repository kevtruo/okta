**Monitoring User Login Status**

* Successful Login | `eventType eq "user.session.start" and outcome.result eq "SUCCESS"`

* Failed Login | `outcome.result eq "FAILURE" and eventType eq "user.authentication.authenticate"`

* Bad Password | `outcome.reason eq "Authentication failed: bad username or password"`

* User Account Lockouts | `eventType eq "user.account.lock"`

**Tracking Application Access**

* Successful Application SSO | `eventType eq "user.authentication.sso" and outcome.result eq "SUCCESS"`

* Denied Application Access | `eventType eq "application.policy.sign_on.deny_access"`

**Auditing User and Group Changes**

* New User Creation | `eventType eq "user.lifecycle.create"`

* User Deactivation | `eventType eq "user.lifecycle.deactivate"`
