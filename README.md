# index.html
aap chấm điểm cảm xúc
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <title>Chấm điểm cảm xúc</title>
</head>
<body>
  <h1>Chào mừng đến với App cảm xúc</h1>
  <p>Chọn mức độ cảm xúc của bạn từ 1 đến 10:</p>

  <input type="range" min="1" max="10" value="5" id="slider" />
  <p>Điểm cảm xúc: <span id="value">5</span></p>

  <script>
    const slider = document.getElementById("slider");
    const value = document.getElementById("value");
    slider.oninput = () => {
      value.textContent = slider.value;
    };
  </script>
</body>
</html>
