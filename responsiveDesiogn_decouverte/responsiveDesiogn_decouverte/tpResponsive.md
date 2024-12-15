# TP : Création d'un CV Responsive - M. John LODOESREM

## Objectif du TP
Transformer un CV statique en une page web responsive, en appliquant les principes du design adaptatif.

## Étape 1 : Préparation du Contenu
### Contenu du CV de M. John LODOESREM

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>CV - John LODOESREM</title>
</head>
<body>
    <header>
        <h1>John LODOESREM</h1>
        <p>Développeur Web Full Stack</p>
        <contact>
            <p>📞 +33 6 12 34 56 78</p>
            <p>✉️ john.lodoesrem@email.com</p>
            <p>📍 Paris, France</p>
        </contact>
    </header>

    <section id="profil">
        <h2>Profil Professionnel</h2>
        <p>Développeur passionné avec 7 ans d'expérience dans le développement web, spécialisé dans les technologies front-end et back-end.</p>
    </section>

    <section id="competences">
        <h2>Compétences</h2>
        <ul>
            <li>HTML5 & CSS3</li>
            <li>JavaScript (ES6+)</li>
            <li>React.js</li>
            <li>Node.js</li>
            <li>Python</li>
            <li>Base de données SQL</li>
        </ul>
    </section>

    <section id="experience">
        <h2>Expérience Professionnelle</h2>
        <article>
            <h3>Développeur Senior - TechInnovate</h3>
            <p>2020 - Présent</p>
            <ul>
                <li>Développement d'applications web full stack</li>
                <li>Conception d'interfaces utilisateur responsive</li>
            </ul>
        </article>
        <article>
            <h3>Développeur Web - WebSolutions</h3>
            <p>2017 - 2020</p>
            <ul>
                <li>Maintenance et optimisation de sites web</li>
                <li>Intégration de design responsive</li>
            </ul>
        </article>
    </section>

    <section id="formation">
        <h2>Formation</h2>
        <p>Master en Développement Web - École Supérieure d'Informatique, Paris</p>
    </section>

    <footer>
        <p>Permis de conduire B | Langues : Français (Langue maternelle), Anglais (Courant)</p>
    </footer>
</body>
</html>
```

## Étape 2 : Création de la Structure CSS Responsive

### Instructions pour le fichier `styles.css`

1. Appliquer un reset CSS
2. Utiliser le modèle de boîte border-box
3. Créer une mise en page responsive
4. Gérer la typographie de manière adaptative

```css
/* Reset et box-sizing */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    font-size: calc(14px + 0.5vw);
}

/* Header responsive */
header {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    margin-bottom: 30px;
}

header h1 {
    font-size: 2.5em;
}

/* Sections */
section {
    margin-bottom: 20px;
    padding: 15px;
    background-color: #f4f4f4;
    border-radius: 5px;
}

section h2 {
    border-bottom: 2px solid #333;
    padding-bottom: 10px;
    margin-bottom: 15px;
}

/* Liste de compétences */
#competences ul {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
}

#competences li {
    background-color: #007bff;
    color: white;
    padding: 5px 10px;
    border-radius: 3px;
}

/* Expériences */
#experience article {
    margin-bottom: 15px;
    padding: 10px;
    background-color: white;
    border-radius: 5px;
}

/* Media Queries */
@media screen and (max-width: 600px) {
    body {
        padding: 10px;
    }

    header h1 {
        font-size: 1.8em;
    }

    #competences ul {
        flex-direction: column;
    }

    #competences li {
        text-align: center;
    }
}
```

## Étape 3 : Ajouter la Balise Viewport

Dans la section `<head>` de votre HTML, ajoutez :
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## Étape 4 : Travaux Pratiques

### Exercices

1. Adaptez le design pour qu'il soit lisible sur mobile
2. Améliorez la section des compétences
3. Ajoutez des effets hover sur les sections
4. Optimisez les images (si vous ajoutez une photo de profil)

### Critères d'Évaluation

- Lisibilité sur mobile
- Performance
- Design cohérent
- Utilisation correcte des media queries
- Compatibilité multi-navigateurs

## Bonus

- Ajoutez un mode sombre
- Créez une version PDF téléchargeable
- Intégrez des animations CSS subtiles

## Ressources Complémentaires

- MDN Web Docs
- CSS-Tricks
- Google Web Fundamentals

## Rendu

Déposez votre projet sur Github :

Bon travail.