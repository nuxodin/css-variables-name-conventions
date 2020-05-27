# CSS variables naming conventions

This project aims to identify commonalities of css-variable names in different frameworks and to derive recommendations.

## what should be available as variable
- colors
- fonts
- spacing
- ???

### colors
Best practice in my eyes:  
--color-primary-h: 38.8;  
--color-primary: hsl(var(--color-primary-h), 80%, 50%);  
--color-primary-light: hsl(var(--color-primary-h), 80%, 85%);   
--color-primary-dark: hsl(var(--color-primary-h), 80%, 30%);  
--color-seconary-h: 20;   
...   
  
**advantages:** at best, you just have to change the "hue"  
**disadvantage:** more code than if you define the colors directly  

also to be considered:  
`--color-1`;  instead of `--color-primary`
--theme-color would be like the Web App Manifest standard...



### fonts
--font-primary
--font-secondary

### spacing
--gap


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




blog-posts:  
https://css-tricks.com/what-do-you-name-color-variables/


