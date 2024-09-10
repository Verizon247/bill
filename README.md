<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Verizon - Login & Bill Summary</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f6f6f6;
            margin: 0;
            padding: 0;
        }
        .header {
            background-color: white;
            padding: 10px;
            text-align: center;
            font-size: 24px;
            color: #d51a2d;
        }
        .container {
            width: 100%;
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: white;
            border: 1px solid #ddd;
            border-radius: 10px;
        }
        .hidden {
            display: none;
        }
        /* Login Page Styles */
        .login-form {
            margin-top: 50px;
        }
        .login-form label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        .login-form input {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .login-form button {
            width: 100%;
            padding: 10px;
            background-color: #d51a2d;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
        }
        .login-form button:hover {
            background-color: #b11421;
        }
        .error {
            color: red;
            font-size: 14px;
        }
        /* Chat Button */
        .chat-button {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #333;
            color: white;
            padding: 10px 20px;
            border-radius: 50px;
            cursor: pointer;
        }
        .chat-popup {
            position: fixed;
            bottom: 80px;
            right: 20px;
            background-color: white;
            border: 1px solid #ccc;
            padding: 10px;
            border-radius: 5px;
            display: none;
        }
        .chat-popup p {
            margin: 0;
            font-size: 14px;
        }
        /* Bill Summary Styles */
        .bill-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 20px;
        }
        .bill-header .account-details {
            font-size: 14px;
            color: #333;
        }
        .bill-header .account-details strong {
            display: block;
        }
        .bill-header .bill-amount {
            font-size: 24px;
            font-weight: bold;
            color: #333;
        }
        .profile-section {
            text-align: left;
            margin-bottom: 20px;
            font-size: 14px;
            color: #333;
        }
        .profile-section strong {
            display: block;
            font-size: 16px;
        }
        .activity, .summary {
            margin-bottom: 30px;
        }
        .activity ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }
        .activity ul li {
            margin-bottom: 5px;
            font-size: 14px;
            color: #333;
        }
        .bill-summary-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
        .bill-summary-table th, .bill-summary-table td {
            text-align: left;
            padding: 10px;
            border-bottom: 1px solid #ddd;
        }
        .bill-summary-table th {
            background-color: #f6f6f6;
        }
        .bill-summary-table td:last-child {
            text-align: right;
        }
        .total-row {
            font-weight: bold;
            font-size: 16px;
            background-color: #f6f6f6;
        }
        .questions, .review, .surcharges {
            margin-top: 20px;
            font-size: 14px;
            color: #333;
        }
        .review a, .questions a {
            color: #0066cc;
            text-decoration: none;
        }
        .review a:hover, .questions a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Verizon Header Example</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }
        /* Header styles */
        .verizon-header {
            background-color: white;
            border-bottom: 1px solid #ddd;
            padding: 10px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-left: 50px;
            padding-right: 50px;
        }

        .verizon-header .left-links {
            display: flex;
            align-items: center;
        }

        .verizon-header .left-links a {
            color: #000;
            text-decoration: none;
            margin-right: 20px;
            font-size: 14px;
        }

        .verizon-header .logo {
            font-weight: bold;
            color: #e80000;
            font-size: 24px;
        }

        .verizon-header .nav-links a {
            text-decoration: none;
            color: black;
            margin: 0 10px;
            font-size: 14px;
        }

        .verizon-header .right-links {
            display: flex;
            align-items: center;
        }

        .verizon-header .right-links a {
            margin-left: 20px;
            font-size: 14px;
            text-decoration: none;
            color: #000;
        }

        .verizon-header .search-box {
            border: 1px solid #ccc;
            border-radius: 50px;
            padding: 5px 10px;
            display: flex;
            align-items: center;
        }

        .verizon-header .search-box input {
            border: none;
            outline: none;
            font-size: 14px;
            padding-left: 5px;
        }

        .verizon-header .search-box button {
            background: none;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <!-- Verizon Header Section -->
    <div class="verizon-header">
        <div class="left-links">
            <span class="logo">Verizon</span>


            
            <a href="#">Personal</a>
            <a href="#">Business</a>
        </div>
        <div class="nav-links">
            <a href="#">Mobile</a>
            <a href="#">Home Internet</a>
            <a href="#">Shop</a>
            <a href="#">Deals</a>
        </div>
        <div class="right-links">
            <a href="tel:1-833-VERIZON">1-833-VERIZON</a>
            <a href="#">Contact Us</a>
            <a href="#">Support</a>
            <a href="#">Stores</a>
            <a href="#">Coverage Map</a>
            <a href="#">Español</a>

            
            <div class="search-box">
                <input type="text" placeholder="Search Verizon">
                <button>🔍</button>
            </div>
            <a href="#">Sign in</a>
            <a href="#">🛒</a>
        </div>
    </div>

    <!-- Header -->
    <div class="header">
        <strong>Verizon</strong>
        <p>Get up to $540 when you bring your own phone. Or get iPhone 15 on us. Online only. No trade-in req'd. Buy | Details</p>
    </div>

    <!-- Login Page -->
    <div class="container" id="loginPage">
        <h2>Sign in</h2>
        <p>New customer? <a href="#">Create new account</a></p>
        <form class="login-form" onsubmit="return validateLogin(event)">
            <label for="userId">User ID or Verizon mobile number</label>
            <input type="text" id="userId" placeholder="Enter your mobile number">
            <div class="error" id="error" style="display: none;">Invalid User ID or Mobile Number</div>
            <button type="submit">Continue</button>
        </form>
    </div>

    <!-- Bill Summary Page -->
    <div class="container hidden" id="billPage">
        <!-- Profile Section -->
        <div class="profile-section">
            <strong>Name: Vina Sky</strong>
            <strong>Stefanvina9@gmail.com</strong>
        </div>

        <div class="bill-header">
            <div class="account-details">
                <strong>Account:</strong> 5833907143-67342 <br>
                <strong>Invoice:</strong> 0761997645 <br>
                <strong>Billing period:</strong> Aug - Aug 25, 2024
            </div>
            <div class="bill-amount">
                Your August bill is <br> $2474.28 <br> Due Aug 30
            </div>
        </div>

        <!-- Activity since last bill -->
        <div class="activity">
            <h3>Activity since your last bill</h3>
            <ul>
                <li>✅ You paid $306.48 and used $10 Verizon Dollars.</li>
                <li>✅ Your bill increased by $40.00.</li>
                <li>✅ You saved 58.60 with discounts.</li>
                <li>✅ 6.21GB used, 17.9GB carried over to the next month.</li>
            </ul>
        </div>

        <!-- Bill Summary -->
        <div class="summary">
            <h3>Bill summary</h3>
            <table class="bill-summary-table">
                <tr>
                    <th>One-time credits</th>
                    <td>-58.60</td>
                </tr>
                <tr>
                    <th>One-time charges</th>
                    <td>$40.00</td>
                </tr>
                <tr>
                    <th>Plans</th>
                    <td>$110.30</td>
                </tr>
                <tr>
                    <th>Devices</th>
                    <td>$2160.29</td>
                </tr>
                <tr>
                    <th>Apps & add-ons</th>
                    <td>$31.00</td>
                </tr>
                <tr>
                    <th>Surcharges</th>
                    <td>$48.40</td>
                </tr>
                <tr>
                    <th>Taxes & gov fees</th>
                    <td>$26.09</td>
                </tr>
                <tr class="total-row">
                    <th>Total</th>
                    <td>$2474.28</td>
                </tr>
            </table>
        </div>

        <!-- Questions about bill -->
        <div class="questions">
            <strong>Questions about your bill?</strong><br>
            <a href="#">verizon.com/support</a> or call 800-922-0204
        </div>

        <!-- Review bill details -->
        <div class="review">
            <strong>Review bill details</strong><br>
            My Verizon app <br>
            Download the app on <a href="#">Google Play</a> or <a href="#">Apple Store</a>
        </div>

        <!-- Surcharges info -->
        <div class="surcharges">
            <strong>Surcharges, taxes and gov fees:</strong> The total amount due for this month includes surcharges of $28.60 and taxes and gov fees of $6.09. 
            For an itemized list of taxes, fees, and surcharges visit <a href="#">verizon.com/mybill</a>.
        </div>
    </div>

    <!-- Footer Section -->
    <footer class="container">
        <div class="footer-links">
            <a href="#">Site Map</a> | <a href="#">Privacy Policy</a> | <a href="#">California Privacy Notice</a> | <a href="#">Health Privacy Notice</a> | <a href="#">Your Privacy Choices</a> | 
            <a href="#">Accessibility</a> | <a href="#">Open Internet</a> | <a href="#">Terms & Conditions</a> | <a href="#">About Our Ads</a>
        </div>
    </footer>

    <!-- Chat Button -->
    <div class="chat-button" onclick="toggleChat()">Chat with us</div>

    <!-- Chat Popup -->
    <div class="chat-popup" id="chatPopup">
        <p>Send us a text to chat with us: +1 609-460-8109</p>
    </div>

    <script>
        // Login validation function
        function validateLogin(event) {
            event.preventDefault();
            const userId = document.getElementById('userId').value;
            if (userId === '9168675309') {
                document.getElementById('loginPage').style.display = 'none';
                document.getElementById('billPage').style.display = 'block';
                document.getElementById('error').style.display = 'none';
            } else {
                document.getElementById('error').style.display = 'block';
            }
        }

        // Toggle the chat popup
        function toggleChat() {
            const chatPopup = document.getElementById('chatPopup');
            if (chatPopup.style.display === 'none' || chatPopup.style.display === '') {
                chatPopup.style.display = 'block';
            } else {
                chatPopup.style.display = 'none';
            }
        }
    </script>

</body>
</html>
