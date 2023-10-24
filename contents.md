# Contents

Poniżej hierarchia globalnych styli. Ich zawartość jest możliwa do użycia w każdym komponencie strony.
Piszemy w nich tylko główne/powtarzalne elementy. **Nie edytujemy ich na potrzeby poszczególnego dilera!**
Zmiany wprowadzamy tylko chcąc rozbudować funkcjonalność dostępną dla wszystkich dilerów.

    src/styles/shared/
    ├── extras/
    │   ├── balloon.scss       - pure css tooltip
    │   ├── base.scss          - główne style layoutu, grid
    │   ├── buttons.scss       - style buttonów
    │   ├── fonts.scss         - style podstawowych treści
    │   ├── forms.scss         - style formularzy
    │   ├── functions.scss     - funkcje używane w scss
    │   ├── icons.scss         - ikony dostępne na stronie
    │   ├── responsive.scss    - wartości i funkcje zapewniające responsywność strony
    │   └── ux.scss            - style dla sliderów, tooltipów, pagera
    ├── _extras.scss          - import plików z katalogu 'extras'
    └── _variables.scss       - zmienne pozwalające dostosować wygląd strony do dilera

> Każdy komponent ma swoje własne style które działają tylko w obszarze swojego komponentu.

## Edycja globalnych styli

Nadpisywanie globalnych styli powinno odbywać się wyłącznie z użyciem indywidualnego katalogu dilera.
Style indywidualne dilera ładują się po stylach globalnych, więc nadpisywane są tylko różnice (plik styli dilera nie zastępuje styli globalnych).

    dealer/src/styles/shared/
    ├── extras/
    │   └── ###.scss           - tu tworzymy plik który chcemy nadpisać
    ├── _extras.scss          - tu importujemy plik który został utworzony w katalogu extras
    └── _variables.scss       - tu nadpisujemy zmienne

#### WAŻNE!

Chcąc przykładowo dodać indywidualny kod css dla danego dilera (np. wystylizować jakiś zewnętrzny widget) należy w folderze extras z katalogu dilera utworzyć nowy plik (przykładowo custom.scss) i zaincludować go w _extras.scss