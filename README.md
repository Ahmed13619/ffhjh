<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>صفحة الدفع</title>
    <style>
        body { font-family: Arial, sans-serif; background-color: #f4f4f4; margin: 0; padding: 0; }
        header { background-color: #4CAF50; color: white; text-align: center; padding: 10px 0; }
        .container { padding: 20px; max-width: 500px; margin: auto; background-color: white; border-radius: 8px; box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); }
        input { width: 100%; padding: 10px; margin: 10px 0; border: 1px solid #ddd; border-radius: 4px; }
        button { background-color: #4CAF50; color: white; padding: 10px; border: none; cursor: pointer; width: 100%; }
        button:hover { background-color: #45a049; }
    </style>
</head>
<body>
    <header>
        <h1>الدفع لشراء الشقة</h1>
    </header>
    <div class="container">
        <form action="/confirm-payment" method="POST">
            <div>
                <label for="cardNumber">رقم البطاقة</label>
                <input type="text" id="cardNumber" name="cardNumber" placeholder="أدخل رقم البطاقة" required>
            </div>
            <div>
                <label for="cardHolder">اسم صاحب البطاقة</label>
                <input type="text" id="cardHolder" name="cardHolder" placeholder="أدخل اسم صاحب البطاقة" required>
            </div>
            <div>
                <label for="expiryDate">تاريخ انتهاء البطاقة</label>
                <input type="text" id="expiryDate" name="expiryDate" placeholder="MM/YY" required>
            </div>
            <div>
                <label for="cvv">رمز الأمان (CVV)</label>
                <input type="text" id="cvv" name="cvv" placeholder="أدخل CVV" required>
            </div>
            <button type="submit">تأكيد الدفع</button>
        </form>
    </div>
</body>
</html>
