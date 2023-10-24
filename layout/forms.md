# Forms

Ogólna budowa formularzy wykorzystuje bootstrapowy układ.


## Modificators

`.has-error` , `.has-error .form-control`
: oznacza inputa jako błędnie zwalidowanego
<div nabthat>
    <input class="form-control has-error" placeholder=".has-error">
</div>





## Sizes

Na podstawie elementów w tablicy $sizes domyślnie generowane są klasy:

`.form-control--xs` , `.form-control--sm` , `.form-control--neutral` , `.form-control--md` , `.form-control--lg` , `.form-control--xl` , `.form-control--main-size`

Modyfikator `.form-control--neutral` ma takie same wartości co sam `.form-control`.

Modyfikator `.form-control--main-size` ma font wielkości bazowego fonta strony i wysokość 2.5 raza większą od fonta. (domyślnie jest to rozmiar między --sm a --neutral).


<div nabthat>
    <input class="form-control form-control--xs" placeholder=".form-control--xs" style="margin-bottom: 5px">
    <input class="form-control form-control--sm" placeholder=".form-control--sm" style="margin-bottom: 5px">
    <input class="form-control form-control--main-size" placeholder=".form-control--main-size" style="margin-bottom: 5px">
    <input class="form-control form-control--neutral" placeholder=".form-control--neutral" style="margin-bottom: 5px">
    <input class="form-control" placeholder=".form-control" style="margin-bottom: 5px">
    <input class="form-control form-control--md" placeholder=".form-control--md" style="margin-bottom: 5px">
    <input class="form-control form-control--lg" placeholder=".form-control--lg" style="margin-bottom: 5px">
    <input class="form-control form-control--xl" placeholder=".form-control--xl">
</div>





## Colors

Na podstawie elementów w tablicy $form-colors domyślnie generowane są klasy:

`.form-control--primary` , `.form-control--secondary` , `.form-control--tertiary` , `.form-control--quaternary` , `.form-control--transparent-light` , `.form-control--transparent-dark` , `.form-control--white` , `.form-control--black`

<div nabthat>
    <input class="form-control form-control--primary" placeholder=".form-control--primary" style="margin-bottom: 5px">
    <input class="form-control form-control--secondary" placeholder=".form-control--secondary" style="margin-bottom: 5px">
    <input class="form-control form-control--tertiary" placeholder=".form-control--tertiary" style="margin-bottom: 5px">
    <input class="form-control form-control--quaternary" placeholder=".form-control--quaternary" style="margin-bottom: 5px">
    <input class="form-control form-control--transparent-light" placeholder=".form-control--transparent-light" style="margin-bottom: 5px">
    <input class="form-control form-control--transparent-dark" placeholder=".form-control--transparent-dark" style="margin-bottom: 5px">
    <input class="form-control form-control--white" placeholder=".form-control--white" style="margin-bottom: 5px">
    <input class="form-control form-control--black" placeholder=".form-control--black">
</div>





## Selects

Selecty automatycznie dostają wystylizowaną strzełkę w kolorze tekstu.

<div nabthat>
    <select class="form-control form-control--primary" style="margin-bottom: 5px"><option>.form-control--primary</option></select>
    <select class="form-control form-control--secondary" style="margin-bottom: 5px"><option>.form-control--secondary</option></select>
    <select class="form-control form-control--tertiary" style="margin-bottom: 5px"><option>.form-control--tertiary</option></select>
    <select class="form-control form-control--quaternary" style="margin-bottom: 5px"><option>.form-control--quaternary</option></select>
    <select class="form-control form-control--transparent-light" style="margin-bottom: 5px"><option>.form-control--transparent-light</option></select>
    <select class="form-control form-control--transparent-dark" style="margin-bottom: 5px"><option>.form-control--transparent-dark</option></select>
    <select class="form-control form-control--white" style="margin-bottom: 5px"><option>.form-control--white</option></select>
    <select class="form-control form-control--black"><option>.form-control--black</option></select>
</div>

Dostępne są też wszystkie rozmiary jak w inputach.

<div nabthat>
    <select class="form-control form-control--xs" style="margin-bottom: 5px"><option>.form-control--xs</option></select>
    <select class="form-control form-control--sm" style="margin-bottom: 5px"><option>.form-control--sm</option></select>
    <select class="form-control form-control--main-size" style="margin-bottom: 5px"><option>.form-control--main-size</option></select>
    <select class="form-control form-control--neutral" style="margin-bottom: 5px"><option>.form-control--neutral</option></select>
    <select class="form-control" style="margin-bottom: 5px"><option>.form-control</option></select>
    <select class="form-control form-control--md" style="margin-bottom: 5px"><option>.form-control--md</option></select>
    <select class="form-control form-control--lg" style="margin-bottom: 5px"><option>.form-control--lg</option></select>
    <select class="form-control form-control--xl"><option>.form-control--xl</option></select>
</div>





## Checkboxes

Składa się z 3 elementów zawartych w `<label>`'u o klasie `.form-checkbox`. `<input>`'a który jest niewidoczny, `<em>` będący wizualną reprezentacją checkboxa, oraz treścią w `<span>` lub `<strong>` (treść jest opcjonalna).

``` html
<label class="form-checkbox">
    <input type="checkbox">
    <em role="presentation"></em>
    <span>Text</span>
</label>
```

Dostępne sa wsystkie rozmiary:
<div nabthat>
    <label class="form-checkbox form-checkbox--xs" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--xs</span>
    </label>
    <label class="form-checkbox form-checkbox--sm" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--sm</span>
    </label>
    <label class="form-checkbox form-checkbox--main-size" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--main-size</span>
    </label>
    <label class="form-checkbox form-checkbox--neutral" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--neutral</span>
    </label>
    <label class="form-checkbox" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox</span>
    </label>
    <label class="form-checkbox form-checkbox--md" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--md</span>
    </label>
    <label class="form-checkbox form-checkbox--lg" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--lg</span>
    </label>
    <label class="form-checkbox form-checkbox--xl" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--xl</span>
    </label>
</div>

i kolory:
<div nabthat>
    <label class="form-checkbox form-checkbox--primary" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--primary</span>
    </label>
    <label class="form-checkbox form-checkbox--secondary" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--secondary</span>
    </label>
    <label class="form-checkbox form-checkbox--tertiary" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--tertiary</span>
    </label>
    <label class="form-checkbox form-checkbox--quaternary" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--quaternary</span>
    </label>
    <label class="form-checkbox form-checkbox--transparent-light" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--transparent-light</span>
    </label>
    <label class="form-checkbox form-checkbox--transparent-dark" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--transparent-dark</span>
    </label>
    <label class="form-checkbox form-checkbox--white" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--white</span>
    </label>
    <label class="form-checkbox form-checkbox--black" style="margin-bottom: 3px">
        <input type="checkbox">
        <em role="presentation"></em>
        <span>.form-checkbox--black</span>
    </label>
</div>





## Radios

Składa się z 3 elementów zawartych w `<label>`'u o klasie `.form-radio`. `<input>`'a który jest niewidoczny, `<em>` będący wizualną reprezentacją radio, oraz treścią w `<span>` lub `<strong>` (treść jest opcjonalna).

``` html
<label class="form-radio">
    <input type="radio">
    <em role="presentation"></em>
    <span>Text</span>
</label>
```

Dostępne sa wsystkie rozmiary:
<div nabthat>
    <label class="form-radio form-radio--xs" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--xs</span>
    </label>
    <label class="form-radio form-radio--sm" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--sm</span>
    </label>
    <label class="form-radio form-radio--main-size" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--main-size</span>
    </label>
    <label class="form-radio form-radio--neutral" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--neutral</span>
    </label>
    <label class="form-radio" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio</span>
    </label>
    <label class="form-radio form-radio--md" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--md</span>
    </label>
    <label class="form-radio form-radio--lg" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--lg</span>
    </label>
    <label class="form-radio form-radio--xl" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--xl</span>
    </label>
</div>

i kolory:
<div nabthat>
    <label class="form-radio form-radio--primary" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--primary</span>
    </label>
    <label class="form-radio form-radio--secondary" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--secondary</span>
    </label>
    <label class="form-radio form-radio--tertiary" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--tertiary</span>
    </label>
    <label class="form-radio form-radio--quaternary" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--quaternary</span>
    </label>
    <label class="form-radio form-radio--transparent-light" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--transparent-light</span>
    </label>
    <label class="form-radio form-radio--transparent-dark" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--transparent-dark</span>
    </label>
    <label class="form-radio form-radio--white" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--white</span>
    </label>
    <label class="form-radio form-radio--black" style="margin-bottom: 3px">
        <input type="radio">
        <em role="presentation"></em>
        <span>.form-radio--black</span>
    </label>
</div>





## Labeled Tabs

Element imitujący taby. W `<div class="labeled-tabs">` można użyć bootstrapowej klasy dla justify-content. Np. `justify-content-between` by wyjustować elementy.

```html
<div class="labeled-tabs">
    <label class="labeled-tab">
        <input type="radio" name="">
        <strong class="labeled-tab__text">Text</strong>
    </label>
    <label class="labeled-tab">
        <input type="radio" name="">
        <strong class="labeled-tab__text">Text</strong>
    </label>
    <label class="labeled-tab">
        <input type="radio" name="">
        <strong class="labeled-tab__text">Text</strong>
    </label>
    <label class="labeled-tab">
        <input type="radio" name="">
        <strong class="labeled-tab__text">Text</strong>
    </label>
</div>
```

<div nabthat>
    <div class="labeled-tabs">
        <label class="labeled-tab">
            <input type="radio" name="test" checked>
            <strong class="labeled-tab__text">Sales</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test">
            <strong class="labeled-tab__text">Finance</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test">
            <strong class="labeled-tab__text">Parts</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test">
            <strong class="labeled-tab__text">Service</strong>
        </label>
    </div>
</div>

Nie ma tu dostępnych innych wersji kolorystycznych. Istnieją wszystkie rozmiary np.:

<div nabthat>
    <div class="labeled-tabs labeled-tabs--xs">
        <label class="labeled-tab">
            <input type="radio" name="test2" checked>
            <strong class="labeled-tab__text">labeled-tabs--xs</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test2">
            <strong class="labeled-tab__text">labeled-tabs--xs</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test2">
            <strong class="labeled-tab__text">labeled-tabs--xs</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test2">
            <strong class="labeled-tab__text">labeled-tabs--xs</strong>
        </label>
    </div>
    <div class="labeled-tabs labeled-tabs--main-size">
        <label class="labeled-tab">
            <input type="radio" name="test3" checked>
            <strong class="labeled-tab__text">labeled-tabs--main-size</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test3">
            <strong class="labeled-tab__text">labeled-tabs--main-size</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test3">
            <strong class="labeled-tab__text">labeled-tabs--main-size</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test3">
            <strong class="labeled-tab__text">labeled-tabs--main-size</strong>
        </label>
    </div>
    <div class="labeled-tabs labeled-tabs--xl">
        <label class="labeled-tab">
            <input type="radio" name="test4" checked>
            <strong class="labeled-tab__text">labeled-tabs--xl</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test4">
            <strong class="labeled-tab__text">labeled-tabs--xl</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test4">
            <strong class="labeled-tab__text">labeled-tabs--xl</strong>
        </label>
        <label class="labeled-tab">
            <input type="radio" name="test4">
            <strong class="labeled-tab__text">labeled-tabs--xl</strong>
        </label>
    </div>
</div>





## Form confirmation

```html
<div class="confirmation">
    <div class="confirmation__wrapper">
        <i class="confirmation__icon w-icon-check"></i>
        <strong class="confirmation__title">Thank You</strong>
        <span class="confirmation__text">We will get back <br>to You shortly.</span>
    </div>
</div>
```

<div nabthat>
    <div class="form-sent" style="height: 140px">
        <div class="confirmation">
            <div class="confirmation__wrapper">
                <i class="confirmation__icon w-icon-check"></i>
                <strong class="confirmation__title">Thank You</strong>
                <span class="confirmation__text">We will get back <br>to You shortly.</span>
            </div>
        </div>
    </div>
</div>

Confirmation jest pozycjonowane absolutnie względem rodzica. Centruje się na jego wysokość. Dlatego należy zadbać by formularz nie był zbyt mały.
Domyślnie zawartość `.confirmation` jest niewidoczna. Ukazuje się gdy bezpośredni rodzic otrzyma klasę `.form-sent`.

Tagi `<span>` `<strong>` można używać zamiennie, klasy `__title` `__text` zapewniają tylko wielkość fonta, kursywę i uppercase. Nie wpływają na font-weight.

Nie istnieją inne wersje kolorystyczne. Kolor treści/ikony można osiągnąć używając klasy modyfikującej kolor treści np. `.text-primary`. Dostępne są wszystkie rozmiary np.:
<div nabthat>
    <div class="form-sent" style="height: 70px">
        <div class="confirmation confirmation--xs">
            <div class="confirmation__wrapper">
                <i class="confirmation__icon w-icon-check"></i>
                <strong class="confirmation__text">.confirmation--xs</strong>
            </div>
        </div>
    </div>
    <div class="form-sent" style="height: 100px">
        <div class="confirmation confirmation--main-size">
            <div class="confirmation__wrapper">
                <i class="confirmation__icon w-icon-check-square text-light-gray"></i>
                <span class="confirmation__text">.confirmation--main-size</span>
            </div>
        </div>
    </div>
    <div class="form-sent" style="height: 140px">
        <div class="confirmation confirmation--xl">
            <div class="confirmation__wrapper">
                <i class="confirmation__icon w-icon-check text-primary"></i>
                <strong class="confirmation__text">.confirmation--xl</strong>
            </div>
        </div>
    </div>
</div>


## Lead button (certificate form)

Poniżej uproszczona budowa formularza.

```html
<form class="form-certificate form-certificate--srp">

    <!-- CERTIFICATE FORM TITLE -->
    <p class="obx-f__title"><span style="font-size: 0.7em">UNLOCK OUR BEST PRICE™</span></p>

    <!-- CERTIFICATE FORM -->
    <div class="row row--extratiny form-group--extratiny">
        <div class="col-7">
            <div class="form-group">
                <input type="email" class="form-control" placeholder="email">
            </div>
        </div>
        <div class="col-5">
            <div class="form-group">
                <input type="text" class="form-control" placeholder="name">
            </div>
        </div>
        <div class="col-12">
            <div class="form-group">
                <div class="input-group">
                    <input type="text" class="form-control" placeholder="zip code">
                
                    <div class="input-group-append">
                        <button class="btn" type="submit">
                            <span class="btn__wrapper" tabindex="-1">
                                <span>Unlock</span>
                                <i class="w-icon-chevron-right"></i>
                            </span>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- CERTIFICATE FORM INFO -->
    <small class="obx-f__info">No obligation to Buy.</small>

    <!-- CERTIFICATE FORM CONFIRMATION -->
    <div class="confirmation confirmation--xs">
        <div class="confirmation__wrapper">
            <i class="confirmation__icon w-icon-check"></i>
            <span class="confirmation__text">We will contact You shortly.</span>
        </div>
    </div>

</form>
```

`<form>` oprócz klasy `.form-certificate` powinien otrzymać jeszcze jakąś klasę modyfikującą która go wystylizuje.
Domyślnie dostępne są klasy `.form-certificate--srp` i `.form-certificate--vdp`. 
Stworzone są na podstawie wpisów w tablicy `$certificate-widget` w _variables.scss.

Element `.obx-f__title` ma zmienne font-size w zależności od układu/szerokości okna by proporcjonalnie zapewnić skalowanie zawartej w nim treści.
Wewnątrz musi znaleźć się `<span>` z własnym font-size ale liczonym na podstawie rodzica (% lub em). Dostosowanym do długości treści.

Niżej zaczyna się `.row` z elementami formularza, klasy pomocnicze `.row--extratiny .form-group--extratiny` zapewniają bardziej kompaktowy układ ale oczywiście są dowolne. Reszta contentu formularza to bootstrapowa budowa. Widoczność elementów buttona (treść, ikona) zarządzalna jest we wpisach tablicy `$certificate-widget` w _variables.scss.
