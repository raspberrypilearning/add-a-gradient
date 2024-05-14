Les styles `gradient1` et `gradient2` permettent d'obtenir des effets de dégradé différents.

![Le carré de droite présente des couleurs qui s'estompent du haut à gauche vers le bas à droite et le carré de gauche présente des couleurs qui s'estompent du bas à gauche vers le haut à droite.](images/gradient.PNG)

## --- code ---

language: html
filename: index.html
line_numbers: false
--------------------------------------------------------

<div class="gradient1">
    <p>Ajoute du texte ici</p>
</div>
<div class="gradient2">
    <p>Ajoute du texte ici</p>
</div>

--- /code ---

**Astuce :** pour modifier les couleurs et la direction du dégradé, ajuste les valeurs de `background-image` pour les classes `gradient1` et `gradient2` dans `style.css`.

## --- code ---

language: CSS
filename: style.css
line_numbers: false
--------------------------------------------------------

.gradient1 {
background-image: linear-gradient(
to bottom right,
var(--secondary),
var(--detail)
);
color: var(--onsecondary);
}

.gradient2 {
background-image: linear-gradient(
to top right,
var(--tertiary),
var(--detail2)
);
color: var(--ontertiary);
}
\--- /code ---
