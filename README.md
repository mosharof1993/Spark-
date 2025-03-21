<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SPARK Financial System</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>SPARK Financial System</h1>
        <button onclick="logout()">Logout</button>
    </header>

    <div id="login-container">
        <h2>Login</h2>
        <input type="text" id="username" placeholder="Enter Username">
        <input type="password" id="password" placeholder="Enter Password">
        <button onclick="login()">Login</button>
    </div>

    <div id="app-container" style="display: none;">
        <h2>Income & Expense Management</h2>
        <input type="number" id="income" placeholder="Enter Income Amount">
        <input type="number" id="expense" placeholder="Enter Expense Amount">
        <button onclick="calculateBalance()">Calculate</button>

        <div class="summary">
            <h3>Total Income: <span id="totalIncome">0</span> BDT</h3>
            <h3>Total Expense: <span id="totalExpense">0</span> BDT</h3>
            <h3>Balance: <span id="balance">0</span> BDT</h3>
        </div>

        <button onclick="downloadPDF()">Download Report</button>
    </div>

    <script src="script.js"></script>
</body>
</html>
