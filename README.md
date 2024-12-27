<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Encontre as mais elegantes joias de prata pura. Perfeitas para mulheres sofisticadas que valorizam a beleza e a qualidade.">
    <meta name="keywords" content="joias de prata, prata pura, acessórios femininos, elegância, joias premium">
    <meta name="author" content="Sua Empresa">
    <title>Joias de Prata Pura - Elegância e Sofisticação</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            background-color: #f9f9f9;
        }
        header {
            background: linear-gradient(90deg, #bbb, #ddd);
            padding: 20px;
            text-align: center;
        }
        header h1 {
            color: #444;
        }
        .cta {
            text-align: center;
            margin: 20px;
        }
        .cta button {
            background: #bbb;
            color: #fff;
            border: none;
            padding: 15px 25px;
            font-size: 18px;
            cursor: pointer;
            border-radius: 5px;
        }
        .cta button:hover {
            background: #888;
        }
        .carousel-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin: 20px auto;
            overflow: hidden;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .carousel {
            display: flex;
            transition: transform 0.5s ease-in-out;
        }
        .carousel img {
            min-width: 100%;
            user-select: none;
        }
        .carousel-buttons {
            position: absolute;
            top: 50%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            transform: translateY(-50%);
        }
        .carousel-buttons button {
            background-color: rgba(0, 0, 0, 0.5);
            border: none;
            color: white;
            padding: 10px;
            cursor: pointer;
            border-radius: 50%;
        }
        footer {
            background: #222;
            color: #fff;
            text-align: center;
            padding: 10px 0;
        }
        #whatsapp-button {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: #25D366;
            color: #fff;
            font-size: 18px;
            padding: 15px;
            border-radius: 50%;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        #whatsapp-button img {
            width: 24px;
            height: 24px;
        }
        #chatbot {
            position: fixed;
            bottom: 80px;
            right: 20px;
            background: #f9f9f9;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            font-size: 14px;
        }
        .banner {
            background: #d4af37;
            color: #fff;
            text-align: center;
            padding: 10px;
            font-size: 20px;
            font-weight: bold;
        }
        @media (max-width: 768px) {
            .cta button {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Descubra a Elegância das Joias de Prata Pura</h1>
</header>

<div class="banner">
    Aproveite 15% de desconto em sua primeira compra!
</div>

<section class="cta">
    <h2>Compre agora e realce sua beleza com sofisticação</h2>
    <button>Saiba Mais</button>
</section>

<div class="carousel-container">
    <div class="carousel">
        <img src="/mnt/data/A_collection_of_five_images_showcasing_elegant_sil.png" alt="Joia de prata 1">
        <img src="/mnt/data/A_collection_of_five_images_showcasing_elegant_sil.png" alt="Joia de prata 2">
        <img src="/mnt/data/A_collection_of_five_images_showcasing_elegant_sil.png" alt="Joia de prata 3">
        <img src="/mnt/data/A_collection_of_five_images_showcasing_elegant_sil.png" alt="Joia de prata 4">
        <img src="/mnt/data/A_collection_of_five_images_showcasing_elegant_sil.png" alt="Joia de prata 5">
    </div>
    <div class="carousel-buttons">
        <button id="prev">&#10094;</button>
        <button id="next">&#10095;</button>
    </div>
</div>

<div id="whatsapp-button" onclick="window.location.href='https://wa.me/553284429071';">
    <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
</div>

<div id="chatbot">
    Olá! Seja bem-vinda! Como posso ajudá-la hoje?
</div>

<footer>
    <p>&copy; 2024 Joias de Prata. Todos os direitos reservados.</p>
</footer>

<script>
    const carousel = document.querySelector('.carousel');
    const images = document.querySelectorAll('.carousel img');
    const prevButton = document.getElementById('prev');
    const nextButton = document.getElementById('next');
    let index = 0;

    function showSlide(newIndex) {
        if (newIndex < 0) {
            index = images.length - 1;
        } else if (newIndex >= images.length) {
            index = 0;
        } else {
            index = newIndex;
        }
        carousel.style.transform = `translateX(-${index * 100}%)`;
    }

    prevButton.addEventListener('click', () => showSlide(index - 1));
    nextButton.addEventListener('click', () => showSlide(index + 1));
</script>

</body>
</html>
