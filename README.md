# CSS variables - naming conventions

This project aims to identify commonalities of css-variable names in different frameworks and to derive recommendations.  
It would be great if third-party components could rely on the availability of the same variables.  


## What should be available?

## Colors
Best practice in my eyes:  
```css
  --hsl-h: 38.8;
  --hsl-s: 80%;
  --hsl-l: 38.4%;

  --color: hsl(var(--hsl-h), var(--hsl-s), var(--hsl-l));

  --color-light: hsl(var(--hsl-h), var(--hsl-s), calc(var(--hsl-l) + (100% - var(--hsl-l)) * .9 ) );
  --color-dark: hsl(var(--hsl-h), var(--hsl-s), calc(var(--hsl-l) * .7 ) );

  --color-bg: hsl(var(--hsl-h), var(--hsl-s), 99.5%);
  --color-text: hsl(var(--hsl-h), var(--hsl-s), calc(var(--hsl-l) * .4 ) );

  --hsl-h-2: 20;   
  --hsl-2-s-2: var(--hsl-s);
  --hsl-l-2: var(--hsl-l);
  --color-2: hsl(var(--hsl-h-2), var(--hsl-s-2), var(--hsl-l-2));
  ...   
  
```
Once lab is supported, we use `--lab-l` will be used  


**advantages:** at best, you just have to change the "hue"  
**disadvantage:** more code than if you define the colors directly  

also to be considered:  
`--color-1`;  instead of `--color` ?  
`--theme-color` would be like the Web App Manifest standard...  
`--theme-primary` often used, what can go wrong when just use `--color` ? (collisions?)   



## Fonts
--font  
--font-2  

## Layout

spacing between sections  
eg. `--space:3rem;` --space-2...?  

column- / table- / grid-gaps  
eg. `--gap:2rem;` `--col-gap:2rem;` `--row-gap:2rem;`  

(max) content-width  
eg. `--width:50rem`  


## Increment / Decrement
Many properties are often requested in different gradations.  
Examples:  
`--width-x`, `--space--x`, `--gray-x`   
Possibilities are:  
`--width-0` to `--width-10` (`--width` would then correspond to `--width-5`)  
`--width-0` to `--width-100` (`--width` would then correspond to `--width-50`)  
`--width-xxs` to `--width-xxl` (`--width` would then correspond to `--width-m`)  

Other recommendations?

## Frameworks

Pico.css  
https://github.com/picocss/pico/blob/master/css/pico.classless.css

MVP.css  
https://andybrewer.github.io/mvp/#variables

feathercss:  
https://github.com/elishaterada/feathercss/blob/master/dist/feather.css

basic.css  
https://github.com/vladocar/Basic.css/blob/master/css/basic.css

pollen:  
https://github.com/radioactivepesto/pollen/tree/master/src/lib

ionic framework:  
https://ionicframework.com/docs/theming/colors

suitcss:  
https://github.com/suitcss/suit/blob/master/packages/theme/lib/theme.css

chota:  
https://jenil.github.io/chota/

bulma:  
https://bulma.io/documentation/customize/variables/

bootstrap:  
https://github.com/twbs/bootstrap/blob/master/scss/_variables.scss

material-design:  
https://github.com/material-components/material-components-web/blob/91aa2d6a613565546a3c47c375ad929f79c910b4/docs/theming.md#step-4-changing-the-theme-with-css-custom-properties

microsoft fast:  
https://fast.design/docs/design/design-system

ant.design:  
https://ant.design/docs/react/customize-theme

zoo-web-components:  
https://github.com/zooplus/zoo-web-components

## Blog-posts
https://css-tricks.com/what-do-you-name-color-variables/
  
  
  
**take part**
