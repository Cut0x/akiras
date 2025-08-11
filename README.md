# Akiras.xyz - Suite d'Outils Créatifs

Une collection d'outils web modernes pour créer des QR codes, des memes et des citations avec un design sombre élégant.

## 🚀 Fonctionnalités

### 📱 Générateur QR Code
- **Types supportés** : Texte, URL, Email, Téléphone, WiFi
- **Personnalisation** : Couleurs, tailles, niveaux de correction d'erreur
- **Export** : PNG et SVG haute qualité
- **Interface** : Tabs intuitives avec prévisualisation en temps réel

### 😂 Générateur de Memes
- **Templates prédéfinis** : Drake, Distracted Boyfriend, Woman & Cat, Thinking
- **Upload personnalisé** : Support de tous formats d'images
- **Éditeur avancé** : Texte avec contours, polices variées
- **Auto-format** : Texte automatiquement en majuscules (style meme)

### 💭 Générateur de Citations
- **Styles variés** : 5 dégradés + couleur unie personnalisable
- **Citations aléatoires** : Base de données de citations inspirantes
- **Formats multiples** : Carré, paysage, portrait, bannière sociale
- **Typographie** : Polices élégantes avec guillemets stylisés

## 🎨 Design & UX

- **Thème sombre moderne** avec palette de couleurs cohérente
- **100% responsive** optimisé mobile, tablette et desktop
- **Bootstrap Icons** pour une iconographie professionnelle
- **Animations fluides** avec transitions CSS avancées
- **Interface sticky** avec navigation contextuelle

## 🛠️ Technologies

- **Frontend** : HTML5, CSS3, JavaScript ES6+
- **Styling** : CSS Variables, Grid, Flexbox
- **Libraries** : QRious.js pour génération QR codes
- **Icons** : Bootstrap Icons 1.11.0
- **Deployment** : Vercel avec redirections optimisées

## 📁 Structure du Projet

```
akiras.xyz/
├── index.html              # Page d'accueil
├── vercel.json             # Configuration Vercel
├── pages/
│   ├── qrcode.html         # Générateur QR Code
│   ├── memes.html          # Générateur Memes
│   └── citations.html      # Générateur Citations
└── README.md              # Documentation
```

## 🌐 URLs

- **Accueil** : `akiras.xyz/`
- **QR Code** : `akiras.xyz/qrcode`
- **Memes** : `akiras.xyz/memes`
- **Citations** : `akiras.xyz/citations`

## 🚀 Déploiement Vercel

1. **Cloner le repo** et connecter à Vercel
2. **Configuration automatique** via `vercel.json`
3. **Domaine personnalisé** : Configurer `akiras.xyz`
4. **SSL/TLS** : Automatique avec Vercel

### Configuration Vercel.json

```json
{
  "rewrites": [
    { "source": "/qrcode", "destination": "/pages/qrcode.html" },
    { "source": "/memes", "destination": "/pages/memes.html" },
    { "source": "/citations", "destination": "/pages/citations.html" }
  ],
  "headers": [
    {
      "source": "/(.*)",
      "headers": [
        { "key": "X-Content-Type-Options", "value": "nosniff" },
        { "key": "X-Frame-Options", "value": "DENY" },
        { "key": "X-XSS-Protection", "value": "1; mode=block" }
      ]
    }
  ]
}
```

## 🎯 Fonctionnalités Avancées

### QR Code
- **Auto-génération** lors de la saisie
- **Validation** des formats (URL, email, téléphone)
- **Copie presse-papier** directement depuis l'interface
- **Templates WiFi** avec sécurité WPA/WEP

### Memes
- **Détection automatique** de la taille d'image
- **Wrap de texte** intelligent
- **Contours adaptatifs** selon la taille de police
- **Preview temps réel** avec canvas HTML5

### Citations
- **Base de données** de 12+ citations célèbres
- **Algorithme de wrap** optimisé pour lisibilité
- **Formats sociaux** (Facebook, Twitter, Instagram)
- **Gradients animés** avec CSS moderne

## 📱 Responsive Design

| Breakpoint | Layout | Navigation |
|------------|--------|------------|
| `> 1200px` | 2 colonnes | Navbar complète |
| `768-1200px` | 1 colonne | Navbar adaptée |
| `< 768px` | Stack mobile | Menu compact |

## 🔧 Personnalisation

### Variables CSS
```css
:root {
  --primary-bg: #0d1117;
  --secondary-bg: #161b22;
  --card-bg: #21262d;
  --accent-color: #58a6ff;
  --text-primary: #c9d1d9;
}
```

### Couleurs du Thème
- **Arrière-plans** : Dégradés de gris foncé
- **Accents** : Bleu GitHub (#58a6ff)
- **Texte** : Blanc cassé pour le confort visuel
- **Bordures** : Gris subtil pour la séparation

## 🌟 Points Forts

1. **Performance** : Chargement rapide, assets optimisés
2. **Accessibilité** : Contrastes WCAG, navigation clavier
3. **SEO** : Meta tags optimisés, structure sémantique
4. **Sécurité** : Headers CSP, validation côté client
5. **UX** : Feedback visuel, états de chargement

## 🔄 Mises à Jour

- **v1.0** : Lancement initial avec 3 outils
- **v1.1** : Optimisations mobile et nouvelles citations
- **v1.2** : Templates memes supplémentaires
- **v2.0** : Refonte design dark theme complet

## 📞 Support

Pour toute question ou suggestion :
- **GitHub Issues** : Rapporter bugs et demandes
- **Email** : contact@valloic.dev
- **Documentation** : Consulter ce README

---

*Créé avec ❤️ pour la communauté créative*
