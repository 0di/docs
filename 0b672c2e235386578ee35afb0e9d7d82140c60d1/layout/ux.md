# UX Mods
Tablice zawierające kolory i rozmiary używane do generowania modyfikatorów.

## Colors

Dostępne kolory są w `_variables.scss`, nazwy zawierają prefix `color-`
Nie dajemy możliwości zmiany koloru konkretnego/pojedyńczego przycisku, wymagałoby to zmiany klasy przypisanej do elementu w html a unikamy takich edycji.
Zmieniamy tylko kolory dla danych klas które wpłyną na wszystkie wystąpienia na stronie.

#### Domyślna dostępna lista kolorów to:

```scss
$color-primary
$color-secondary
$color-tertiary
$color-quaternary

$color-extras
$color-action
$color-error

$color-white
$color-lightest-gray
$color-lighter-gray
$color-light-gray
$color-gray
$color-dark-gray
$color-darker-gray
$color-black
```

> Wartości te edytujemy tylko w pliku _variables.scss indywidualnym dla dilera.

Każdy z kolorów jest użyty w tablicy `$ux-colors` wykorzystywanej do generowania modyfikatorów kolorystycznych dla różnych elementów strony (button, tooltip, text) gdzie parowany jest z odpowiednim kolorem treści oraz informacją o sposobie zmiany koloru np przy :hover na buttonach (darken/lighten).

```scss
$ux-colors: (
    'primary': (
        base: $color-primary,
        text: #FFFFFF,
        states: darken
    ),
    'secondary': (
        base: $color-secondary,
        text: #FFFFFF,
        states: darken
    )
    ...
)
```

Na podstawie wpisu `primary` w tablicy `$ux-colors` wygenerowane zostaną m.in:
- Button `.btn--primary` wraz z :hover, :focus, :active oraz jego wersja `.btn--outline`
- Text color `.text--primary`
- Tooltip `.tooltip--primary` (NgBootstrap) oraz `[data-balloon-primary]` (Pure CSS Balloon)
- Badge `.badge--primary`

---
##### **Więcej informacji:**
1. [Button colors](/layout/buttons#colors)
2. [Font colors](/layout/fonts#colors)
3. [Tooltip colors](/layout/tooltip#colors)



## Sizes

Dostępne rozmiary są w `_variables.scss`, w tablicy `$sizes`
Używane są przy generowaniu modyfikatorów dla elementów formularzy i buttonów. **Nie mają związku z siatką strony (gridem)**.

#### Domyślna dostępna lista rozmiarów to:

```scss
$sizes: (
    'xxs': (
        font: 0.5rem,
        dimension: 1.25rem
    ),
    'xs': (
        font: 0.6rem,
        dimension: 1.5rem
    ),
    'sm': (
        font: 0.7rem,
        dimension: 1.75rem
    ),
    'neutral': (
        font: 0.8rem,
        dimension: 2rem
    ),
    'md': (
        font: 0.9rem,
        dimension: 2.25rem
    ),
    'lg': (
        font: 1rem,
        dimension: 2.5rem
    ),
    'xl': (
        font: 1.1rem,
        dimension: 2.75rem
    ),
    'main-size': (
        font: $main-font-size,
        dimension: 2.5 * $main-font-size
    )
);
```

Wartość w `dimension` używana jest jako wysokość (i szerokość w przypadku kwadratowych elementów). `Font` to po prostu rozmiar fonta.

Na podstawie wpisu `xs` w tablicy `$sizes` wygenerowane zostaną m.in:
- Button `.btn--xs` - wysokość 1.5rem, font 0.6rem
- Input/select/textarea `.form-control--xs` - wysokość 1.5rem, font 0.6rem
- Form confirmation `.confirmation--xs` - font o rozmiarze 0.6rem, - ikona 1.5 (wartość z dimension) razy 1.4em (wartość stała).
- Input group text `.input-group-text--xs` - font 0.6rem
- Checkbox `.form-checkbox--xs` - wysokość 1.5rem, szerokość 1.5rem, font 0.6rem
- Radio `.form-radio--xs` - wysokość 1.5rem, szerokość 1.5rem, font 0.6rem
- Tytuły tabów `.labeled-tabs--xs` - font 0.6rem
- Badge `.badge--xs` - font 0.6rem

Wpis `neutral` używany jest do klas głównych (bez modyfikatorów) np. `.btn` , `.form-control`. Ale automatycznie generowany jest też np. `.btn--neutral` i `.form-control--neutral` mający te same wartości.

---
##### **Więcej informacji:**
1. [Button sizes](/layout/buttons#sizes)
2. [Form sizes](/layout/form#sizes)