OverdueMemberCalculator
=======================

Description: 
When your customer's recurring payments are suspended, and you want their due date to stay the same - your only option through the paypal GUI is to give a trial date that ends on their usual payment date. With this page, you can generate a payment button that will charge the customer on their usual due date and ask them to pay what they owe.

whmcs.txt - generates a link inside a WHMCS e-mail template to the OverdueMemberCalculator

I'm using it for overdue members at my local hackerspace.

The following parameters are required in the URL:
 - email - URI encoded email address of your paypal account
 - lastPaidYear - 4 digit year of when the member last paid (example: 2012)
 - lastPaidMonth - month the member last paid (use numbers 1-12)
 - lastPaidDay - date the person last paid (use numbers 1-31)
 - membershipPrice - price of your membership dues (I've only tested this with whole numbers)

Example of a complete URL:

http://dallasmakerspace.org/misc/button.html?email=paypalalert%40dallasmakerspace.org&lastPaidYear=2011&lastPaidMonth=1&lastPaidDay=2&membershipPrice=50

Troubleshooting
 - Problem: "The link you have used to enter the PayPal system is invalid. Please review the link and try again."
 - Solution: Use a correct e-mail address in email parameter. You entered one that isn't valid to paypal.
