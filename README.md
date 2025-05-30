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
  
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Calculo de Salario</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <nav class="navbar">
      <a href="index.html">Home</a>
      <a href="salario.html">Calculo de Salario</a>
      <a href="pagina2.html">Pagina 2</a>
    </nav>
  </header>

  <main class="container">
    <h1>Calculo de Salario</h1>
    <form id="salarioForm" class="form">
      <label for="nome">Nome:</label>
      <input type="text" id="nome" required>

      <label for="idade">Idade:</label>
      <input type="number" id="idade" required>

      <label for="salario">Salario Bruto:</label>
      <input type="number" id="salario" step="0.5" required>

      <label for="dependentes">Numero de Dependentes:</label>
      <input type="number" id="dependentes" required>

      <button type="submit">Calcular</button>
    </form>
  </main>



  <script>
    document.getElementById("salarioForm").addEventListener("submit", function(e) {
      e.preventDefault();

      const nome = document.getElementById("nome").value;
      const idade = parseInt(document.getElementById("idade").value);
      const salarioBruto = parseFloat(document.getElementById("salario").value);
      const dependentes = parseInt(document.getElementById("dependentes").value);

      const bonus = idade > 50 ? 300 : 200;
      const inss = salarioBruto * 0.08;
      const vt = salarioBruto * 0.05;
      const valorDependentes = dependentes * 50;
      const salarioLiquido = salarioBruto - inss - vt + bonus + valorDependentes;

      alert(`Nome: ${nome}\nDependentes: ${dependentes}\nSalario Bruto: R$ ${salarioBruto.toFixed(2)}\nINSS: R$ ${inss.toFixed(2)}\nVT: R$ ${vt.toFixed(2)}\nSalário Líquido: R$ ${salarioLiquido.toFixed(2)}`);
    });
  </script>
</body>
</html>
<link rel="stylesheet" href="pagina 1 css atividade calculo.css">
