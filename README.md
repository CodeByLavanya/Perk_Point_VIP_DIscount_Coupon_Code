1. We will introduce a VIP reward system based on customer tags.
2. VIP Tag &amp; Reward Points
o Customers who have a special “VIP” tag will be eligible for reward points.
o You can add tag in customer level manually.
o When a VIP customer places an order:
 We will listen to the order creation webhook.
 Once the order is successfully placed, reward points will be
credited.
 Points calculation: 2 × order subtotal (for example, ₹1,000 subtotal
= 2,000 points).
3. Redeeming Points in Cart
o When the same VIP customer visits the store again:
 On the cart page, show an input box displaying their available
reward points (perks).
 The customer can enter the number of points they want to redeem.

4. Coupon Generation &amp; Application
o After the customer enters the points to redeem:
 The backend will generate a coupon code for the entered value.
 This coupon will be automatically applied to the cart.
o No need to handle coupon removal logic.
o created coupon code should be used only once and only by that customer
alone.
o Need to validate in backend as well does the point customer trying to
redeem is valid.
5. Excluded Products
o Some special products should not allow coupons.
o If such products are in the cart, the generated coupon should not be
applied.
o Have a option in admin to mark products as special . So while creating
discount code it should exclude these.
