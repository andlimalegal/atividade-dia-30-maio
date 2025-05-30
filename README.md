# atividade-dia-30-maio
/* Reset basico */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f4f4f4;
    color: #333;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  
  header {
    background-color: #4CAF50;
    padding: 15px 0;
  }
  
  .navbar {
    display: flex;
    justify-content: center;
    gap: 30px;
  }
  
  .navbar a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
  }
  
  .navbar a:hover {
    text-decoration: underline;
  }
  
  .container {
    flex: 1;
    max-width: 600px;
    margin: 30px auto;
    padding: 20px;
    background-color: #fff;
    border-radius: 12px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  
  h1 {
    text-align: center;
    margin-bottom: 25px;
    color: #4CAF50;
  }
  
  .form {
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  
  .form label {
    font-weight: bold;
  }
  
  .form input {
    padding: 8px;
    border: 1px solid #ccc;
    border-radius: 6px;
  }
  
  button {
    padding: 10px;
    background-color: #4CAF50;
    color: white;
    font-size: 16px;
    border: none;
    border-radius: 6px;
    cursor: pointer;
  }
  
  button:hover {
    background-color: #45a049;
  }
  
  footer {
    text-align: center;
    padding: 15px 0;
    background-color: #ddd;
    font-size: 14px;
    color: #333;
  }
  
