# CSRF

>Cross Site Request Forgery is an attack that forces an end user to execute unwanted action on a web application in which they are currently authenticated.

## Prerequisites:
> User should have active session.

## Mitigation

1. CSRF Token: Token is added in hidden form field, unique per session, large random value.
1. Synchronizer Token Pattern
2. Encryption Based Token Pattern
3. Hash Based Token Pattern
4. Same Site Cookie Attribute
5. Double Submit Cookie (Cookie & request parameter).
6. Re-authentication, One-time token, Captcha (Strong CSRF defense).

## Test Cases:

```
1)
2)
```
## Example/POC :

* [CSRF logs the victim into attacker's account](https://hackerone.com/reports/339352)
* [CSRF: add item to victim's cart automatically (starbucks.com - updatecart)](https://hackerone.com/reports/177472)
* [login csrf in analytics.mopub.com](https://hackerone.com/reports/577920)
* [CSRF at (Apply to this program) that lead to submit your request automatic with out any validations] (https://hackerone.com/reports/334253)
