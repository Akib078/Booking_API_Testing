# Booking_API_Testing

Postman Documentation: https://documenter.getpostman.com/view/38964101/2sAY4siPwv

Base URL: https://restful-booker.herokuapp.com

Tools Used: Postman, JavaScript, Newman. 

•	Conducted POST, GET, PUT, DELETE operations on the API in Postman and verified the status codes.

•	Wrote automation scripts and cases using JS to reduce testing time and generated report using Newman. 

Test Documentation:

i. PUT
Update Booking
https://restful-booker.herokuapp.com/booking/
HEADERS
Cookie
token=

Body
raw (json)
json
{
  "firstname" : "Akkib",
  "lastname" : "RRR",
  "totalprice" : 111,
  "depositpaid" : true,
  "bookingdates" : {
    "checkin" : "2018-01-01",
    "checkout" : "2019-01-01"
  },
  "additionalneeds" : "Breakfast"
}
Example Request
Update Booking
View More
curl
curl --location --request PUT 'https://restful-booker.herokuapp.com/booking/' \
--header 'Cookie: token=' \
--data '{
  "firstname" : "Akkib",
  "lastname" : "RRR",
  "totalprice" : 111,
  "depositpaid" : true,
  "bookingdates" : {
    "checkin" : "2018-01-01",
    "checkout" : "2019-01-01"
  },
  "additionalneeds" : "Breakfast"
}'
Example Response
Body
Headers (0)
No response body
This request doesn't return any response body

ii. GET
Verify Updates
https://restful-booker.herokuapp.com/booking/

Newman Report: 

![Report Screenshot](https://github.com/user-attachments/assets/499fe384-af09-487c-af62-8426e1235c6c)


