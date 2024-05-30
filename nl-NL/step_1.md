De `gradient1` en `gradient2` styles bieden verschillende verloopeffecten.

![Het vierkant aan de linkerkant toont kleuren die vervagen van linksboven naar rechtsonder en het vierkant aan de rechterkant toont kleuren die vervagen van linksonder naar rechtsboven.](images/gradient.PNG)

--- code ---
---
language: html
filename: index.html
line_numbers: false
---

<div class="gradient1">
    <p>Add text here</p>
</div>
<div class="gradient2">
    <p>Add text here</p>
</div>
--- /code ---

**Tip:** Om de kleuren en richting van het verloop te veranderen, pas de `background-image`-waarden aan voor de `gradient1` en `gradient2` classes in `style.css`.

--- code ---
---
language: CSS
filename: style.css
line_numbers: false
---

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
--- /code ---
