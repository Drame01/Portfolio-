# Portfolio-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Accueil</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#projects">Projets</a></li>
                <li><a href="#about">À propos</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h1>Bienvenue sur notre Portfolio</h1>
        <p>Découvrez nos services et projets</p>
    </section>

    <section id="services">
        <h2>Services</h2>
        <div class="service">
            <h3>Création de Miniature</h3>
            <p>Miniatures attrayantes et optimisées pour attirer les clics.</p>
        </div>
        <div class="service">
            <h3>Création de Serveur Discord</h3>
            <p>Serveurs Discord configurés sur mesure pour votre communauté.</p>
        </div>
        <div class="service">
            <h3>Écriture de Scripts</h3>
            <p>Scripts personnalisés pour vidéos YouTube, podcasts ou présentations.</p>
        </div>
        <div class="service">
            <h3>Développement de Site Web</h3>
            <p>Sites web modernes et responsives optimisés pour SEO.</p>
        </div>
        <div class="service">
            <h3>Montage Vidéo</h3>
            <p>Montage dynamique et engageant pour vos vidéos.</p>
        </div>
    </section>

    <section id="projects">
        <h2>Projets</h2>
        <div class="project">
            <h3>Projet 1</h3>
            <p>Description du projet 1.</p>
        </div>
        <div class="project">
            <h3>Projet 2</h3>
            <p>Description du projet 2.</p>
        </div>
        <div class="project">
            <h3>Projet 3</h3>
            <p>Description du projet 3.</p>
        </div>
    </section>

    <section id="about">
        <h2>À propos de moi</h2>
        <p>Texte à propos de vous et de votre expérience.</p>
    </section>

    <section id="contact">
        <h2>Contact</h2>
        <form id="contact-form">
            <label for="name">Nom:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            
            <button type="submit">Envoyer</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Mon Portfolio. Tous droits réservés.</p>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background: #333;
    color: #fff;
    padding: 10px 0;
}

nav ul {
    list-style: none;
    padding: 0;
    text-align: center;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

section {
    padding: 20px;
    text-align: center;
}

#home {
    background: #f4f4f4;
    padding: 60px 20px;
}

#services, #projects, #about, #contact {
    padding: 40px 20px;
}

.service, .project {
    margin: 20px 0;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

form label, form input, form textarea {
    margin: 10px 0;
}

form button {
    padding: 10px 20px;
    background: #333;
    color: #fff;
    border: none;
    cursor: pointer;
}
document.getElementById('contact-form').addEventListener('submit', function(e) {
    e.preventDefault();
    
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;
    
    alert(`Merci ${name}, nous avons bien reçu votre message !`);
    
    // Vous pouvez ajouter du code ici pour envoyer le formulaire via AJAX ou une autre méthode
});
