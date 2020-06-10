# CSS variables - naming conventions

This project aims to identify commonalities of css-variable names in different frameworks and to derive recommendations.  
It would be great if third-party components could rely on the availability of the same variables.  

## What should be available?

## Colors
Best practice in my eyes:  
```css
--color-h: 38.8;  
--color-s: 80%;  
--color: hsl(var(--color-primary-h), var(--color-primary-s), 50%);  
--color-light: hsl(var(--color-primary-h), var(--color-primary-s), 85%);   
--color-dark: hsl(var(--color-primary-h), var(--color-primary-s), 30%);  

--color-2-h: 20;   
...   
```

**advantages:** at best, you just have to change the "hue"  
**disadvantage:** more code than if you define the colors directly  

also to be considered:  
`--color-1`;  instead of `--color` ?  
`--theme-color` would be like the Web App Manifest standard...  
`--theme-primary` often used (what can go wrong when just use `--color` ?)  



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


## Frameworks

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



## Blog-posts
https://css-tricks.com/what-do-you-name-color-variables/
  
  
  
**take part**
