OverdueMemberCalculator
=======================

Generates a paypal button based on the URL.

I'm using it to dynamically create payment buttons for overdue members at my local hackerspace.

4 parameters are required in the URL:
*email - URI encoded email address of your paypal account
*lastPaidYear - 4 digit year of when the member last paid (example: 2012)
*lastPaidMonth - month the member last paid (use numbers 1-12)
*lastPaidDay - date the person last paid (use numbers 1-31)
*membershipPrice - price of your membership dues (I've only tested this with whole numbers)

Example of a complete URL:
http://dallasmakerspace.org/misc/button.html?email=paypalalerts%40dallasmakerspace.org&lastPaidYear=2011&lastPaidMonth=1&lastPaidDay=2&membershipPrice=50&memberName=Jesus
'
