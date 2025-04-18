# TEst_REpositary_._-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Recommendation Popup</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 50px;
    }
    label, input, button {
      display: block;
      margin-bottom: 10px;
    }
    button {
      padding: 8px 16px;
      font-size: 16px;
      background-color: #007bff;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>

  <h2>Submit a Recommendation</h2>
  <label for="recommendation">Your Recommendation:</label>
  <input type="text" id="recommendation" placeholder="Write something nice...">

  <button onclick="submitRecommendation()">Submit</button>

  <script>
    function submitRecommendation() {
      const input = document.getElementById("recommendation").value;
      if (input.trim() !== "") {
        alert("Thank you for submitting a recommendation!");
        // You could also update the DOM to add the new recommendation here
      } else {
        alert("Please enter a recommendation before submitting.");
      }
    }
  </script>

</body>
</html>
