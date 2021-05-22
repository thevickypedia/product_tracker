# Product Tracker
Track availability and price of products across different websites

`whiplash` uses a simple scrapping technique to get prices of products using the product id (passed as arguments) to get
its availability, price and delivery methods. You can also send a notification using 
[AWS SNS](https://docs.aws.amazon.com/sns/latest/dg/welcome.html) which can send a notification message to your phone.

### DevNotes:<br>
For [walmart](https://www.walmart.com/) passing a header dictionary will work in order to prove that you're not a bot
but [amazon](https://amazon.com/) uses cookies to validate if the request is coming through a browser. One can also use,
a `curl` converted script, but I have used `requests-html` library instead.
