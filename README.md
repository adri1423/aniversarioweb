<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz Aniversario</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffebee;
            color: #d81b60;
            padding: 50px;
        }
        .mensaje {
            font-size: 24px;
            font-weight: bold;
            margin-top: 20px;
        }
        .corazon {
            font-size: 50px;
        }
    </style>
</head>
<body>
    <h1>💖 ¡Feliz Aniversario, mi amor! 💖</h1>
    <p id="mensaje" class="mensaje"></p>
    <p class="corazon">❤️❤️❤️</p>

    <script>
        function mostrarMensaje() {
            let fechaHoy = new Date();
            let dia = fechaHoy.getDate();
            let mes = fechaHoy.getMonth() + 1; // Enero es 0, sumamos 1
            let añoActual = fechaHoy.getFullYear();
            let añoInicio = 2023; // Año en que comenzó la relación
            let añosJuntos = añoActual - añoInicio;

            if (dia === 14 && mes === 2) {
                document.getElementById("mensaje").innerHTML = 
                    `Hoy cumplimos ${añosJuntos} años juntos. 💕🥂<br>
                    Gracias por todos estos momentos inolvidables.`;
            } else {
                document.getElementById("mensaje").innerHTML = 
                    "Aún no es nuestro aniversario, pero cada día te amo más. 💖";
            }
        }

        mostrarMensaje();
    </script>
</body>
</html>
