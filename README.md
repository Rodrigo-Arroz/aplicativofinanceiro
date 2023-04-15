<!DOCTYPE html>
<html>
<head>
  <title>Meu Aplicativo de Investimentos</title>
</head>
<body>
  <header>
    <!-- Coloque o seu logo aqui -->
    <h1>Meu Aplicativo de Investimentos</h1>
  </header>
  <section id="login">
    <h2>Login</h2>
    <form id="login-form">
      <label for="email">Email:</label>
      <input type="email" id="email" name="email">
      <label for="senha">Senha:</label>
      <input type="password" id="senha" name="senha">
      <input type="submit" value="Entrar">
    </form>
  </section>
  <section id="fundos-imobiliarios" style="display: none;">
    <h2>Fundos Imobiliários</h2>
    <!-- Coloque a lista de fundos imobiliários aqui -->
    <ul>
      <li>Nome do Fundo 1 - Dividendo Yield: X% | Preço: R$X | Variação do Dia: X% | Volume: X</li>
      <li>Nome do Fundo 2 - Dividendo Yield: X% | Preço: R$X | Variação do Dia: X% | Volume: X</li>
      <!-- Outros fundos imobiliários -->
    </ul>
  </section>
  <section id="renda-fixa" style="display: none;">
    <h2>Renda Fixa</h2>
    <!-- Coloque a lista de opções de renda fixa aqui -->
    <ul>
      <li>Opção de Renda Fixa 1</li>
      <li>Opção de Renda Fixa 2</li>
      <!-- Outras opções de renda fixa -->
    </ul>
  </section>
  <section id="renda-variavel" style="display: none;">
    <h2>Renda Variável</h2>
    <!-- Coloque a lista de opções de renda variável aqui -->
    <ul>
      <li>Opção de Renda Variável 1</li>
      <li>Opção de Renda Variável 2</li>
      <!-- Outras opções de renda variável -->
    </ul>
  </section>
  <footer>
    <!-- Coloque informações de rodapé aqui -->
    <p>Informações de rodapé</p>
  </footer>

  <script>
    document.getElementById('login-form').addEventListener('submit', function(event) {
      event.preventDefault(); // Previne o envio do formulário
      // Aqui você pode adicionar a lógica de verificação do login e senha
      // Se o login for bem-sucedido, você pode mostrar as outras seções usando display: block;
      document.getElementById('fundos-imobiliarios').style.display = 'block';
      document.getElementById('renda-fixa').style.display = 'block';
      document.getElementById('renda-variavel').style.display = 'block';
    });
  </script>
</body>
</html>
