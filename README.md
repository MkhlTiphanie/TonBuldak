<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TonBuldak - Commande et Personnalisation</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
            background-image: url('images/noodles-pattern.png'), url('images/koala-pattern.png');
            background-size: 100px 100px, 200px 200px;
            background-position: left top, right bottom;
            background-repeat: repeat, repeat;
        }
        header {
            background-color: #f8b7d3;
            color: white;
            padding: 1rem 2rem;
            text-align: center;
            font-size: 1.8rem;
        }
        nav {
            background-color: #ffe0b2;
            padding: 1rem;
            text-align: center;
        }
        nav a {
            margin: 0 1rem;
            text-decoration: none;
            color: #f8b7d3;
            font-weight: bold;
        }
        .container {
            padding: 2rem;
        }
        .hero {
            text-align: center;
            margin-bottom: 2rem;
        }
        .hero img {
            width: 100%;
            border-radius: 8px;
        }
        .products, .contact-form, .extras {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 2rem;
            margin-bottom: 3rem;
        }
        .product, .extra {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 300px;
            text-align: center;
            padding: 1rem;
        }
        .product img, .extra img {
            width: 100%;
            border-radius: 8px;
        }
        .product h3, .extra h3 {
            color: #f8b7d3;
            margin: 1rem 0;
        }
        .product button, .extra button {
            background-color: #f8b7d3;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            cursor: pointer;
        }
        .product button:hover, .extra button:hover {
            background-color: #f49dc0;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 0.8rem;
            margin: 0.5rem 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .contact-form button {
            background-color: #f8b7d3;
            color: white;
            border: none;
            padding: 0.8rem;
            border-radius: 5px;
            cursor: pointer;
        }
        .contact-form button:hover {
            background-color: #f49dc0;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #ffe0b2;
            margin-top: 2rem;
        }
    </style>
</head>
<body>

<!-- Header & Navigation -->
<header>
    TonBuldak - Commandez Maintenant
</header>

<nav>
    <a href="#accueil">Accueil</a>
    <a href="#commande">Commander</a>
    <a href="#desserts">Desserts & Boissons</a>
    <a href="#contact">Contact</a>
    <a href="#panier">Panier</a> <!-- Lien vers le panier -->
</nav>

<!-- Accueil Section -->
<section id="accueil" class="container">
    <div class="hero">
        <h2>Bienvenue chez TonBuldak</h2>
        <p>Découvrez nos délicieuses nouilles et personnalisez-les selon vos envies !</p>
    </div>
</section>

<!-- Commande Section -->
<section id="commande" class="container">
    <h2>Nos Bol de Nouilles</h2>
    <div class="products">
        <div class="product">
            <img src="images/spicy-bowl.jpg" alt="Bol épicé">
            <h3>Bol Épicé</h3>
            <p>Un mélange intense pour les amateurs de sensations fortes.</p>
            <p><strong>7,99 €</strong></p>
            <div class="supplements">
                <label><input type="checkbox" name="spicy-supplements" value="nems"> Nems (+1€)</label>
                <label><input type="checkbox" name="spicy-supplements" value="algues"> Algues (+1€)</label>
                <label><input type="checkbox" name="spicy-supplements" value="toboki"> Toboki (+1€)</label>
                <label><input type="checkbox" name="spicy-supplements" value="oeufs"> Oeufs (+1€)</label>
                <label><input type="checkbox" name="spicy-supplements" value="saucisses"> Saucisses (+1€)</label>
                <label><input type="checkbox" name="spicy-supplements" value="fromage"> Fromage (+1€)</label>
                <label><input type="checkbox" name="spicy-supplements" value="cacahuetes"> Cacahuètes (+1€)</label>
            </div>
            <button onclick="addToCart('Bol Épicé')">Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="images/sweet-spicy-bowl.jpg" alt="Bol sucré épicé">
            <h3>Bol Sucré-Épicé</h3>
            <p>L'équilibre parfait entre douceur et piquant.</p>
            <p><strong>8,99 €</strong></p>
            <div class="supplements">
                <label><input type="checkbox" name="sweet-supplements" value="nems"> Nems (+1€)</label>
                <label><input type="checkbox" name="sweet-supplements" value="algues"> Algues (+1€)</label>
                <label><input type="checkbox" name="sweet-supplements" value="toboki"> Toboki (+1€)</label>
                <label><input type="checkbox" name="sweet-supplements" value="oeufs"> Oeufs (+1€)</label>
                <label><input type="checkbox" name="sweet-supplements" value="saucisses"> Saucisses (+1€)</label>
                <label><input type="checkbox" name="sweet-supplements" value="fromage"> Fromage (+1€)</label>
                <label><input type="checkbox" name="sweet-supplements" value="cacahuetes"> Cacahuètes (+1€)</label>
            </div>
            <button onclick="addToCart('Bol Sucré-Épicé')">Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="images/vegan-bowl.jpg" alt="Bol Vegan">
            <h3>Bol Vegan</h3>
            <p>Des saveurs éthiques et délicieuses pour tous.</p>
            <p><strong>6,99 €</strong></p>
            <div class="supplements">
                <label><input type="checkbox" name="vegan-supplements" value="nems"> Nems (+1€)</label>
                <label><input type="checkbox" name="vegan-supplements" value="algues"> Algues (+1€)</label>
                <label><input type="checkbox" name="vegan-supplements" value="toboki"> Toboki (+1€)</label>
                <label><input type="checkbox" name="vegan-supplements" value="oeufs"> Oeufs (+1€)</label>
                <label><input type="checkbox" name="vegan-supplements" value="saucisses"> Saucisses (+1€)</label>
                <label><input type="checkbox" name="vegan-supplements" value="fromage"> Fromage (+1€)</label>
                <label><input type="checkbox" name="vegan-supplements" value="cacahuetes"> Cacahuètes (+1€)</label>
            </div>
            <button onclick="addToCart('Bol Vegan')">Ajouter au panier</button>
        </div>
    </div>
</section>

<!-- Desserts & Boissons Section -->
<section id="desserts" class="container">
    <h2>Desserts & Boissons</h2>
    <div class="extras">
        <div class="extra">
            <img src="images/boisson.jpg" alt="Boisson">
            <h3>Boisson</h3>
            <div>
                <label><input type="radio" name="boisson" value="coca"> Coca (+1,5€)</label><br>
                <label><input type="radio" name="boisson" value="ice-tea"> Ice Tea (+1,5€)</label><br>
                <label><input type="radio" name="boisson" value="fanta"> Fanta (+1,5€)</label><br>
                <label><input type="radio" name="boisson" value="seven-up"> Seven Up (+1,5€)</label><br>
                <label><input type="radio" name="boisson" value="jus"> Jus de fruits (+1,5€)</label><br>
                <label><input type="radio" name="boisson" value="eau"> Eau (+1€)</label>
            </div>
            <button onclick="addToCart('Boisson')">Ajouter au panier</button>
        </div>
        <div class="extra">
            <img src="images/boules-de-coco.jpg" alt="Boules de coco">
            <h3>Boules de Coco</h3>
            <p>Une douceur fondante à base de coco.</p>
            <button onclick="addToCart('Boules de Coco')">Ajouter au panier</button>
        </div>
        <div class="extra">
            <img src="images/mochis.jpg" alt="Mochis">
            <h3>Mochis Glacés</h3>
            <p>Des mochis glacés pour terminer en beauté.</p>
            <button onclick="addToCart('Mochis Glacés')">Ajouter au panier</button>
        </div>
    </div>
</section>

<!-- Panier Section -->
<section id="panier" class="container">
    <h2>Votre Panier</h2>
    <div id="panier-items">
        <p>Votre panier est vide.</p>
    </div>
    <p><strong>Total :</strong> <span id="total-panier">0 €</span></p>
    <button onclick="proceedToPayment()">Passer à la caisse</button>
</section>

<!-- Contact Form Section -->
<section id="contact" class="container">
    <h2>Contactez-nous</h2>
    <div class="contact-form">
        <input type="text" placeholder="Votre nom" required>
        <input type="email" placeholder="Votre email" required>
        <textarea placeholder="Votre message" rows="5" required></textarea>
        <button type="submit">Envoyer</button>
    </div>
</section>

<!-- Footer -->
<footer>
    <p>&copy; 2025 TonBuldak. Tous droits réservés.</p>
</footer>

<script>
    let panier = [];
    const prixItems = {
        'Bol Épicé': 7.99,
        'Bol Sucré-Épicé': 8.99,
        'Bol Vegan': 6.99,
        'Boisson': 1.5,
        'Boules de Coco': 2.5,
        'Mochis Glacés': 3.0
    };

    // Fonction pour ajouter un article au panier
    function addToCart(item) {
        panier.push(item);
        updateCart();
    }

    // Met à jour l'affichage du panier
    function updateCart() {
        let panierContainer = document.getElementById("panier-items");
        let total = 0;
        panierContainer.innerHTML = '';  // Réinitialise le contenu
        if (panier.length === 0) {
            panierContainer.innerHTML = '<p>Votre panier est vide.</p>';
        } else {
            panier.forEach((item, index) => {
                let itemElement = document.createElement('div');
                itemElement.innerHTML = `<p>${item} - ${prixItems[item]} €</p>`;
                panierContainer.appendChild(itemElement);
                total += prixItems[item];
            });
        }
        document.getElementById("total-panier").textContent = `${total.toFixed(2)} €`;
    }

    // Fonction de redirection vers la page de paiement
    function proceedToPayment() {
        if (panier.length === 0) {
            alert('Votre panier est vide.');
        } else {
            window.location.href = 'payment.html'; // Remplacer par la vraie page de paiement
        }
    }
</script>

</body>
</html>
