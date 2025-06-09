`gradient1` 和 `gradient2` 样式提供不同的渐变效果。

![右侧的方块显示颜色从左上角向右下角逐渐消失，左侧的方块显示颜色从左下角向右上角逐渐消失。](images/gradient.PNG)

## --- code ---

language: html
filename: index.html
line_numbers: false
--------------------------------------------------------

<div class="gradient1">
    <p>在此处添加文本</p>
</div>
<div class="gradient2">
    <p>在此处添加文本</p>
</div>

--- /code ---

**提示**：要更改渐变的颜色和方向，请调整 `style.css` 中 `gradient1` 和 `gradient2` 类的 `background-image` 值。

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
