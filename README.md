<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Student Registration Form</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    form {
      background: white;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      width: 100%;
      max-width: 400px;
    }

    h2 {
      text-align: center;
      margin-bottom: 1rem;
    }

    label {
      display: block;
      margin-top: 1rem;
      margin-bottom: 0.5rem;
    }

    input {
      width: 100%;
      padding: 0.5rem;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      margin-top: 1.5rem;
      width: 100%;
      padding: 0.75rem;
      font-size: 1rem;
      background-color: #007BFF;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>

  <form>
    <h2>Student Registration</h2>

    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" required 
           pattern="[A-Za-z\s]{3,}" 
           title="Name should be at least 3 alphabetic characters" />

    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required 
           placeholder="example@domain.com" />

    <label for="age">Age:</label>
    <input type="number" id="age" name="age" required 
           min="10" max="100" />

    <button type="submit">Register</button>
  </form>

</body>
</html>
