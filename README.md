1. We will introduce a VIP reward system based on customer tags.
2. VIP Tag &amp; Reward Points
o Customers who have a special “VIP” tag will be eligible for reward points.
o You can add tag in customer level manually.
o When a VIP customer places an order:<br>
 We will listen to the order creation webhook.<br>
 Once the order is successfully placed, reward points will be
credited.<br>
 Points calculation: 2 × order subtotal (for example, ₹1,000 subtotal
= 2,000 points).

<img width="1439" height="775" alt="Screenshot 2026-01-28 at 9 36 26 AM" src="https://github.com/user-attachments/assets/17a9d61f-fdd8-4e1b-8279-214a4060a97f" />
<img width="1417" height="711" alt="Screenshot 2026-01-28 at 11 29 04 AM" src="https://github.com/user-attachments/assets/2ed2755c-4cf1-451e-99d7-1754e073cfa9" />


4. Redeeming Points in Cart<br>
o When the same VIP customer visits the store again:<br>
 On the cart page, show an input box displaying their available
reward points (perks).<br>
 The customer can enter the number of points they want to redeem.

5. Coupon Generation &amp; Application<br>
o After the customer enters the points to redeem:<br>
 The backend will generate a coupon code for the entered value.<br>
 This coupon will be automatically applied to the cart.<br>
o No need to handle coupon removal logic.<br>
o created coupon code should be used only once and only by that customer
alone.<br>
o Need to validate in backend as well does the point customer trying to
redeem is valid.
6. Excluded Products
o Some special products should not allow coupons.
o If such products are in the cart, the generated coupon should not be
applied.
o Have a option in admin to mark products as special . So while creating
discount code it should exclude these.
<img width="1435" height="819" alt="Screenshot 2026-01-28 at 9 35 54 AM" src="https://github.com/user-attachments/assets/d56bbfb3-11f2-4308-8ec9-6342cf4b12d7" />
