# CSS variables - naming conventions

This project aims to identify commonalities of css-variable names in different frameworks and to derive recommendations.

## what should be available as variable

### Colors
Best practice in my eyes:  
```css
--color-primary-h: 38.8;  
--color-primary: hsl(var(--color-primary-h), 80%, 50%);  
--color-primary-light: hsl(var(--color-primary-h), 80%, 85%);   
--color-primary-dark: hsl(var(--color-primary-h), 80%, 30%);  
--color-seconary-h: 20;   
...   
```

**advantages:** at best, you just have to change the "hue"  
**disadvantage:** more code than if you define the colors directly  

also to be considered:  
`--color-1`;  instead of `--color-primary` pros: not just primary and secondary
--theme-color would be like the Web App Manifest standard...



### Fonts
--font-primary  
--font-secondary  

### Spacing
--gap


## Frameworks

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


