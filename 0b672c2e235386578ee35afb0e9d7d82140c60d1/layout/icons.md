# Icons

Na potrzeby ikon wykorzystywane są @font-face lub w ostateczności pliki .svg
Wszystkie znajdują się w odpowiednich katalogach w `src\assets\fonts`

Dodawanie nowych ikon następuje w pliku `icons.scss` w większości przypadków zalecane jest dodawanie ich w głównym pliku a nie pliku konkretnego dilera aby zapewnić możliwość ich użycia dla wszystkich (chyba, że są one sprecyzowane dla konkretnego dilera).





## Web icons

Używa fontu `IconsWeb` dla `<i>` zawierającego klasę rozpoczynającą się frazą `w-icon-`.
Aktualnie użyta jest przerobiona w [IcoMoon](https://icomoon.io/app) (odchudzona z lepiej wycentrowanymi ikonami) paczka [Linearicons](http://cms.devoffice.com/repack/packs/linearicons/)





## Custom icons

W wyjątkowych przypadkach możliwe jest użycie odpowiednio przygotowanego obrazka `.svg` jako ikony (z możliwym użyciem font-size, color...)
Ikona musi zostać uprzednio dodana do css np. w `icons.scss` lub w pliku styli dla konkretnej podstrony, używając:

```scss
@include c-icon('nazwa');
```

Funkcja `c-icon` utworzy wtedy klasę `.c-icon-nazwa` z atrybutem `mask-image` zawierającym url do lokalizacji `assets/fonts/IconsSVG/nazwa.svg` gdzie musi się znajdować plik ikony.



## Features icons

Używa fontu `IconsFeatures` dla `<i>` zawierającego klasę rozpoczynającą się frazą `f-icon-`.
Font został przychotowany w [IcoMoon](https://icomoon.io/app)

<ul nabthat class="icons-list">
  <li><i class="f-icon-aaa-capable"></i><span>aaa-capable</span></li>
  <li><i class="f-icon-ac-dual"></i><span>ac-dual</span></li>
  <li><i class="f-icon-ac"></i><span>ac</span></li>
  <li><i class="f-icon-adaptive-cruise-control"></i><span>adaptive-cruise-control</span></li>
  <li><i class="f-icon-alloy-wheels"></i><span>alloy-wheels</span></li>
  <li><i class="f-icon-android"></i><span>android</span></li>
  <li><i class="f-icon-apple-carplay"></i><span>apple-carplay</span></li>
  <li><i class="f-icon-automatic-headlights"></i><span>automatic-headlights</span></li>
  <li><i class="f-icon-backup-camera"></i><span>backup-camera</span></li>
  <li><i class="f-icon-blind-spot"></i><span>blind-spot</span></li>
  <li><i class="f-icon-bluetooth"></i><span>bluetooth</span></li>
  <li><i class="f-icon-cloth"></i><span>cloth</span></li>
  <li><i class="f-icon-collision-braking"></i><span>collision-braking</span></li>
  <li><i class="f-icon-collision-warning"></i><span>collision-warning</span></li>
  <li><i class="f-icon-competition-package"></i><span>competition-package</span></li>
  <li><i class="f-icon-convenience-package"></i><span>convenience-package</span></li>
  <li><i class="f-icon-cooled-seat"></i><span>cooled-seat</span></li>
  <li><i class="f-icon-cross-traffic-alert"></i><span>cross-traffic-alert</span></li>
  <li><i class="f-icon-diesel-engine"></i><span>diesel-engine</span></li>
  <li><i class="f-icon-drive-assist-package"></i><span>drive-assist-package</span></li>
  <li><i class="f-icon-entertainment"></i><span>entertainment</span></li>
  <li><i class="f-icon-executive-package"></i><span>executive-package</span></li>
  <li><i class="f-icon-flip-camera"></i><span>flip-camera</span></li>
  <li><i class="f-icon-fog-lights"></i><span>fog-lights</span></li>
  <li><i class="f-icon-folding-mirrors"></i><span>folding-mirrors</span></li>
  <li><i class="f-icon-following-distance-indicator"></i><span>following-distance-indicator</span></li>
  <li><i class="f-icon-head-up"></i><span>head-up</span></li>
  <li><i class="f-icon-heated-seat"></i><span>heated-seat</span></li>
  <li><i class="f-icon-heated-wheel"></i><span>heated-wheel</span></li>
  <li><i class="f-icon-hill"></i><span>hill</span></li>
  <li><i class="f-icon-honda-sensing"></i><span>honda-sensing</span></li>
  <li><i class="f-icon-immobiliser"></i><span>immobiliser</span></li>
  <li><i class="f-icon-keyless-entry"></i><span>keyless-entry</span></li>
  <li><i class="f-icon-keyless"></i><span>keyless</span></li>
  <li><i class="f-icon-lane-assist-warning"></i><span>lane-assist-warning</span></li>
  <li><i class="f-icon-lane-assist"></i><span>lane-assist</span></li>
  <li><i class="f-icon-leather"></i><span>leather</span></li>
  <li><i class="f-icon-luxury-package"></i><span>luxury-package</span></li>
  <li><i class="f-icon-m-sport-edition"></i><span>m-sport-edition</span></li>
  <li><i class="f-icon-m-sport-package"></i><span>m-sport-package</span></li>
  <li><i class="f-icon-moonroof"></i><span>moonroof</span></li>
  <li><i class="f-icon-motion-sensor"></i><span>motion-sensor</span></li>
  <li><i class="f-icon-mykey"></i><span>mykey</span></li>
  <li><i class="f-icon-navigation"></i><span>navigation</span></li>
  <li><i class="f-icon-nissan-connect"></i><span>nissan-connect</span></li>
  <li><i class="f-icon-no-moonroof"></i><span>no-moonroof</span></li>
  <li><i class="f-icon-panoramic-moonroof"></i><span>panoramic-moonroof</span></li>
  <li><i class="f-icon-park-distance-control"></i><span>park-distance-control</span></li>
  <li><i class="f-icon-parking-sensors"></i><span>parking-sensors</span></li>
  <li><i class="f-icon-power-door-lock"></i><span>power-door-lock</span></li>
  <li><i class="f-icon-power-seat-dual"></i><span>power-seat-dual</span></li>
  <li><i class="f-icon-power-seat"></i><span>power-seat</span></li>
  <li><i class="f-icon-power-sliding-doors"></i><span>power-sliding-doors</span></li>
  <li><i class="f-icon-premium-package"></i><span>premium-package</span></li>
  <li><i class="f-icon-press-brake"></i><span>press-brake</span></li>
  <li><i class="f-icon-rain-sensor"></i><span>rain-sensor</span></li>
  <li><i class="f-icon-rear-park-assist"></i><span>rear-park-assist</span></li>
  <li><i class="f-icon-rear-spoiler"></i><span>rear-spoiler</span></li>
  <li><i class="f-icon-remote-boot-no-foot"></i><span>remote-boot-no-foot</span></li>
  <li><i class="f-icon-remote-boot"></i><span>remote-boot</span></li>
  <li><i class="f-icon-remote-engine-start"></i><span>remote-engine-start</span></li>
  <li><i class="f-icon-remote-garage"></i><span>remote-garage</span></li>
  <li><i class="f-icon-reverse-sensing-system"></i><span>reverse-sensing-system</span></li>
  <li><i class="f-icon-safety-lock"></i><span>safety-lock</span></li>
  <li><i class="f-icon-second-row-seat"></i><span>second-row-seat</span></li>
  <li><i class="f-icon-security-system"></i><span>security-system</span></li>
  <li><i class="f-icon-shadow-sport-edition"></i><span>shadow-sport-edition</span></li>
  <li><i class="f-icon-sideview-mirrors"></i><span>sideview-mirrors</span></li>
  <li><i class="f-icon-sirius"></i><span>sirius</span></li>
  <li><i class="f-icon-speakers"></i><span>speakers</span></li>
  <li><i class="f-icon-steering-wheel-controls"></i><span>steering-wheel-controls</span></li>
  <li><i class="f-icon-sync"></i><span>sync</span></li>
  <li><i class="f-icon-third-row-seat"></i><span>third-row-seat</span></li>
  <li><i class="f-icon-tire-pressure"></i><span>tire-pressure</span></li>
  <li><i class="f-icon-wifi"></i><span>wifi</span></li>
  <li><i class="f-icon-wireless-charging"></i><span>wireless-charging</span></li>
</ul>

<ul nabthat class="icons-list">
  <li><i class="f-icon-automatic-transmission"></i><span>automatic-transmission</span></li>
  <li><i class="f-icon-autoshift-transmission"></i><span>autoshift-transmission</span></li>
  <li><i class="f-icon-cvt-transmission"></i><span>cvt-transmission</span></li>
  <li><i class="f-icon-manual-transmission"></i><span>manual-transmission</span></li>
  <li><i class="f-icon-sportronic-transmission"></i><span>sportronic-transmission</span></li>
</ul>

<ul nabthat class="icons-list">
  <li><i class="f-icon-2wd"></i><span>2wd</span></li>
  <li><i class="f-icon-4wd"></i><span>4wd</span></li>
  <li><i class="f-icon-4x4"></i><span>4x4</span></li>
  <li><i class="f-icon-awd"></i><span>awd</span></li>
  <li><i class="f-icon-fwd"></i><span>fwd</span></li>
  <li><i class="f-icon-rwd"></i><span>rwd</span></li>
</ul>