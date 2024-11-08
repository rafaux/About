
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Slider com Slick</title>

    <!-- CSS do Slick -->
    <link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css"/>
    <link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css"/>

    <!-- jQuery -->
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>

    <!-- JS do Slick -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.js"></script>
    
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .slider {
            width: 80%;
            margin: 50px auto;
        }
        .slick-slide img {
            width: 100%;
            border-radius: 10px;
        }
    </style>
</head>
<body>

    <h2 style="text-align: center;">Exemplo de Slider com Slick</h2>

    <div class="slider">
        <div><img src="https://via.placeholder.com/800x300?text=Imagem+1" alt="Imagem 1"></div>
        <div><img src="https://via.placeholder.com/800x300?text=Imagem+2" alt="Imagem 2"></div>
        <div><img src="https://via.placeholder.com/800x300?text=Imagem+3" alt="Imagem 3"></div>
        <div><img src="https://via.placeholder.com/800x300?text=Imagem+4" alt="Imagem 4"></div>
        <div><img src="https://via.placeholder.com/800x300?text=Imagem+5" alt="Imagem 5"></div>
    </div>

    <script>
        $(document).ready(function(){
            // Inicializa o slider Slick
            $('.slider').slick({
                autoplay: true, // Ativa o autoplay
                autoplaySpeed: 3000, // Intervalo entre as imagens (em milissegundos)
                arrows: true, // Exibe as setas de navegação
                dots: true, // Exibe os pontos de navegação
                infinite: true, // Permite rolar infinitamente
                speed: 500, // Duração da transição entre slides
                fade: false, // Faz a transição entre as imagens de forma deslizante (não de fade)
                cssEase: 'linear' // Tipo de transição
            });
        });
    </script>

</body>
</html>
