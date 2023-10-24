# Buttons

Przyciski z uwagi na a11y i chęć ociągnięcia :focusa klawiaturą ale bez :focusa przy kliknięciu myszą mają budowę:

```html
<button class="btn" type="button">
    <span class="btn__wrapper" tabindex="-1">
        <span>Text</span>
    </span>
</button>
```

Przyciskiem może być `<button>` lub `<a>`.
Wewnątrz `.btn__wrapper` text może być w `<span>`, `<strong>` lub `<small>`.
Na równi z textem może znajdować się ikona w `<i>`, w kolejności zarówno przed jak i za tekstem. Przykładowo:

```html
<a href="" class="btn">
    <span class="btn__wrapper" tabindex="-1">
        <strong>Text</strong>
        <i class="w-icon-chevron-right"></i>
    </span>
</a>
```


> Wszystkie modyfikatory (w tym rozmiary i kolory przypisywane są do elementu `.btn`).





## Modificators

`.btn--wide`
: nadaje minimalną szerokość buttona + większe paddingi
<div nabthat>
    <button class="btn btn--primary btn--wide" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>Text</span>
        </span>
    </button>
</div>


`.btn--full`
: button ma 100% szerokości + brak paddingów
<div nabthat>
    <button class="btn btn--primary btn--full" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>Text</span>
        </span>
    </button>
</div>

`.btn--icon`
: ustala szerokość buttona równą wysokości (kwadratowy), bez paddingów, wewnątrz `.btn__wrapper` powinnna się wtedy znaleźć tylko ikona bez treści
<div nabthat>
    <button class="btn btn--primary btn--icon" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <i class="w-icon-check"></i>
        </span>
    </button>
</div>

`.disabled` , `[disabled]`
: ustala kursor jak na element nieklikalny i wyłącza stylizowanie :hover, :active
<div nabthat>
    <button class="btn btn--primary" type="button" disabled>
        <span class="btn__wrapper" tabindex="-1">
            <span>Text</span>
            <i class="w-icon-check"></i>
        </span>
    </button>
</div>


`.blocked`
: ustala kursor jak na element nieklikalny, nakłada 50% szary filtr, 20% przeźroczystość i wyłącza stylizowanie :hover, :active
<div nabthat>
    <button class="btn btn--primary blocked" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>Text</span>
            <i class="w-icon-check"></i>
        </span>
    </button>
</div>


`[data-loading="true"]`
: dodaje po prawej stronie buttona animowany gif sugerujący ładowanie
<div nabthat>
    <button class="btn btn--primary btn--wide" type="button" data-loading="true">
        <span class="btn__wrapper" tabindex="-1">
            <span>Text</span>
        </span>
    </button>
</div>

`.btn--rows`
: elementy buttona będą 'wierszowo' zamiast obok siebie
<div nabthat>
    <button class="btn btn--primary btn--rows" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <strong>Text</strong>
            <small>Text</small>
        </span>
    </button>
    <button class="btn btn--primary btn--rows" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <i class="w-icon-check"></i>
            <small>Text</small>
        </span>
    </button>
</div>





## Sizes

Na podstawie elementów w tablicy $sizes domyślnie generowane są klasy:

`.btn--xxs` , `.btn--xs` , `.btn--sm` , `.btn--neutral` , `.btn--md` , `.btn--lg` , `.btn--xl` , `.btn--main-size`

Modyfikator `.btn--neutral` ma takie same wartości co sam `.btn`.

Modyfikator `.btn--main-size` ma font wielkości bazowego fonta strony i wysokość 2.5 raza większą od fonta. (domyślnie jest to rozmiar między --sm a --neutral).


<div nabthat>
<button class="btn btn--primary btn--xxs" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--xxs</span>
        </span>
    </button>
    <button class="btn btn--primary btn--xs" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--xs</span>
        </span>
    </button>
    <button class="btn btn--primary btn--sm" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--sm</span>
        </span>
    </button>
    <button class="btn btn--primary btn--main-size" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--main-size</span>
        </span>
    </button>
    <button class="btn btn--primary btn--neutral" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--neutral</span>
        </span>
    </button>
    <button class="btn btn--primary" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn</span>
        </span>
    </button>
    <button class="btn btn--primary btn--md" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--md</span>
        </span>
    </button>
    <button class="btn btn--primary btn--lg" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--lg</span>
        </span>
    </button>
    <button class="btn btn--primary btn--xl" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--xl</span>
        </span>
    </button>    
</div>

---
##### **Więcej informacji:**
1. [UX Mods - Sizes](/layout/ux#sizes)





## Colors

Na podstawie elementów w tablicy $ux-colors domyślnie generowane są klasy:

`.btn--primary` , `.btn--secondary` , `.btn--tertiary` , `.btn--quaternary` , `.btn--action` , `.btn--extras` , `.btn--error`
`.btn--white` , `.btn--lighter-gray` , `.btn--light-gray` , `.btn--gray` , `.btn--dark-gray` , `.btn--darker-gray` , `.btn--black`

<div nabthat>
    <button class="btn btn--primary" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--primary</span>
        </span>
    </button>
    <button class="btn btn--secondary" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--secondary</span>
        </span>
    </button>
    <button class="btn btn--tertiary" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--tertiary</span>
        </span>
    </button>
    <button class="btn btn--quaternary" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--quaternary</span>
        </span>
    </button>
    <button class="btn btn--action" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--action</span>
        </span>
    </button>
    <button class="btn btn--extras" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--extras</span>
        </span>
    </button>
    <button class="btn btn--error" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--error</span>
        </span>
    </button>
    <button class="btn btn--white" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--white</span>
        </span>
    </button>
    <button class="btn btn--lighter-gray" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--lighter-gray</span>
        </span>
    </button>
    <button class="btn btn--light-gray" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--light-gray</span>
        </span>
    </button>
    <button class="btn btn--gray" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--gray</span>
        </span>
    </button>
    <button class="btn btn--dark-gray" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--dark-gray</span>
        </span>
    </button>
    <button class="btn btn--darker-gray" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--darker-gray</span>
        </span>
    </button>
    <button class="btn btn--black" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--black</span>
        </span>
    </button>
</div>

Dodatkowo istnieje klasa `.btn--outline` która łączy się z powyższymi modyfikatorami kolorów. **Przy .btn--outline background jest przeźroczysty a nie biały**

<div nabthat>
    <button class="btn btn--primary btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--primary</span>
        </span>
    </button>
    <button class="btn btn--secondary btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--secondary</span>
        </span>
    </button>
    <button class="btn btn--tertiary btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--tertiary</span>
        </span>
    </button>
    <button class="btn btn--quaternary btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--quaternary</span>
        </span>
    </button>
    <button class="btn btn--action btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--action</span>
        </span>
    </button>
    <button class="btn btn--extras btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--extras</span>
        </span>
    </button>
    <button class="btn btn--error btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--error</span>
        </span>
    </button>
    <button class="btn btn--white btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--white</span>
        </span>
    </button>
    <button class="btn btn--lighter-gray btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--lighter-gray</span>
        </span>
    </button>
    <button class="btn btn--light-gray btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--light-gray</span>
        </span>
    </button>
    <button class="btn btn--gray btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--gray</span>
        </span>
    </button>
    <button class="btn btn--dark-gray btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--dark-gray</span>
        </span>
    </button>
    <button class="btn btn--darker-gray btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--darker-gray</span>
        </span>
    </button>
    <button class="btn btn--black btn--outline" type="button">
        <span class="btn__wrapper" tabindex="-1">
            <span>.btn--black</span>
        </span>
    </button>
</div>

---
##### **Więcej informacji:**
1. [UX Mods - Colors](/layout/ux#colors)





## Badge

Wykorzystywany w liście aktywnych filtrów na SPR. Może posiadać dowolny tag (`<button>` , `<a>` , `<span>`).
Jako content można użyć:

`<small>`
: treść z font-size 80%

`<span>`
: podstawowa treść

`<strong>`
: pogrubiona treść

`<i>`
: ikona

<div nabthat>
    <button class="badge badge--primary">
        <small>small</small>
        <span>span</span>
        <strong>strong</strong>
        <i class="w-icon-cross"></i>
    </button>
</div>

Dostępne sa wszystkie modyfikatory colors i sizes. Przykładowo `.badge--xs`, `.badge--main-size`, `.badge--action`, `.badge--outline`.

<div nabthat>
    <span class="badge badge--xxs">
        <span>badge--xxs</span>
    </span>
    <span class="badge badge--xs">
        <span>badge--xs</span>
    </span>
    <span class="badge badge--sm">
        <span>badge--sm</span>
    </span>
    <span class="badge badge--neutral">
        <span>badge--neutral</span>
    </span>
    <span class="badge badge--md">
        <span>badge--md</span>
    </span>
    <span class="badge badge--lg">
        <span>badge--lg</span>
    </span>
    <span class="badge badge--xl">
        <span>badge--xl</span>
    </span>
    <span class="badge badge--main-size">
        <span>badge--main-size</span>
    </span>
</div>
<div nabthat>
    <span class="badge badge--primary">
        <span>badge--primary</span>
    </span>
    <span class="badge badge--secondary">
        <span>badge--secondary</span>
    </span>
    <span class="badge badge--tertiary">
        <span>badge--tertiary</span>
    </span>
    <span class="badge badge--quaternary">
        <span>badge--quaternary</span>
    </span>
    <span class="badge badge--action">
        <span>badge--action</span>
    </span>
    <span class="badge badge--extras">
        <span>badge--extras</span>
    </span>
    <span class="badge badge--error">
        <span>badge--error</span>
    </span>
    <span class="badge badge--white">
        <span>badge--white</span>
    </span>
    <span class="badge badge--lighter-gray">
        <span>badge--lighter-gray</span>
    </span>
    <span class="badge badge--light-gray">
        <span>badge--light-gray</span>
    </span>
    <span class="badge badge--gray">
        <span>badge--gray</span>
    </span>
    <span class="badge badge--dark-gray">
        <span>badge--dark-gray</span>
    </span>
    <span class="badge badge--darker-gray">
        <span>badge--darker-gray</span>
    </span>
    <span class="badge badge--black">
        <span>badge--black</span>
    </span>
</div>




## Dropdown button

Bootstrapowy dropdown button ma lekko zmienioną budowę. Nie posiada wersji kolorystycznych, przyjmuje kolor --primary. 
Aktualnie używany jest tylko do wyboru sortowania na SRP.

```html
<div class="dropdown-btn" placement="bottom-right" ngbDropdown>
    <button class="btn dropdown-btn__toggle" id="_customID_" ngbDropdownToggle>
    <span class="btn__wrapper" tabindex="-1">
        <span>Text</span>
    </span>
    </button>
    <div class="dropdown-btn__menu" aria-labelledby="_customID_" ngbDropdownMenu>
        <button class="dropdown-btn__menu__item">Wpis</button>
        <button class="dropdown-btn__menu__item">Wpis</button>
    </div>
</div>
```

---
##### **Więcej informacji:**
1. [UX colors](/layout/colors)
