# summery 
## Next.js
![image](https://cdn-media-1.freecodecamp.org/images/1*uIepZ6YWTubeVxD5n5kkyg.png)
### Next.js has built-in support for CSS and Sass.
## how Download Starter Code
###  This sets up a nextjs-blog directory such that it’s identical to the result of the previous lesson.
```
npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn-starter/tree/master/assets-metadata-css-starter"
```

## Next.js has built-in support for CSS and Sass which allows you to import .css and .scss files.Using popular CSS libraries like Tailwind CSS is also supported.In this lesson, we’ll talk about how to write and import CSS files in Next.js. We’ll also talk about Next.js’s built-in support for CSS Modules and Sass. Let’s dive in!



## Styling Tips

### Using Sass
#### Out of the box, Next.js allows you to import Sass using both the .scss and .sass extensions. You can use component-level Sass via CSS Modules and the .module.scss or .module.sass extension.Before you can use Next.js' built-in Sass support, be sure to install sass:
```
npm install sass
```

## Customizing PostCSS Config
### Out of the box, with no configuration, Next.js compiles CSS using PostCSS.To customize PostCSS config, you can create a top-level file called postcss.config.js. This is useful if you’re using libraries like Tailwind CSS.Here are the steps to add Tailwind CSS. We recommend using postcss-preset-env and postcss-flexbugs-fixes to match Next.js’s default behavior. First, install the packages:
```
npm install tailwindcss postcss-preset-env postcss-flexbugs-fixes
```





