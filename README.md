# IT17354516-CSRFProtection-
Synchronizer Token Pattern
1.After creating web application, edit the login function
   -When validating user credentials and creating the session, *generate a random string* and store in memory as *CSRF token*
2.When loading a page request CSRF token from server.
3.When submitting form also send CSRF token derived using JavaScript.
4.Validate CSRF token prior to action requested through POST request.
# 5.Submit the form
6. Validation of CSRF token occurs

Double Submit Cookies Pattern
1.After creating web application, edit the login function.
   -When validating user credentials and creating session, generate a random string and create CSRF cookie to store random string.
  (Secure flaging cookie enables sending it through HTTPS)
2.When loading page retrieve CSRF token from CSRF cookie.
3.When submitting form also send CSRF token derived using JavaScript.
4.Validate CSRF token prior to action requested through POST request.
# 5.Submit the form
6. Validation of CSRF token occurs

