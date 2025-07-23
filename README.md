# studying-01-iphone-14-vadymprokopchuk  
Free Tutorial Coding Iphone 14 Pro Website from @vadymprokopchuk  

## Deployments  
https://pereguda-anatoliy.github.io/studying-01-iphone-14-vadymprokopchuk/  

## Ресурсы  

[Youtube Video Link](https://www.youtube.com/watch?v=2dVPFVX3ZZ0)  
[Author's YouTube Сhannel](https://www.youtube.com/@vadymprokopchuk)  
[Author's Telegram Сhannel](https://t.me/from0to1com)  
[Макет](https://drive.google.com/file/d/1N3QB3YGJbuVkMw7l3Qg5NMJz9F53CA7s/view)  
[VSC](https://code.visualstudio.com/)  
[Figma](https://www.figma.com/downloads/)  
[Doka Directory](https://doka.guide/)  
[Normalize](https://necolas.github.io/normalize.css/)  
[Fonts](https://fonts.google.com/)  

## Notes  

### VSC  
Manage - Settigs - Commonly Used - Files: Auto Save - onFocusChange  
Автосейв при смене фокуса  

### Figma  
PressMouseWheel - произвольное перемещение макета  
Space + PressLeftMouseButton - произвольное перемещение макета  
ScrollMouseWheel - перемещение макета вверх-вниз  
Shift + ScrollMouseWheel - перемещение макета влево-вправо  
Ctrl + ScrollMouseWheel - масштабирование макета  

Shift + R - показать или скрыть Линейки  

### HTML and Emmet  
header.header + Tab --> `<header class="header"></header>`  
.container + Tab --> `<div class="container"></div>`  
телефон в ссылке: `<a href="tel:380504565656" class="phone">+38 050-456-56-56</a>`  

### CSS and Emmet  
w1200 + Tab --> `width: 1200px;`  
df + Tab --> `display: flex;`  
jcsb + Tab --> `justify-content: space-between;`  
aic + Tab --> `align-items: center;`  
p70-0-40 + Tab --> `padding: 70px 0 40px;`  
fz64 + Tab --> `font-size: 64px;`  
lh29px + Tab --> `line-height: 29px;` в сокращении указывать px!  


Directions of margins and padding  
Top Right Bottom Left: 25px 25px 25px 25px  
Top Right&Left Bottom: 25px 25px 25px  
Top&Botton Right&Left: 25px 25px
All: 25px  

Механика Flex в Header  
1. `Flex-grow` + `Flex-basis` создают "пружинный" эффект:  
Блоки меню и телефон занимают всю свободную ширину  
`flex-grow: 1;` Растягиваем на всё свободное место  
`flex-basis: 0;` Игнорируем начальную ширину  
Лого остается "зажатым" между ними по центру  
2. `Space-between` в `.nav` распределяет:  
Первый элемент (меню) прижимается влево  
Последний элемент (телефон) - вправо  
Центральный элемент (лого) автоматически центрируется  
3. `Display: flex` для `.menu`:  
Превращает список `<ul>` в горизонтальное меню
Пункты автоматически выстраиваются в ряд
4. схема:  
[ Меню (растягивается) ] [ Лого (фикс) ] [ Телефон (растягивается) ]  
```  
.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
```  
```  
.menu {
    display: flex;
    flex-grow: 1;
    flex-basis: 0;
}
```  
```  
.phone {
    flex-grow: 1;
    flex-basis: 0;
    text-align: right;
}
```  

### Questions  
Пройдет ли валидацию ссылка без href?  
`<a class="logo"></a>`  
Убрать атрибут href разрешается спецификацией. Такая ссылка будет вести себя как «заглушка» и не будет интерактивной: не появится контекстное меню по правому клику, не изменится вид курсора при наведении, не возникнет фокус при работе с клавиатуры.  
[Дока](https://doka.guide/html/a/)  

Не работает `ctrl + /` для комментирования  
Сочетания клавиш в VSC проверил  
HTML `<!-- любой текст -->`  
CSS `/* любой текст */`  
JS `/* любой текст */`  









