# sql_basic-queries
Clear Outstanding of how to retrieve data
In this task, I worked with SQL SELECT statements to retrieve specific data from a table.
I used WHERE conditions with logical operators like AND, OR filter data effectively.
Pattern matching was performed using the LIKE operator, and range filtering using the BETWEEN clause.
I also applied the ORDER BY clause to sort results in ascending or descending order.
These queries helped in understanding data filtering and sorting in real-time scenarios.


select *from guests;
select *from rooms;
select *from bookings;
select *from payments;
select *from services_used;
select *from rooms where RoomID is not null;
select *from rooms where RoomType='Suite' and PricePerNight=5000;
select *from payments where PaymentMethod='UPI' or Amountpaid='3000';
select *from guests where Name like '%a';
select *from guests where Phone like '%0';
select *from payments where AmountPaid between 5000 and 8000;
select *from bookings where CheckInDate between '2025-08-10' and '2025-08-15';
select *from services_used where ServiceID not between 1 and 3;
select Name,Email from guests order by Name;
select *from payments order by Amountpaid desc;
select *from rooms order by RoomType;
select *from services_used order by ServiceDate desc;

