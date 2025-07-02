<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Cadastro de Produtos</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
      background-color: #f5f5f5;
    }
    h1 {
      text-align: center;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 20px;
    }
    th, td {
      border: 1px solid #ccc;
      padding: 8px;
      text-align: left;
    }
    th {
      background-color: #e0e0e0;
    }
    form {
      margin-bottom: 20px;
      background: #fff;
      padding: 15px;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    label, input, button {
      display: block;
      margin-top: 10px;
    }
    input {
      padding: 6px;
      width: 100%;
    }
    .btn {
      background-color: #2196F3;
      color: white;
      padding: 10px;
      border: none;
      margin-top: 15px;
      cursor: pointer;
    }
    .btn:hover {
      background-color: #0b7dda;
    }
  </style>
</head>
<body>
  <h1>Cadastro de Produtos</h1>

  <form id="productForm">
    <label for="name">Nome do Produto:</label>
    <input type="text" id="name" required />

    <label for="description">Descrição:</label>
    <input type="text" id="description" required />

    <label for="price">Preço (R$):</label>
    <input type="number" id="price" step="0.01" required />

    <label for="quantity">Quantidade:</label>
    <input type="number" id="quantity" required />

    <button type="submit" class="btn">Salvar Produto</button>
  </form>

  <table id="productTable">
    <thead>
      <tr>
        <th>Nome</th>
        <th>Descrição</th>
        <th>Preço</th>
        <th>Quantidade</th>
        <th>Ações</th>
      </tr>
    </thead>
    <tbody></tbody>
  </table>

  <script>
    const form = document.getElementById('productForm');
    const table = document.getElementById('productTable').querySelector('tbody');
    let products = JSON.parse(localStorage.getItem('products')) || [];
    let editIndex = -1;

    function renderTable() {
      table.innerHTML = '';
      products.forEach((product, index) => {
        const row = table.insertRow();
        row.innerHTML = `
          <td>${product.name}</td>
          <td>${product.description}</td>
          <td>R$ ${product.price.toFixed(2)}</td>
          <td>${product.quantity}</td>
          <td>
            <button onclick="editProduct(${index})">Editar</button>
            <button onclick="deleteProduct(${index})">Excluir</button>
          </td>
        `;
      });
    }

    function saveProducts() {
      localStorage.setItem('products', JSON.stringify(products));
    }

    function editProduct(index) {
      const product = products[index];
      document.getElementById('name').value = product.name;
      document.getElementById('description').value = product.description;
      document.getElementById('price').value = product.price;
      document.getElementById('quantity').value = product.quantity;
      editIndex = index;
    }

    function deleteProduct(index) {
      if (confirm('Tem certeza que deseja excluir este produto?')) {
        products.splice(index, 1);
        saveProducts();
        renderTable();
      }
    }

    form.addEventListener('submit', function (e) {
      e.preventDefault();
      const product = {
        name: document.getElementById('name').value,
        description: document.getElementById('description').value,
        price: parseFloat(document.getElementById('price').value),
        quantity: parseInt(document.getElementById('quantity').value),
      };

      if (editIndex >= 0) {
        products[editIndex] = product;
        editIndex = -1;
      } else {
        products.push(product);
      }

      saveProducts();
      renderTable();
      form.reset();
    });

    renderTable();
  </script>
</body>
</html>
