# Golden-dhaba
Optional
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Golden Dhaba - Room 1</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #fff8e1;
      margin: 0;
      padding: 0;
    }
    header {
      background: #ffc107;
      padding: 20px;
      text-align: center;
      color: white;
    }
    h1 {
      margin: 0;
    }
    .menu {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 20px;
    }
    .dish {
      background: #fff3cd;
      border-radius: 8px;
      margin: 10px;
      padding: 15px;
      width: 250px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .dish img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      border-radius: 5px;
    }
    .order-btn, .checkout-btn {
      padding: 8px 12px;
      margin-top: 10px;
      background-color: #ff5722;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    .cart {
      text-align: center;
      padding: 20px;
    }
    footer {
      background: #ffc107;
      color: white;
      text-align: center;
      padding: 10px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Golden Dhaba - Room 1</h1>
    <p>Welcome! Order your favorite dishes below.</p>
  </header>

  <div class="menu" id="menu"></div>

  <div class="cart">
    <h2>Your Order</h2>
    <ul id="cartItems"></ul>
    <p>Total: ₹<span id="totalPrice">0</span></p>
    <button class="checkout-btn" onclick="placeOrder()">Place Order
