<!DOCTYPE html>
<html>
<head>
  <title>Temperature Monitor</title>
</head>
<body>
  <h1>Current Body Temperature: <span id="temperature"></span> °C</h1>
  <script>
    function updateTemperature() {
      fetch('/get_temp')
        .then(response => response.json())
        .then(data => {
          document.getElementById('temperature').textContent = data.temperature;
        });
    }

    setInterval(updateTemperature, 5000); // Update every 5 seconds
  </script>
</body>
</html>- 👋 Hi, I’m @Mohithm29
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Mohithm29/Mohithm29 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
