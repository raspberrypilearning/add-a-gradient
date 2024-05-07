The `gradient1` and `gradient2` styles provide different gradient effects.

![A screenshot showing the two gradient styles. The first shows colours fading from top left to bottom right and the second shows colours fading from bottom left to top right.](images/gradient.PNG)

## --- code ---

language: html
filename: index.html
line_numbers: false
--------------------------------------------------------

<div class="gradient1">
    <p>Add text here</p>
</div>
<div class="gradient2">
    <p>Add text here</p>
</div>

--- /code ---

**Tip:** To change the colours and direction of the gradient, adjust the `background-image` values for the `gradient1` and `gradient2` class in 'style.css'.

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
