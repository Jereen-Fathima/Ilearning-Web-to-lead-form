<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="Content-type" content="text/html; charset=UTF-8">
    <title>Web-to-Lead Enrollment Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 400px;
            background-color: white;
            padding: 20px;
            margin: 0 auto;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            border-radius: 10px;
        }
        h2 {
            text-align: center;
            color: #4CAF50;
        }
        label {
            font-weight: bold;
            display: block;
            margin-top: 10px;
            color: #333;
        }
        input[type="text"], input[type="email"] {
            width: 100%;
            padding: 8px;
            margin: 5px 0 15px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        input[type="submit"] {
            width: 100%;
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

    <div class="container">
        <h2>Enrollment Form</h2>
        <form action="https://webto.salesforce.com/servlet/servlet.WebToLead?encoding=UTF-8&orgId=00DNS000003kVqI" method="POST">
            
            <!-- Hidden fields for Salesforce Web-to-Lead -->
            <input type="hidden" name="oid" value="00DNS000003kVqI">
            <input type="hidden" name="retURL" value="https://www.google.co.in/">

            <!-- Optional debug fields -->
            <!-- Uncomment for testing -->
            <!-- <input type="hidden" name="debug" value=1> -->
            <!-- <input type="hidden" name="debugEmail" value="jereenfathima@gmail.com"> -->

            <!-- Form fields -->
            <label for="first_name">First Name</label>
            <input id="first_name" name="first_name" type="text" maxlength="40" placeholder="Enter your first name" required>

            <label for="last_name">Last Name</label>
            <input id="last_name" name="last_name" type="text" maxlength="80" placeholder="Enter your last name" required>

            <label for="email">Email</label>
            <input id="email" name="email" type="email" maxlength="80" placeholder="Enter your email" required>

            <label for="company">Company</label>
            <input id="company" name="company" type="text" maxlength="40" placeholder="Enter your company name" required>

            <label for="city">City</label>
            <input id="city" name="city" type="text" maxlength="40" placeholder="Enter your city" required>

            <label for="state">State/Province</label>
            <input id="state" name="state" type="text" maxlength="20" placeholder="Enter your state/province" required>

            <input type="submit" value="Submit">
        </form>
    </div>

</body>
</html>
