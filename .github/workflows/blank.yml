<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Đặt lịch sạc - PIT8 STATION</title>
  <style>
    @font-face {
      font-family: 'Ethnocentric';
      src: url('https://cdn.jsdelivr.net/gh/itfoundry/ethnocentric/Ethnocentric-Regular.otf') format('opentype');
    }

    body {
      font-family: sans-serif;
      background: #f2f6fc;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 480px;
      margin: 50px auto;
      background: #fff;
      padding: 30px;
      border-radius: 16px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      text-align: center;
    }

    h1 {
      font-size: 28px;
      margin-bottom: 20px;
    }

    .highlight {
      color: #1c9e54;
      font-family: 'Ethnocentric', sans-serif;
      font-size: 32px;
      display: block;
      margin-top: 8px;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    form input,
    form button {
      display: block;
      width: 100%;
      padding: 12px;
      margin-bottom: 16px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 16px;
    }

    form button {
      background-color: #1c9e54;
      color: white;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.3s;
    }

    form button:hover {
      background-color: #158a45;
    }

    .hidden {
      display: none;
    }

    #confirmation {
      margin-top: 30px;
      padding: 20px;
      background-color: #e0f8e9;
      border: 1px solid #b6e2c5;
      border-radius: 12px;
      color: #1c6e35;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Đặt lịch sạc tại <span class="highlight">PIT8 STATION</span></h1>
    
    <form id="bookingForm">
      <input type="text" placeholder="Họ và tên" id="name" required />
      <input type="tel" placeholder="Số điện thoại" id="phone" required />
      <input type="text" placeholder="Loại phương tiện (VD: VinFast VF8)" id="vehicle" required />
      <input type="date" id="date" required />
      <input type="time" id="time" required />
      
      <button type="submit">Xác nhận đặt lịch</button>
    </form>

    <div id="confirmation" class="hidden">
      <h2>✅ Đặt lịch thành công!</h2>
      <p id="confirmText"></p>
    </div>
  </div>

  <script>
    const form = document.getElementById('bookingForm');
    const confirmation = document.getElementById('confirmation');
    const confirmText = document.getElementById('confirmText');

    form.addEventListener('submit', function(e) {
      e.preventDefault();
      const name = document.getElementById('name').value;
      const phone = document.getElementById('phone').value;
      const vehicle = document.getElementById('vehicle').value;
      const date = document.getElementById('date').value;
      const time = document.getElementById('time').value;

      if (name && phone && vehicle && date && time) {
        confirmText.textContent = `Cảm ơn ${name}! Hẹn gặp bạn tại PIT8 STATION vào lúc ${time} ngày ${date}.`;
        confirmation.classList.remove('hidden');
        form.classList.add('hidden');
      }
    });
  </script>
</body>
</html>
