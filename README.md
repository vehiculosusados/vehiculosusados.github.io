# vehiculosusados.github.io
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Vende Tu Vehículo - Oferta Directa</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 15px;
            text-align: center;
        }
        h1 {
            margin: 0;
        }
        form {
            background-color: #fff;
            padding: 20px;
            max-width: 600px;
            margin: 20px auto;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        label {
            display: block;
            margin-top: 15px;
            font-weight: bold;
        }
        input, select {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #333;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #555;
        }
        footer {
            text-align: center;
            margin-top: 40px;
            color: #777;
        }
    </style>
</head>
<body>
    <header>
        <h1>Vende Tu Vehículo</h1>
        <p>Recibe una oferta rápida y segura</p>
    </header>
    <form id="carForm">
        <h2>Información del Vehículo</h2>
        <label for="name">Nombre completo:</label>
        <input type="text" id="name" name="name" required />

        <label for="email">Correo electrónico:</label>
        <input type="email" id="email" name="email" required />

        <label for="phone">Teléfono:</label>
        <input type="tel" id="phone" name="phone" required />

        <label for="brand">Marca del vehículo:</label>
        <input type="text" id="brand" name="brand" required />

        <label for="model">Modelo:</label>
        <input type="text" id="model" name="model" required />

        <label for="year">Año:</label>
        <input type="number" id="year" name="year" min="1900" max="2025" required />

        <label for="mileage">Kilometraje:</label>
        <input type="number" id="mileage" name="mileage" required />

        <label for="condition">Estado del vehículo:</label>
        <select id="condition" name="condition" required>
            <option value="">Seleccione</option>
            <option value="Excelente">Excelente</option>
            <option value="Bueno">Bueno</option>
            <option value="Regular">Regular</option>
            <option value="Malo">Malo</option>
        </select>

        <button type="submit">Enviar solicitud</button>
    </form>

    <footer>
        <p>&copy; 2025 Vende Tu Vehículo. Todos los derechos reservados.</p>
    </footer>

    <script>
        document.getElementById('carForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Gracias por enviar tu información. Nos pondremos en contacto contigo con una oferta.');
            // Aquí puedes agregar código para enviar los datos al servidor
            this.reset();
        });
    </script>
</body>
</html>
